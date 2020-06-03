---
title: Adicionar e remover endereços de email da lista de remetentes bloqueados usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Descubra como usar a API gerenciada do EWS ou o EWS para adicionar endereços de email e removê-los da lista de remetentes bloqueados.
ms.openlocfilehash: 270613a739acba165c7bac1bd2c1ef275b5d3aca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528276"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a><span data-ttu-id="4fe48-103">Adicionar e remover endereços de email da lista de remetentes bloqueados usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe48-103">Add and remove email addresses from the Blocked Senders List by using EWS in Exchange</span></span>

<span data-ttu-id="4fe48-104">Descubra como usar a API gerenciada do EWS ou o EWS para adicionar endereços de email e removê-los da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4fe48-104">Find out how to use the EWS Managed API or EWS to add email addresses to and remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="4fe48-105">A lista de remetentes bloqueados nas opções de lixo eletrônico de um usuário oferece uma maneira de mover todas as mensagens de email de remetentes especificados para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="4fe48-105">The Blocked Senders List in a user's Junk Email options provides a way to move all email messages from specified senders to the Junk Email folder.</span></span> <span data-ttu-id="4fe48-106">Você pode habilitar a API gerenciada do EWS ou o aplicativo EWS para adicionar endereços de email ou removê-los da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4fe48-106">You can enable your EWS Managed API or EWS application to add email addresses to or remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="4fe48-107">Observe que uma mensagem do endereço de email deve existir na caixa de correio do usuário antes que você possa adicionar o endereço de email ou removê-lo da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4fe48-107">Note that a message from the email address must exist in the user's mailbox before you can add the email address to or remove it from the Blocked Senders List.</span></span> <span data-ttu-id="4fe48-108">O método [ExchangeService. MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API e a operação [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS usam uma coleção de IDs de item.</span><span class="sxs-lookup"><span data-stu-id="4fe48-108">The [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API method and the [MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS operation use a collection of item IDs.</span></span> <span data-ttu-id="4fe48-109">As IDs de item na coleção indicam mensagens na caixa de correio para a qual o status de lixo eletrônico deve ser alterado.</span><span class="sxs-lookup"><span data-stu-id="4fe48-109">The item IDs in the collection indicate messages in the mailbox for which the junk mail status should be changed.</span></span> 
  
<span data-ttu-id="4fe48-110">Você pode usar os cmdlets [Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx) e [set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) do Shell de gerenciamento do Exchange para acessar a lista de remetentes bloqueados diretamente.</span><span class="sxs-lookup"><span data-stu-id="4fe48-110">You can use the [Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx) and [Set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell cmdlets to access the Blocked Senders List directly.</span></span> 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a><span data-ttu-id="4fe48-111">Adicionar um endereço de email ou removê-lo da lista de remetentes bloqueados usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="4fe48-111">Add an email address to or remove it from the Blocked Senders List by using the EWS Managed API</span></span>
<span data-ttu-id="4fe48-112"><a name="bk_AddRemoveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4fe48-112"><a name="bk_AddRemoveEWSMA"> </a></span></span>

<span data-ttu-id="4fe48-113">Para adicionar o remetente de uma mensagem de email à lista de remetentes bloqueados, use o método **MarkAsJunk** e defina o parâmetro **isjunk** como **true**.</span><span class="sxs-lookup"><span data-stu-id="4fe48-113">To add the sender of an email message to the Blocked Senders List, use the **MarkAsJunk** method and set the **isJunk** parameter to **true**.</span></span> <span data-ttu-id="4fe48-114">Para remover o remetente de uma mensagem de email da lista de remetentes bloqueados, defina o parâmetro **isjunk** como **false**.</span><span class="sxs-lookup"><span data-stu-id="4fe48-114">To remove the sender of an email message from the Blocked Senders List, set the **isJunk** parameter to **false**.</span></span>
  
<span data-ttu-id="4fe48-115">O exemplo a seguir mostra como usar o método **MarkAsJunk** para alterar o status de lixo eletrônico de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="4fe48-115">The following example shows how to use the **MarkAsJunk** method to change the junk status of a message.</span></span> 
  
```cs
private static void MarkMessageAsJunk(ExchangeService service, ItemId messageId, bool isJunk, bool moveItem)
{
    List<ItemId> junkItemIds = new List<ItemId>();
    junkItemIds.Add(messageId);
    ServiceResponseCollection<MarkAsJunkResponse> responseCollection = null;
    try
    {
        // If isJunk is true, the sender of the email message is added to 
        // the Blocked Senders List. If isJunk is false, the sender is removed
        // from the list (if present).
        responseCollection = service.MarkAsJunk(junkItemIds, isJunk, moveItem);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error marking item as junk: {0}", ex.ErrorCode);
        return;
    }
    foreach (MarkAsJunkResponse response in responseCollection)
    {
        if (response.Result == ServiceResult.Success)
        {
            Console.WriteLine("Successfully marked message as {0}junk.", isJunk ? "": "NOT ");
            if (moveItem)
            {
                Console.WriteLine("New item ID: {0}", response.MovedItemId.ToString());
            }
        }
        else
        {
            Console.WriteLine("[{0}]: {1}", response.Result.ToString(),
                response.ErrorCode.ToString());
        }
    }
}
```

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a><span data-ttu-id="4fe48-116">Adicionar um endereço de email ou removê-lo da lista de remetentes bloqueados usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4fe48-116">Add an email address to or remove it from the Blocked Senders List by using EWS</span></span>
<span data-ttu-id="4fe48-117"><a name="bk_AddRemoveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4fe48-117"><a name="bk_AddRemoveEWS"> </a></span></span>

<span data-ttu-id="4fe48-118">A solicitação SOAP do EWS a seguir marca um item como lixo eletrônico Configurando o atributo **isjunk** no elemento [MarkAsJunk](https://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) como **true**.</span><span class="sxs-lookup"><span data-stu-id="4fe48-118">The following EWS SOAP request marks an item as junk by setting the **IsJunk** attribute on the [MarkAsJunk](https://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) element to **true**.</span></span> <span data-ttu-id="4fe48-119">Ele também move a mensagem para a pasta lixo eletrônico definindo o atributo **MoveItem** no elemento **MarkAsJunk** como **true**.</span><span class="sxs-lookup"><span data-stu-id="4fe48-119">It also moves the message to the Junk Email folder by setting the **MoveItem** attribute on the **MarkAsJunk** element to **true**.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:MarkAsJunk IsJunk="true" MoveItem="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4fe48-120">A resposta SOAP do EWS a seguir mostra a resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4fe48-120">The following EWS SOAP response shows the successful response.</span></span> <span data-ttu-id="4fe48-121">O elemento [MovedItemId](https://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) na resposta contém a ID do item após ele ter sido movido.</span><span class="sxs-lookup"><span data-stu-id="4fe48-121">The [MovedItemId](https://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) element in the response contains the item ID for the item after it was moved.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:MovedItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEbAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59DIAAA="
              ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59E+" />
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4fe48-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="4fe48-122">See also</span></span>

- [<span data-ttu-id="4fe48-123">Gerenciamento de caixa de entrada e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe48-123">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)   
- [<span data-ttu-id="4fe48-124">ExchangeService. MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="4fe48-124">ExchangeService.MarkAsJunk</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="4fe48-125">Operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="4fe48-125">MarkAsJunk operation</span></span>](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [<span data-ttu-id="4fe48-126">Get-MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fe48-126">Get-MailboxJunkEmailConfiguration</span></span>](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="4fe48-127">Set-MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fe48-127">Set-MailboxJunkEmailConfiguration</span></span>](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) 
- [<span data-ttu-id="4fe48-128">Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="4fe48-128">Exchange Management Shell</span></span>](../management/exchange-management-shell.md)
    

