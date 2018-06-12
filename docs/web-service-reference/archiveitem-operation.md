---
title: Operação ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Encontre informações sobre o EWS ArchiveItem operação.
ms.openlocfilehash: 954943acefef8da61e92de5f8857ca023ca4fc9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751201"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="ecd00-103">Operação ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ecd00-103">ArchiveItem operation</span></span>

<span data-ttu-id="ecd00-104">Encontre informações sobre a operação de EWS **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="ecd00-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="ecd00-105">A operação **ArchiveItem** move um item em caixa de correio de arquivo morto do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ecd00-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="ecd00-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ecd00-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="ecd00-107">Usando a operação ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ecd00-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="ecd00-108">A operação **ArchiveItem** leva dois argumentos na solicitação que identificam os itens para mover para a caixa de correio de arquivo morto e a pasta de destino para os itens.</span><span class="sxs-lookup"><span data-stu-id="ecd00-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="ecd00-109">Uma caixa de correio de arquivo morto deve ser habilitada para que esta operação funcione.</span><span class="sxs-lookup"><span data-stu-id="ecd00-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="ecd00-110">Para obter informações sobre como habilitar uma caixa de correio de arquivo morto, consulte [Gerenciar o arquivos mortos In-loco](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span><span class="sxs-lookup"><span data-stu-id="ecd00-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="ecd00-111">Cabeçalhos SOAP ArchiveItem operação</span><span class="sxs-lookup"><span data-stu-id="ecd00-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="ecd00-112">A operação **ArchiveItem** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ecd00-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ecd00-113">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="ecd00-113">**Header name**</span></span>|<span data-ttu-id="ecd00-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ecd00-114">**Element**</span></span>|<span data-ttu-id="ecd00-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ecd00-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ecd00-116">**Representação**</span><span class="sxs-lookup"><span data-stu-id="ecd00-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="ecd00-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ecd00-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ecd00-118">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="ecd00-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="ecd00-119">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd00-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ecd00-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="ecd00-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="ecd00-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ecd00-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ecd00-122">Identifica a cultura, conforme definido no RFC 3066, **marcas para a identificação de idiomas**, que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ecd00-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="ecd00-123">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd00-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ecd00-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ecd00-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ecd00-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ecd00-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ecd00-126">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="ecd00-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ecd00-127">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd00-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ecd00-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ecd00-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ecd00-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ecd00-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ecd00-130">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecd00-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ecd00-131">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ecd00-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="ecd00-132">Exemplo de solicitação de operação ArchiveItem: mover um item para a pasta de caixa de entrada de arquivamento</span><span class="sxs-lookup"><span data-stu-id="ecd00-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="ecd00-133">O exemplo a seguir de uma solicitação de operação **ArchiveItem** mostra como mover um item para o pasta caixa de entrada de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="ecd00-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ecd00-134">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ecd00-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ecd00-135">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ecd00-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ecd00-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ecd00-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="ecd00-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="ecd00-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="ecd00-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ecd00-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="ecd00-139">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ecd00-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="ecd00-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="ecd00-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="ecd00-141">Resposta de operação ArchiveItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ecd00-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="ecd00-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **ArchiveItem** para mover um item para uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="ecd00-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ecd00-143">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ecd00-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ecd00-144">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ecd00-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="ecd00-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ecd00-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="ecd00-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ecd00-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="ecd00-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ecd00-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="ecd00-148">Items</span><span class="sxs-lookup"><span data-stu-id="ecd00-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="ecd00-149">Resposta de erro de operação ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ecd00-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="ecd00-150">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="ecd00-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="ecd00-151">Esta é uma resposta a uma solicitação válida para arquivar um item quando uma caixa de correio de arquivo morto não está habilitada para um usuário.</span><span class="sxs-lookup"><span data-stu-id="ecd00-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ecd00-152">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="ecd00-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ecd00-153">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ecd00-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="ecd00-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ecd00-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="ecd00-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ecd00-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="ecd00-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="ecd00-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="ecd00-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ecd00-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="ecd00-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ecd00-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="ecd00-159">Items</span><span class="sxs-lookup"><span data-stu-id="ecd00-159">Items</span></span>](items.md)
    
<span data-ttu-id="ecd00-160">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="ecd00-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ecd00-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="ecd00-161">See also</span></span>

- [<span data-ttu-id="ecd00-162">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ecd00-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="ecd00-163">Arquivamento no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ecd00-163">Archiving in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

