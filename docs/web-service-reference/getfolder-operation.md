---
title: Operação GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: A operação GetFolder obtém pastas do Exchange store.
ms.openlocfilehash: 1d2806e4febb6059b8a866d585bc70f49befbdef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752510"
---
# <a name="getfolder-operation"></a><span data-ttu-id="24df5-103">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="24df5-103">GetFolder operation</span></span>

<span data-ttu-id="24df5-104">A operação **GetFolder** obtém pastas do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="24df5-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="24df5-105">Exemplo de solicitação de GetFolder</span><span class="sxs-lookup"><span data-stu-id="24df5-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="24df5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="24df5-106">Description</span></span>

<span data-ttu-id="24df5-107">O exemplo a seguir de uma solicitação de **GetFolder** mostra como obter um identificador de pasta, nome, a contagem de itens nessa pasta, a contagem de pastas filho e o número de itens não lidos são exibidos na pasta.</span><span class="sxs-lookup"><span data-stu-id="24df5-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="24df5-108">Código</span><span class="sxs-lookup"><span data-stu-id="24df5-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <FolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </FolderIds>
    </GetFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="24df5-109">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24df5-109">Request elements</span></span>

<span data-ttu-id="24df5-110">Essa solicitação **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="24df5-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="24df5-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="24df5-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="24df5-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="24df5-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="24df5-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="24df5-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="24df5-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="24df5-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="24df5-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="24df5-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="24df5-116">Consulte o esquema de elementos adicionais que você pode usar para formar uma solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="24df5-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="24df5-117">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="24df5-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="24df5-118">Exemplo de resposta GetFolder</span><span class="sxs-lookup"><span data-stu-id="24df5-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="24df5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="24df5-119">Description</span></span>

<span data-ttu-id="24df5-120">O exemplo de corpo simples (SOAP Object Access Protocol) a seguir mostra uma resposta bem-sucedida à solicitação de **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="24df5-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="24df5-121">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24df5-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="24df5-122">Código</span><span class="sxs-lookup"><span data-stu-id="24df5-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AQApA=" ChangeKey="AQAAAB" />
              <t:DisplayName>Inbox</t:DisplayName>
              <t:TotalCount>2</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:UnreadCount>2</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="24df5-123">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="24df5-123">Response elements</span></span>

<span data-ttu-id="24df5-124">Essa resposta **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="24df5-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="24df5-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="24df5-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="24df5-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24df5-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="24df5-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24df5-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="24df5-128">Pastas</span><span class="sxs-lookup"><span data-stu-id="24df5-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="24df5-129">Folder</span><span class="sxs-lookup"><span data-stu-id="24df5-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="24df5-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="24df5-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="24df5-131">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="24df5-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="24df5-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="24df5-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="24df5-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="24df5-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="24df5-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="24df5-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="24df5-135">Exemplo de resposta de erro GetFolder</span><span class="sxs-lookup"><span data-stu-id="24df5-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="24df5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="24df5-136">Description</span></span>

<span data-ttu-id="24df5-137">O exemplo de corpo SOAP a seguir mostra uma resposta de erro é gerada por um incorretas [FolderId](folderid.md) na solicitação.</span><span class="sxs-lookup"><span data-stu-id="24df5-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="24df5-138">Código</span><span class="sxs-lookup"><span data-stu-id="24df5-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="24df5-139">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="24df5-139">Response elements</span></span>

<span data-ttu-id="24df5-140">Essa resposta de erro **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="24df5-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="24df5-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="24df5-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="24df5-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="24df5-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="24df5-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24df5-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="24df5-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="24df5-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="24df5-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="24df5-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="24df5-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="24df5-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="24df5-147">Pastas</span><span class="sxs-lookup"><span data-stu-id="24df5-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="24df5-148">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="24df5-148">Version differences</span></span>

<span data-ttu-id="24df5-149">Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="24df5-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="24df5-150">Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="24df5-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="24df5-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="24df5-151">See also</span></span>



- [<span data-ttu-id="24df5-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="24df5-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

