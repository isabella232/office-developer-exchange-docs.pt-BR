---
title: Operação SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: A operação SyncFolderHierarchy sincroniza pastas entre o computador que está executando o Microsoft Exchange Server 2010 e o cliente.
ms.openlocfilehash: 1c7ad2413064161ba54e8a7a30bfcd6f23f218bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456427"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="543da-103">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="543da-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="543da-104">A operação SyncFolderHierarchy sincroniza pastas entre o computador que está executando o Microsoft Exchange Server 2010 e o cliente.</span><span class="sxs-lookup"><span data-stu-id="543da-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="543da-105">A operação SyncFolderHierarchy não retorna pastas quando as propriedades [UnreadCount](unreadcount.md) ou [TotalCount](totalcount.md) foram alteradas.</span><span class="sxs-lookup"><span data-stu-id="543da-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="543da-106">Exemplo de solicitação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="543da-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="543da-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="543da-107">Description</span></span>

<span data-ttu-id="543da-108">O exemplo a seguir de uma solicitação SyncFolderHierarchy mostra como sincronizar uma hierarquia de pastas de cliente com o servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="543da-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="543da-109">Este exemplo mostra uma hierarquia de pastas que já foi sincronizada pelo menos uma vez.</span><span class="sxs-lookup"><span data-stu-id="543da-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="543da-110">O elemento [SyncState](syncstate-ex15websvcsotherref.md) não está incluído na solicitação para a primeira tentativa de sincronizar um cliente com o Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="543da-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="543da-111">A primeira solicitação retornará todas as pastas da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="543da-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="543da-112">O elemento [SyncState](syncstate-ex15websvcsotherref.md) será retornado no [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="543da-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="543da-113">Este elemento é usado para sincronizar o estado das solicitações SyncFolderHierarchy subsequentes.</span><span class="sxs-lookup"><span data-stu-id="543da-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="543da-114">Código</span><span class="sxs-lookup"><span data-stu-id="543da-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="543da-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="543da-115">Comments</span></span>

<span data-ttu-id="543da-116">Os dados codificados em base64 do elemento [SyncState](syncstate-ex15websvcsotherref.md) foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="543da-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="543da-117">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="543da-117">Request elements</span></span>

<span data-ttu-id="543da-118">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="543da-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="543da-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="543da-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="543da-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="543da-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="543da-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="543da-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="543da-122">SyncState</span><span class="sxs-lookup"><span data-stu-id="543da-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="543da-123">O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="543da-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="543da-124">Resposta SyncFolderHierarchy bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="543da-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="543da-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="543da-125">Description</span></span>

<span data-ttu-id="543da-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="543da-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="543da-127">Neste exemplo, uma nova pasta foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="543da-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="543da-128">Código</span><span class="sxs-lookup"><span data-stu-id="543da-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="543da-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="543da-129">Comments</span></span>

<span data-ttu-id="543da-130">O elemento [SyncState](syncstate-ex15websvcsotherref.md) dados codificados em Base64 e os dados de identificador de pasta foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="543da-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="543da-131">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="543da-131">Successful response elements</span></span>

<span data-ttu-id="543da-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="543da-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="543da-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="543da-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="543da-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="543da-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="543da-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="543da-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="543da-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="543da-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="543da-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="543da-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="543da-138">SyncState</span><span class="sxs-lookup"><span data-stu-id="543da-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="543da-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="543da-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="543da-140">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="543da-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="543da-141">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="543da-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="543da-142">Folder</span><span class="sxs-lookup"><span data-stu-id="543da-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="543da-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="543da-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="543da-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="543da-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="543da-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="543da-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="543da-146">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="543da-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="543da-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="543da-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="543da-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="543da-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="543da-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="543da-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="543da-150">Resposta de erro SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="543da-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="543da-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="543da-151">Description</span></span>

<span data-ttu-id="543da-152">O exemplo a seguir mostra uma resposta de erro a uma solicitação SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="543da-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="543da-153">Esse erro foi causado por um SyncState inválido.</span><span class="sxs-lookup"><span data-stu-id="543da-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="543da-154">Código</span><span class="sxs-lookup"><span data-stu-id="543da-154">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="543da-155">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="543da-155">Error response elements</span></span>

<span data-ttu-id="543da-156">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="543da-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="543da-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="543da-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="543da-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="543da-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="543da-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="543da-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="543da-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="543da-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="543da-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="543da-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="543da-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="543da-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="543da-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="543da-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="543da-164">SyncState</span><span class="sxs-lookup"><span data-stu-id="543da-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="543da-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="543da-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="543da-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="543da-166">See also</span></span>



- [<span data-ttu-id="543da-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="543da-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

