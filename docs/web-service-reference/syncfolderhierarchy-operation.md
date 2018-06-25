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
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837681"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="b38a7-103">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b38a7-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="b38a7-104">A operação SyncFolderHierarchy sincroniza pastas entre o computador que está executando o Microsoft Exchange Server 2010 e o cliente.</span><span class="sxs-lookup"><span data-stu-id="b38a7-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="b38a7-105">A operação SyncFolderHierarchy não retorna pastas quando as propriedades [UnreadCount](unreadcount.md) ou [TotalCount](totalcount.md) tem sido alterado.</span><span class="sxs-lookup"><span data-stu-id="b38a7-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="b38a7-106">Exemplo de solicitação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b38a7-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="b38a7-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b38a7-107">Description</span></span>

<span data-ttu-id="b38a7-108">O exemplo a seguir de uma solicitação de SyncFolderHierarchy mostra como sincronizar um cliente de hierarquia de pastas com o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="b38a7-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="b38a7-109">Este exemplo mostra uma hierarquia de pastas que já foi sincronizada pelo menos uma vez.</span><span class="sxs-lookup"><span data-stu-id="b38a7-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="b38a7-110">O elemento de [estado de sincronização](syncstate-ex15websvcsotherref.md) não está incluído na solicitação para a primeira tentativa sincronizar um cliente com o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="b38a7-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="b38a7-111">A primeira solicitação retornará todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b38a7-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="b38a7-112">O elemento de [estado de sincronização](syncstate-ex15websvcsotherref.md) será retornado no [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="b38a7-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="b38a7-113">Esse elemento é usado para sincronizar o estado de solicitações de SyncFolderHierarchy subsequentes.</span><span class="sxs-lookup"><span data-stu-id="b38a7-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="b38a7-114">Código</span><span class="sxs-lookup"><span data-stu-id="b38a7-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b38a7-115">Comments</span><span class="sxs-lookup"><span data-stu-id="b38a7-115">Comments</span></span>

<span data-ttu-id="b38a7-116">Os dados de [estado de sincronização](syncstate-ex15websvcsotherref.md) do elemento codificado na base64 foi reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b38a7-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b38a7-117">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b38a7-117">Request elements</span></span>

<span data-ttu-id="b38a7-118">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="b38a7-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b38a7-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b38a7-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="b38a7-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="b38a7-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="b38a7-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="b38a7-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="b38a7-122">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="b38a7-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="b38a7-123">O esquema que descreve esses elementos está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b38a7-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="b38a7-124">Resposta de SyncFolderHierarchy bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b38a7-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="b38a7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b38a7-125">Description</span></span>

<span data-ttu-id="b38a7-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="b38a7-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="b38a7-127">Neste exemplo, uma nova pasta foi sincronizada.</span><span class="sxs-lookup"><span data-stu-id="b38a7-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="b38a7-128">Código</span><span class="sxs-lookup"><span data-stu-id="b38a7-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="b38a7-129">Comments</span><span class="sxs-lookup"><span data-stu-id="b38a7-129">Comments</span></span>

<span data-ttu-id="b38a7-130">Os dados de [estado de sincronização](syncstate-ex15websvcsotherref.md) do elemento codificado na base64 e os dados da pasta identificador foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b38a7-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="b38a7-131">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b38a7-131">Successful response elements</span></span>

<span data-ttu-id="b38a7-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="b38a7-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b38a7-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b38a7-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b38a7-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="b38a7-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="b38a7-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b38a7-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b38a7-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b38a7-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="b38a7-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b38a7-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b38a7-138">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="b38a7-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b38a7-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="b38a7-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="b38a7-140">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="b38a7-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="b38a7-141">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="b38a7-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="b38a7-142">Folder</span><span class="sxs-lookup"><span data-stu-id="b38a7-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="b38a7-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="b38a7-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="b38a7-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b38a7-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="b38a7-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="b38a7-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="b38a7-146">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="b38a7-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b38a7-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b38a7-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="b38a7-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="b38a7-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="b38a7-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="b38a7-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="b38a7-150">Resposta de erro SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b38a7-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="b38a7-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="b38a7-151">Description</span></span>

<span data-ttu-id="b38a7-152">O exemplo a seguir mostra uma resposta de erro a uma solicitação de SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="b38a7-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="b38a7-153">Esse erro foi causado por um estado de sincronização inválido.</span><span class="sxs-lookup"><span data-stu-id="b38a7-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="b38a7-154">Código</span><span class="sxs-lookup"><span data-stu-id="b38a7-154">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="b38a7-155">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="b38a7-155">Error response elements</span></span>

<span data-ttu-id="b38a7-156">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="b38a7-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b38a7-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b38a7-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b38a7-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="b38a7-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="b38a7-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b38a7-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b38a7-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b38a7-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="b38a7-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="b38a7-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b38a7-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b38a7-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b38a7-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b38a7-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b38a7-164">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="b38a7-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b38a7-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="b38a7-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="b38a7-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="b38a7-166">See also</span></span>



- [<span data-ttu-id="b38a7-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b38a7-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

