---
title: Operação MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Encontre informações sobre a operação do EWS do MarkAllItemsAsRead.
ms.openlocfilehash: aeeacea1cd5eed723f93027dd1ef75b34605fdfd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530527"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="5e11b-103">Operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="5e11b-104">Encontre informações sobre a operação do EWS do **MarkAllItemsAsRead** .</span><span class="sxs-lookup"><span data-stu-id="5e11b-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="5e11b-105">A operação **MarkAllItemsAsRead** define a propriedade [IsRead](isread.md) em todos os itens, em uma ou mais pastas, para indicar que todos os itens são lidos ou não lidos.</span><span class="sxs-lookup"><span data-stu-id="5e11b-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="5e11b-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5e11b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="5e11b-107">Usando a operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="5e11b-108">A operação **MarkAllItemsAsRead** pode definir a propriedade [IsRead](isread.md) em todos os itens em pastas identificadas pelo identificador de pasta dos serviços Web do Exchange (EWS) ou o nome da pasta padrão do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e11b-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="5e11b-109">A operação **MarkAllItemsAsRead** também pode suprimir o envio de confirmações de leitura para itens marcados como lidos.</span><span class="sxs-lookup"><span data-stu-id="5e11b-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="5e11b-110">Cabeçalhos SOAP de operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="5e11b-111">A operação **MarkAllItemsAsRead** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5e11b-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5e11b-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="5e11b-112">**Header name**</span></span>|<span data-ttu-id="5e11b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e11b-113">**Element**</span></span>|<span data-ttu-id="5e11b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e11b-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e11b-115">**Representação**</span><span class="sxs-lookup"><span data-stu-id="5e11b-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5e11b-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5e11b-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5e11b-117">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="5e11b-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5e11b-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5e11b-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5e11b-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5e11b-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5e11b-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5e11b-121">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5e11b-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5e11b-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5e11b-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5e11b-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5e11b-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5e11b-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5e11b-125">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5e11b-126">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5e11b-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5e11b-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5e11b-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5e11b-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5e11b-129">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5e11b-130">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5e11b-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="5e11b-131">Exemplo de solicitação de operação MarkAllItemsAsRead: marcar todos os itens em uma pasta como lidas</span><span class="sxs-lookup"><span data-stu-id="5e11b-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="5e11b-132">O exemplo a seguir de uma solicitação de operação **MarkAllItemsAsRead** mostra como definir a propriedade [IsRead](isread.md) , que também é chamada de sinalizador de leitura, como **true** em todos os itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5e11b-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="5e11b-133">Este exemplo também mostra que as confirmações de leitura não são enviadas em resposta a nenhuma solicitação de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="5e11b-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5e11b-134">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5e11b-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="5e11b-135">As chaves de alteração não são necessárias para esta operação.</span><span class="sxs-lookup"><span data-stu-id="5e11b-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="5e11b-136">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5e11b-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e11b-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="5e11b-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="5e11b-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="5e11b-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="5e11b-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="5e11b-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="5e11b-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="5e11b-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="5e11b-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="5e11b-142">Resposta de operação MarkAllItemsAsRead bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5e11b-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="5e11b-143">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **MarkAllItemsAsRead** para marcar todos os itens de uma pasta como lidos.</span><span class="sxs-lookup"><span data-stu-id="5e11b-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5e11b-144">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5e11b-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e11b-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="5e11b-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="5e11b-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5e11b-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5e11b-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5e11b-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="5e11b-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5e11b-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="5e11b-149">Exemplo de solicitação de operação MarkAllItemsAsRead: marcar todos os itens em uma pasta como não lidas</span><span class="sxs-lookup"><span data-stu-id="5e11b-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="5e11b-150">O exemplo a seguir de uma solicitação de operação **MarkAllItemsAsRead** mostra como definir a propriedade [IsRead](isread.md) como **false** em todos os itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5e11b-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="5e11b-151">Este exemplo também mostra que as confirmações de leitura não são enviadas em resposta a nenhuma solicitação de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="5e11b-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="5e11b-152">Uma resposta bem-sucedida a uma solicitação para marcar todos os itens como lido é o mesmo que a resposta a uma solicitação para marcar todos os itens como não lidos.</span><span class="sxs-lookup"><span data-stu-id="5e11b-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="5e11b-153">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5e11b-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e11b-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="5e11b-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="5e11b-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="5e11b-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="5e11b-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="5e11b-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="5e11b-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="5e11b-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="5e11b-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="5e11b-159">Resposta de erro de operação MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="5e11b-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="5e11b-160">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **MarkAllItemsAsRead** para marcar todos os itens de uma pasta como lidos ou não lidos quando a pasta não existe na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5e11b-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5e11b-161">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5e11b-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e11b-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="5e11b-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="5e11b-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5e11b-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5e11b-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5e11b-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="5e11b-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="5e11b-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5e11b-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5e11b-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5e11b-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5e11b-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="5e11b-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="5e11b-168">See also</span></span>

- [<span data-ttu-id="5e11b-169">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5e11b-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5e11b-170">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="5e11b-170">FindFolder operation</span></span>](findfolder-operation.md)
    

