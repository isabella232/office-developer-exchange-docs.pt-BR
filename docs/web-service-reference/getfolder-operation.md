---
title: Operação GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: A operação GetFolder Obtém pastas do repositório do Exchange.
localization_priority: Priority
ms.openlocfilehash: 9d511f309b9210fd9b5a49ff6c60bc7982992973
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459178"
---
# <a name="getfolder-operation"></a><span data-ttu-id="b6d63-103">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="b6d63-103">GetFolder operation</span></span>

<span data-ttu-id="b6d63-104">A operação **GetFolder** Obtém pastas do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6d63-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="b6d63-105">Exemplo de solicitação GetFolder</span><span class="sxs-lookup"><span data-stu-id="b6d63-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="b6d63-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d63-106">Description</span></span>

<span data-ttu-id="b6d63-107">O exemplo a seguir de uma solicitação **GetFolder** mostra como obter um identificador de pasta, um nome de exibição, a contagem de itens nessa pasta, a contagem de pastas filhas e o número de itens não lidos na pasta.</span><span class="sxs-lookup"><span data-stu-id="b6d63-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b6d63-108">Código</span><span class="sxs-lookup"><span data-stu-id="b6d63-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="request-elements"></a><span data-ttu-id="b6d63-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="b6d63-109">Request elements</span></span>

<span data-ttu-id="b6d63-110">Esta solicitação **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6d63-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="b6d63-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="b6d63-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="b6d63-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="b6d63-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="b6d63-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="b6d63-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="b6d63-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="b6d63-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="b6d63-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="b6d63-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="b6d63-116">Confira o esquema para elementos adicionais que você pode usar para formar uma solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="b6d63-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b6d63-117">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6d63-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="b6d63-118">Exemplo de resposta GetFolder</span><span class="sxs-lookup"><span data-stu-id="b6d63-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="b6d63-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d63-119">Description</span></span>

<span data-ttu-id="b6d63-120">O seguinte exemplo de texto SOAP (protocolo de acesso a objeto simples) mostra uma resposta bem-sucedida à solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="b6d63-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b6d63-121">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6d63-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b6d63-122">Código</span><span class="sxs-lookup"><span data-stu-id="b6d63-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="b6d63-123">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="b6d63-123">Response elements</span></span>

<span data-ttu-id="b6d63-124">Esta resposta **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6d63-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="b6d63-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b6d63-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="b6d63-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b6d63-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b6d63-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b6d63-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="b6d63-128">Pastas</span><span class="sxs-lookup"><span data-stu-id="b6d63-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b6d63-129">Folder</span><span class="sxs-lookup"><span data-stu-id="b6d63-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="b6d63-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="b6d63-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="b6d63-131">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="b6d63-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="b6d63-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b6d63-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="b6d63-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="b6d63-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="b6d63-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="b6d63-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="b6d63-135">Exemplo de resposta de erro GetFolder</span><span class="sxs-lookup"><span data-stu-id="b6d63-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b6d63-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d63-136">Description</span></span>

<span data-ttu-id="b6d63-137">O seguinte exemplo de corpo SOAP mostra uma resposta de erro causada por uma [FolderId](folderid.md) incorreta na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d63-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b6d63-138">Código</span><span class="sxs-lookup"><span data-stu-id="b6d63-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="b6d63-139">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="b6d63-139">Response elements</span></span>

<span data-ttu-id="b6d63-140">Esta resposta de erro **GetFolder** inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b6d63-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="b6d63-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="b6d63-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="b6d63-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b6d63-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b6d63-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b6d63-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="b6d63-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="b6d63-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b6d63-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b6d63-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b6d63-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b6d63-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="b6d63-147">Pastas</span><span class="sxs-lookup"><span data-stu-id="b6d63-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="b6d63-148">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="b6d63-148">Version differences</span></span>

<span data-ttu-id="b6d63-149">Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b6d63-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="b6d63-150">Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="b6d63-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b6d63-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6d63-151">See also</span></span>



- [<span data-ttu-id="b6d63-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6d63-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

