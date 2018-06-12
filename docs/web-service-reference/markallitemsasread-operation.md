---
title: Operação MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Encontre informações sobre o EWS MarkAllItemsAsRead operação.
ms.openlocfilehash: 995a6219f0a3b41bddb0d65c875d981322e1ce78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824354"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="89d19-103">Operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="89d19-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="89d19-104">Encontre informações sobre a operação de EWS **MarkAllItemsAsRead** .</span><span class="sxs-lookup"><span data-stu-id="89d19-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="89d19-105">A operação **MarkAllItemsAsRead** define a propriedade [foi lido](isread.md) em todos os itens, uma ou mais pastas para indicar que todos os itens são lidos ou não lidos.</span><span class="sxs-lookup"><span data-stu-id="89d19-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="89d19-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89d19-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="89d19-107">Usando a operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="89d19-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="89d19-108">A operação **MarkAllItemsAsRead** pode definir a propriedade [foi lido](isread.md) em todos os itens nas pastas identificados pelo identificador de pasta de serviços Web do Exchange (EWS) ou o nome de pasta padrão do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89d19-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="89d19-109">A operação **MarkAllItemsAsRead** também pode suprimir o envio de confirmações de leitura para os itens marcados como lidos.</span><span class="sxs-lookup"><span data-stu-id="89d19-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="89d19-110">Cabeçalhos SOAP MarkAllItemsAsRead operação</span><span class="sxs-lookup"><span data-stu-id="89d19-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="89d19-111">A operação **MarkAllItemsAsRead** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="89d19-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="89d19-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="89d19-112">**Header name**</span></span>|<span data-ttu-id="89d19-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89d19-113">**Element**</span></span>|<span data-ttu-id="89d19-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89d19-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="89d19-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="89d19-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="89d19-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="89d19-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="89d19-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="89d19-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="89d19-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="89d19-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="89d19-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="89d19-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="89d19-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="89d19-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="89d19-121">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="89d19-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="89d19-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="89d19-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="89d19-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="89d19-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="89d19-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="89d19-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="89d19-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="89d19-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="89d19-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="89d19-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="89d19-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="89d19-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="89d19-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="89d19-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="89d19-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="89d19-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="89d19-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="89d19-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="89d19-131">Exemplo de solicitação de operação MarkAllItemsAsRead: marcar todos os itens em uma pasta como lida</span><span class="sxs-lookup"><span data-stu-id="89d19-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="89d19-132">O exemplo a seguir de uma solicitação de operação **MarkAllItemsAsRead** mostra como definir a propriedade [foi lido](isread.md) , que também é chamada o sinalizador de leitura, como **true** em todos os itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="89d19-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="89d19-133">Este exemplo também mostra read confirmações não são enviadas em resposta às solicitações de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="89d19-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="89d19-134">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="89d19-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="89d19-135">Alterar chaves não são necessárias para essa operação.</span><span class="sxs-lookup"><span data-stu-id="89d19-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="89d19-136">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="89d19-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="89d19-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="89d19-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="89d19-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="89d19-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="89d19-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="89d19-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="89d19-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="89d19-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="89d19-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="89d19-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="89d19-142">Resposta de operação MarkAllItemsAsRead bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="89d19-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="89d19-143">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **MarkAllItemsAsRead** para marcar todos os itens em uma pasta como lidos.</span><span class="sxs-lookup"><span data-stu-id="89d19-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="89d19-144">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="89d19-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="89d19-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="89d19-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="89d19-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="89d19-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="89d19-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="89d19-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="89d19-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="89d19-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="89d19-149">Exemplo de solicitação de operação MarkAllItemsAsRead: marcar todos os itens em uma pasta como não lido</span><span class="sxs-lookup"><span data-stu-id="89d19-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="89d19-150">O exemplo a seguir de uma solicitação de operação **MarkAllItemsAsRead** mostra como definir a propriedade [foi lido](isread.md) como **false** em todos os itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="89d19-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="89d19-151">Este exemplo também mostra read confirmações não são enviadas em resposta às solicitações de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="89d19-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
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
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="89d19-152">Uma resposta bem-sucedida a uma solicitação para marcar todos os itens como lidos é o mesmo que a resposta a uma solicitação para marcar todos os itens como não lidos.</span><span class="sxs-lookup"><span data-stu-id="89d19-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="89d19-153">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="89d19-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="89d19-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="89d19-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="89d19-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="89d19-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="89d19-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="89d19-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="89d19-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="89d19-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="89d19-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="89d19-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="89d19-159">Resposta de erro de operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="89d19-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="89d19-160">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **MarkAllItemsAsRead** para marcar todos os itens em uma pasta como lidos ou não lidos quando a pasta não existir na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="89d19-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="89d19-161">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="89d19-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="89d19-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="89d19-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="89d19-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="89d19-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="89d19-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="89d19-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="89d19-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="89d19-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="89d19-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="89d19-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="89d19-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="89d19-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="89d19-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="89d19-168">See also</span></span>

- [<span data-ttu-id="89d19-169">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="89d19-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="89d19-170">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="89d19-170">FindFolder operation</span></span>](findfolder-operation.md)
    

