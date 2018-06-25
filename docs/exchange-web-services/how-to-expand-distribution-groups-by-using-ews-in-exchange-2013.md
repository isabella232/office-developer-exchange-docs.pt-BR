---
title: Expandir grupos de distribuição, usando o EWS no Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Saiba como expandir um grupo de distribuição usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750710"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Expandir grupos de distribuição, usando o EWS no Exchange 2013

Saiba como expandir um grupo de distribuição usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar o método de API gerenciada de EWS [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou a operação de EWS [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) para expandir um grupo de distribuição para identificar todos os destinatários. 
  
Porque o método [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) está sobrecarregado, você poderá chamá-lo de várias maneiras: 
  
- [ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - se expande um grupo identificado por um endereço SMTP. 
    
- [ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - se expande um grupo identificado por um endereço de email. 
    
- [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - expande um grupo identificado por um ID de grupo. 
    
- [ExpanGroup (String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - expande um grupo identificado por um endereço SMTP e o tipo de roteamento de endereço. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Expanda um grupo de distribuição universal ou grupo de segurança usando a API gerenciada de EWS
<a name="bk_ExpandDGEWSMA"> </a>

O exemplo a seguir mostra como expandir um grupo de distribuição universal ou grupo de segurança usando um endereço de email, que é a abordagem mais simples. Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Isso não é muito código, mas também é bem básico e podem não dar o que você está procurando. Vamos ele uma etapa adicional. Grupos de distribuição também podem conter outros grupos de distribuição. Simplesmente a expansão dos grupos de distribuição contidos o endereço de email de saída mas não expandi-las. Adicionando mais algumas linhas de código, você pode recursivamente expanda os grupos para gerar a saída de cada contato.
  
```cs
private static void ExpandDistributionLists(ExchangeService service, string Mailbox)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(Mailbox);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         // Check to see if the mailbox is a public group
         if (address.MailboxType == MailboxType.PublicGroup)
      {
         // Call the function again to expand the contained
         // distribution group.
         ExpandDistributionLists(service, address.Address);
      }
      else
      {
         // Output the address of the mailbox.
         Console.WriteLine("Email Address: {0}", address);
      }
   }
}

```

E agora você pode chamar essa nova função no seu código e expanda todos os grupos de distribuição pública contidos no primeiro.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Expandir um grupo de contatos, usando a API gerenciada de EWS
<a name="bk_ExpandDGEWSMA"> </a>

Porque não têm um endereço de email associado grupos de contatos, você precisa expandir o grupo com base no ItemId usando o método [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) . Você pode criar uma função, conforme mostrado no exemplo anterior e alterar o segundo tipo de parâmetro de uma cadeia de caracteres para um [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
```cs
private static void ExpandContactGroup(ExchangeService service, ItemId groupID)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(groupID);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         if (address.MailboxType == MailboxType.PublicGroup)
         {
            ExpandDistributionLists(service, address.Address);
         }
         else
         {
            Console.WriteLine("Email Address: {0}", address);
         }
      }
}
```

Agora você pode chamar essa função usando o objeto de serviço do Exchange e o **ItemId** do grupo de contatos. Observe que o **ItemId** no exemplo é reduzido para melhorar a legibilidade. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Expandir um grupo de distribuição universal ou grupo de segurança, usando o EWS
<a name="bk_ExpandDGEWSMA"> </a>

O exemplo a seguir mostra a mensagem de solicitação XML que é enviada do cliente para o servidor quando você usar a operação [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) . Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Expandir um grupo de distribuição universal](#bk_ExpandDGEWSMA). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a mensagem de resposta XML que é enviada do servidor para o cliente. Observe que as caixas de correio e grupos de distribuição universal são retornados.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Support</Name>
          <EmailAddress>support@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
      </DLExpansion>
    </ExpandDLResponseMessage>
  </ResponseMessages>
</ExpandDLResponse>
</s:Body>
</s:Envelope>
```

Ao contrário de quando você usa o EWS Managed API, quando você usa o EWS para expandir um grupo de distribuição universal, você não pode recursivamente expanda os grupos de distribuição que são retornados. Você precisará enviar uma solicitação adicional para expandir cada um dos grupos de distribuição, incluídos na resposta.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Expandir um grupo de contatos usando o EWS
<a name="bk_ExpandDGEWSMA"> </a>

A solicitação XML para expandir um grupo de contatos é semelhante a uma solicitação para expandir um grupo de distribuição. Em vez de um endereço de email, você deve usar o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do grupo de contatos. O **ItemId** neste exemplo é abreviada para fins de legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

A estrutura da resposta XML a uma solicitação para expandir um grupo de contatos é o mesmo que a resposta a uma solicitação para expandir um grupo de distribuição universal.
  
## <a name="see-also"></a>Confira também


- [Grupos de distribuição e EWS no Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Criar grupos de contatos usando o EWS no Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

