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
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a><span data-ttu-id="62623-103">Expandir grupos de distribuição, usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="62623-103">Expand distribution groups by using EWS in Exchange 2013</span></span>

<span data-ttu-id="62623-104">Saiba como expandir um grupo de distribuição usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="62623-104">Learn how to expand a distribution group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="62623-105">Você pode usar o método de API gerenciada de EWS [ExchangeService.ExpandGroup](http://msdn.microsoft.com/pt-br/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) ou a operação de EWS [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) para expandir um grupo de distribuição para identificar todos os destinatários.</span><span class="sxs-lookup"><span data-stu-id="62623-105">You can use the [ExchangeService.ExpandGroup](http://msdn.microsoft.com/pt-br/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS operation to expand a distribution group to identify all recipients.</span></span> 
  
<span data-ttu-id="62623-106">Porque o método [ExpandGroup](http://msdn.microsoft.com/pt-br/library/office/ee344007%28v=exchg.80%29.aspx) está sobrecarregado, você poderá chamá-lo de várias maneiras:</span><span class="sxs-lookup"><span data-stu-id="62623-106">Because the [ExpandGroup](http://msdn.microsoft.com/pt-br/library/office/ee344007%28v=exchg.80%29.aspx) method is overloaded, you can call it in several ways:</span></span> 
  
- <span data-ttu-id="62623-107">[ExpandGroup(String)](http://msdn.microsoft.com/pt-br/library/office/ee343988%28v=exchg.80%29.aspx) - se expande um grupo identificado por um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="62623-107">[ExpandGroup(String)](http://msdn.microsoft.com/pt-br/library/office/ee343988%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address.</span></span> 
    
- <span data-ttu-id="62623-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/pt-br/library/office/ee344007%28v=exchg.80%29.aspx) - se expande um grupo identificado por um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="62623-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/pt-br/library/office/ee344007%28v=exchg.80%29.aspx) - Expands a group identified by an email address.</span></span> 
    
- <span data-ttu-id="62623-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/pt-br/library/office/ee356407%28v=exchg.80%29.aspx) - expande um grupo identificado por um ID de grupo.</span><span class="sxs-lookup"><span data-stu-id="62623-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/pt-br/library/office/ee356407%28v=exchg.80%29.aspx) - Expands a group identified by a group ID.</span></span> 
    
- <span data-ttu-id="62623-110">[ExpanGroup (String, String)](http://msdn.microsoft.com/pt-br/library/office/ee356468%28v=exchg.80%29.aspx) - expande um grupo identificado por um endereço SMTP e o tipo de roteamento de endereço.</span><span class="sxs-lookup"><span data-stu-id="62623-110">[ExpanGroup(String, String)](http://msdn.microsoft.com/pt-br/library/office/ee356468%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address and the routing type of that address.</span></span> 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a><span data-ttu-id="62623-111">Expanda um grupo de distribuição universal ou grupo de segurança usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="62623-111">Expand a universal distribution group or security group by using EWS Managed API</span></span>
<span data-ttu-id="62623-112"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62623-112"></span></span>

<span data-ttu-id="62623-113">O exemplo a seguir mostra como expandir um grupo de distribuição universal ou grupo de segurança usando um endereço de email, que é a abordagem mais simples.</span><span class="sxs-lookup"><span data-stu-id="62623-113">The following example shows how to expand a universal distribution group or security group by using an email address, which is the simplest approach.</span></span> <span data-ttu-id="62623-114">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="62623-114">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

<span data-ttu-id="62623-115">Isso não é muito código, mas também é bem básico e podem não dar o que você está procurando.</span><span class="sxs-lookup"><span data-stu-id="62623-115">That's not a lot of code, but it's also pretty basic and might not give you what you are looking for.</span></span> <span data-ttu-id="62623-116">Vamos ele uma etapa adicional.</span><span class="sxs-lookup"><span data-stu-id="62623-116">So let's take it a step further.</span></span> <span data-ttu-id="62623-117">Grupos de distribuição também podem conter outros grupos de distribuição.</span><span class="sxs-lookup"><span data-stu-id="62623-117">Distribution groups can also contain other distribution groups.</span></span> <span data-ttu-id="62623-118">Simplesmente a expansão dos grupos de distribuição contidos o endereço de email de saída mas não expandi-las.</span><span class="sxs-lookup"><span data-stu-id="62623-118">Simply expanding it will output the email address of the contained distribution groups but not expand them.</span></span> <span data-ttu-id="62623-119">Adicionando mais algumas linhas de código, você pode recursivamente expanda os grupos para gerar a saída de cada contato.</span><span class="sxs-lookup"><span data-stu-id="62623-119">By adding a few more lines of code, you can recursively expand the groups to output every contact.</span></span>
  
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

<span data-ttu-id="62623-120">E agora você pode chamar essa nova função no seu código e expanda todos os grupos de distribuição pública contidos no primeiro.</span><span class="sxs-lookup"><span data-stu-id="62623-120">And now you can call this new function in the your code and expand all the public distribution groups contained within the first one.</span></span>
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a><span data-ttu-id="62623-121">Expandir um grupo de contatos, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="62623-121">Expand a contact group by using EWS Managed API</span></span>
<span data-ttu-id="62623-122"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62623-122"></span></span>

<span data-ttu-id="62623-123">Porque não têm um endereço de email associado grupos de contatos, você precisa expandir o grupo com base no ItemId usando o método [ExpandGroup(ItemId)](http://msdn.microsoft.com/pt-br/library/office/ee356407%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="62623-123">Because contact groups do not have an associated email address, you need to expand the group based on the ItemId by using the [ExpandGroup(ItemId)](http://msdn.microsoft.com/pt-br/library/office/ee356407%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="62623-124">Você pode criar uma função, conforme mostrado no exemplo anterior e alterar o segundo tipo de parâmetro de uma cadeia de caracteres para um [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="62623-124">You can create a function, as shown in the previous example, and change the second parameter type from a string to an [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span></span>
  
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

<span data-ttu-id="62623-125">Agora você pode chamar essa função usando o objeto de serviço do Exchange e o **ItemId** do grupo de contatos.</span><span class="sxs-lookup"><span data-stu-id="62623-125">Now you can call this function by using the Exchange service object and the **ItemId** of the contact group.</span></span> <span data-ttu-id="62623-126">Observe que o **ItemId** no exemplo é reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62623-126">Note that the **ItemId** in the example is shortened for readability.</span></span> 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a><span data-ttu-id="62623-127">Expandir um grupo de distribuição universal ou grupo de segurança, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="62623-127">Expand a universal distribution group or security group by using EWS</span></span>
<span data-ttu-id="62623-128"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62623-128"></span></span>

<span data-ttu-id="62623-129">O exemplo a seguir mostra a mensagem de solicitação XML que é enviada do cliente para o servidor quando você usar a operação [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="62623-129">The following example shows the XML request message that is sent from the client to the server when you use the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="62623-130">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Expandir um grupo de distribuição universal](#bk_ExpandDGEWSMA).</span><span class="sxs-lookup"><span data-stu-id="62623-130">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [expand a universal distribution group](#bk_ExpandDGEWSMA).</span></span> 
  
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

<span data-ttu-id="62623-131">O exemplo a seguir mostra a mensagem de resposta XML que é enviada do servidor para o cliente.</span><span class="sxs-lookup"><span data-stu-id="62623-131">The following example shows the XML response message that is sent from the server to the client.</span></span> <span data-ttu-id="62623-132">Observe que as caixas de correio e grupos de distribuição universal são retornados.</span><span class="sxs-lookup"><span data-stu-id="62623-132">Notice that both mailboxes and universal distribution groups are returned.</span></span>
  
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

<span data-ttu-id="62623-133">Ao contrário de quando você usa o EWS Managed API, quando você usa o EWS para expandir um grupo de distribuição universal, você não pode recursivamente expanda os grupos de distribuição que são retornados.</span><span class="sxs-lookup"><span data-stu-id="62623-133">Unlike when you use the EWS Managed API, when you use EWS to expand a universal distribution group, you can't recursively expand the distribution groups that are returned.</span></span> <span data-ttu-id="62623-134">Você precisará enviar uma solicitação adicional para expandir cada um dos grupos de distribuição, incluídos na resposta.</span><span class="sxs-lookup"><span data-stu-id="62623-134">You will need to send an additional request to expand each of the distribution groups included in the response.</span></span>
  
## <a name="expand-a-contact-group-by-using-ews"></a><span data-ttu-id="62623-135">Expandir um grupo de contatos usando o EWS</span><span class="sxs-lookup"><span data-stu-id="62623-135">Expand a contact group by using EWS</span></span>
<span data-ttu-id="62623-136"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62623-136"></span></span>

<span data-ttu-id="62623-137">A solicitação XML para expandir um grupo de contatos é semelhante a uma solicitação para expandir um grupo de distribuição.</span><span class="sxs-lookup"><span data-stu-id="62623-137">The XML request to expand a contact group is similar to a request to expand a distribution group.</span></span> <span data-ttu-id="62623-138">Em vez de um endereço de email, você deve usar o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do grupo de contatos.</span><span class="sxs-lookup"><span data-stu-id="62623-138">Instead of an email address, you use the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the contact group.</span></span> <span data-ttu-id="62623-139">O **ItemId** neste exemplo é abreviada para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="62623-139">The **ItemId** in this example is shortened for readability.</span></span> 
  
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

<span data-ttu-id="62623-140">A estrutura da resposta XML a uma solicitação para expandir um grupo de contatos é o mesmo que a resposta a uma solicitação para expandir um grupo de distribuição universal.</span><span class="sxs-lookup"><span data-stu-id="62623-140">The structure of the XML response to a request to expand a contact group is the same as the response to a request to expand a universal distribution group.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="62623-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="62623-141">See also</span></span>


- [<span data-ttu-id="62623-142">Grupos de distribuição e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="62623-142">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="62623-143">Criar grupos de contatos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="62623-143">Create contact groups by using EWS in Exchange</span></span>](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

