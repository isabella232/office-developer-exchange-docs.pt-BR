---
title: Adicionar e remover os endereços de email da lista de remetentes bloqueados usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Descubra como usar a API gerenciada de EWS ou o EWS para adicionar endereços de e-mail e removê-los da lista de remetentes bloqueados.
ms.openlocfilehash: c03ed585ebd62802000179d8c837786ba5f9aab4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750667"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a><span data-ttu-id="c8cf2-103">Adicionar e remover os endereços de email da lista de remetentes bloqueados usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8cf2-103">Add and remove email addresses from the Blocked Senders List by using EWS in Exchange</span></span>

<span data-ttu-id="c8cf2-104">Descubra como usar a API gerenciada de EWS ou o EWS para adicionar endereços de e-mail e removê-los da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-104">Find out how to use the EWS Managed API or EWS to add email addresses to and remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="c8cf2-105">A lista de remetentes bloqueados nas opções de lixo eletrônico do usuário fornece uma maneira de mover todos os emails de remetentes especificados para a pasta Lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-105">The Blocked Senders List in a user's Junk Email options provides a way to move all email messages from specified senders to the Junk Email folder.</span></span> <span data-ttu-id="c8cf2-106">É possível habilitar o EWS Managed API ou o aplicativo de EWS adicionar endereços de e-mail ou removê-los da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-106">You can enable your EWS Managed API or EWS application to add email addresses to or remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="c8cf2-107">Observe que uma mensagem a partir do endereço de email deve existir na caixa de correio do usuário antes de adicionar o endereço de email para ou removê-lo da lista de remetentes bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-107">Note that a message from the email address must exist in the user's mailbox before you can add the email address to or remove it from the Blocked Senders List.</span></span> <span data-ttu-id="c8cf2-108">O método [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API e a operação de EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) usam um conjunto de IDs de item.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-108">The [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API method and the [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS operation use a collection of item IDs.</span></span> <span data-ttu-id="c8cf2-109">O item IDs na coleção indicam mensagens na caixa de correio para o qual o status de lixo eletrônico deve ser alterado.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-109">The item IDs in the collection indicate messages in the mailbox for which the junk mail status should be changed.</span></span> 
  
<span data-ttu-id="c8cf2-110">Você pode usar os cmdlets [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) e o Shell de gerenciamento do Exchange [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) para acessar a lista de remetentes bloqueados diretamente.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-110">You can use the [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) and [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell cmdlets to access the Blocked Senders List directly.</span></span> 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a><span data-ttu-id="c8cf2-111">Adicionar um endereço de email para ou removê-lo da lista de remetentes bloqueados usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="c8cf2-111">Add an email address to or remove it from the Blocked Senders List by using the EWS Managed API</span></span>
<span data-ttu-id="c8cf2-112"><a name="bk_AddRemoveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="c8cf2-112"></span></span>

<span data-ttu-id="c8cf2-113">Para adicionar o remetente de uma mensagem de email à lista de remetentes bloqueados, use o método **MarkAsJunk** e defina o parâmetro **isJunk** como **true**.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-113">To add the sender of an email message to the Blocked Senders List, use the **MarkAsJunk** method and set the **isJunk** parameter to **true**.</span></span> <span data-ttu-id="c8cf2-114">Para remover o remetente de uma mensagem de email da lista de remetentes bloqueados, defina o parâmetro **isJunk** como **false**.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-114">To remove the sender of an email message from the Blocked Senders List, set the **isJunk** parameter to **false**.</span></span>
  
<span data-ttu-id="c8cf2-115">O exemplo a seguir mostra como usar o método **MarkAsJunk** para alterar o status de lixo eletrônico de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-115">The following example shows how to use the **MarkAsJunk** method to change the junk status of a message.</span></span> 
  
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

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a><span data-ttu-id="c8cf2-116">Adicionar um endereço de email para ou removê-lo da lista de remetentes bloqueados usando o EWS</span><span class="sxs-lookup"><span data-stu-id="c8cf2-116">Add an email address to or remove it from the Blocked Senders List by using EWS</span></span>
<span data-ttu-id="c8cf2-117"><a name="bk_AddRemoveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="c8cf2-117"></span></span>

<span data-ttu-id="c8cf2-118">A solicitação de EWS SOAP a seguir marca um item como lixo eletrônico, definindo o atributo **IsJunk** no elemento [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) como **true**.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-118">The following EWS SOAP request marks an item as junk by setting the **IsJunk** attribute on the [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) element to **true**.</span></span> <span data-ttu-id="c8cf2-119">Ele também move a mensagem para a pasta Lixo eletrônico, definindo o atributo **MoveItem** no elemento **MarkAsJunk** como **true**.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-119">It also moves the message to the Junk Email folder by setting the **MoveItem** attribute on the **MarkAsJunk** element to **true**.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="c8cf2-120">A seguinte resposta SOAP EWS mostra a resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-120">The following EWS SOAP response shows the successful response.</span></span> <span data-ttu-id="c8cf2-121">O elemento [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) na resposta contém a ID de item para o item depois que ele foi movido.</span><span class="sxs-lookup"><span data-stu-id="c8cf2-121">The [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) element in the response contains the item ID for the item after it was moved.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="c8cf2-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8cf2-122">See also</span></span>

- [<span data-ttu-id="c8cf2-123">Gerenciamento de caixa de entrada e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c8cf2-123">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)   
- [<span data-ttu-id="c8cf2-124">ExchangeService.MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="c8cf2-124">ExchangeService.MarkAsJunk</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="c8cf2-125">Operação MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="c8cf2-125">MarkAsJunk operation</span></span>](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [<span data-ttu-id="c8cf2-126">Get-MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8cf2-126">Get-MailboxJunkEmailConfiguration</span></span>](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="c8cf2-127">Set-MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8cf2-127">Set-MailboxJunkEmailConfiguration</span></span>](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) 
- [<span data-ttu-id="c8cf2-128">Shell de Gerenciamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="c8cf2-128">Exchange Management Shell</span></span>](../management/exchange-management-shell.md)
    

