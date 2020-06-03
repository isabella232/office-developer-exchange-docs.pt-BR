---
title: Expandir grupos de distribuição usando EWS no Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Saiba como expandir um grupo de distribuição usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 2cbeb65b5a722bce4d5cab8fd716230874a6afca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528115"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Expandir grupos de distribuição usando EWS no Exchange 2013

Saiba como expandir um grupo de distribuição usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar o método de API gerenciada do EWS [ExchangeService. Expand](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou a operação de [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS para expandir um grupo de distribuição para identificar todos os destinatários. 
  
Como o método [expandobject](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) está sobrecarregado, você pode chamá-lo de várias maneiras: 
  
- [Expand (cadeia de caracteres)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx) -expande um grupo identificado por um endereço SMTP. 
    
- [Expando (EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) -expande um grupo identificado por um endereço de email. 
    
- [Expando (ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) -expande um grupo identificado por uma ID de grupo. 
    
- [ExpanGroup (String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx) -expande um grupo identificado por um endereço SMTP e o tipo de roteamento desse endereço. 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>Expanda um grupo de distribuição universal ou um grupo de segurança usando a API gerenciada do EWS
<a name="bk_ExpandDGEWSMA"> </a>

O exemplo a seguir mostra como expandir um grupo de distribuição universal ou grupo de segurança usando um endereço de email, que é a abordagem mais simples. Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

Isso não é muito código, mas também é bem básico e pode não fornecer o que você está procurando. Então vamos dar um passo adiante. Os grupos de distribuição também podem conter outros grupos de distribuição. Simplesmente expandi-lo produzirá o endereço de email dos grupos de distribuição contidos, mas não os expandirá. Ao adicionar mais algumas linhas de código, você pode expandir recursivamente os grupos para dar saída a todos os contatos.
  
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

E agora você pode chamar essa nova função no seu código e expandir todos os grupos de distribuição pública contidos no primeiro.
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>Expandir um grupo de contatos usando a API gerenciada do EWS
<a name="bk_ExpandDGEWSMA"> </a>

Como os grupos de contatos não têm um endereço de email associado, você precisa expandir o grupo com base no ItemId usando o método [expando (ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) . Você pode criar uma função, conforme mostrado no exemplo anterior, e alterar o segundo tipo de parâmetro de uma cadeia de caracteres para uma [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).
  
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

Agora você pode chamar essa função usando o objeto de serviço do Exchange e o **ItemId** do grupo de contatos. Observe que o **ItemId** no exemplo é reduzido para facilitar a leitura. 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>Expanda um grupo de distribuição universal ou um grupo de segurança usando o EWS
<a name="bk_ExpandDGEWSMA"> </a>

O exemplo a seguir mostra a mensagem de solicitação XML que é enviada do cliente para o servidor quando você usa a operação [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) . Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [expandir um grupo de distribuição universal](#bk_ExpandDGEWSMA). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a mensagem de resposta XML que é enviada do servidor para o cliente. Observe que as caixas de correio e os grupos de distribuição universais são retornados.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Ao contrário de quando você usa a API gerenciada do EWS, quando usa o EWS para expandir um grupo de distribuição universal, você não pode expandir recursivamente os grupos de distribuição que são retornados. Você precisará enviar uma solicitação adicional para expandir cada um dos grupos de distribuição incluídos na resposta.
  
## <a name="expand-a-contact-group-by-using-ews"></a>Expandir um grupo de contatos usando o EWS
<a name="bk_ExpandDGEWSMA"> </a>

A solicitação XML para expandir um grupo de contatos é semelhante a uma solicitação para expandir um grupo de distribuição. Em vez de um endereço de email, você usa o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do grupo de contatos. O **ItemId** neste exemplo foi reduzido para legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

A estrutura da resposta XML a uma solicitação para expandir um grupo de contatos é o mesmo que a resposta a uma solicitação para expandir um grupo de distribuição universal.
  
## <a name="see-also"></a>Confira também


- [Grupos de distribuição e EWS no Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Criar grupos de contatos usando o EWS no Exchange](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

