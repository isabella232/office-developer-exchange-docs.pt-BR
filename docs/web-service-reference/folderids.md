---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: O elemento FolderIds contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar as notificações de eventos.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752333"
---
# <a name="folderids"></a><span data-ttu-id="92414-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="92414-103">FolderIds</span></span>

<span data-ttu-id="92414-104">O elemento **FolderIds** contém uma matriz de identificadores de pasta que são usados para identificar pastas para copiar, mover, obter, excluir ou monitorar as notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="92414-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="92414-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="92414-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92414-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="92414-106">Attributes and elements</span></span>

<span data-ttu-id="92414-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="92414-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92414-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="92414-108">Attributes</span></span>

<span data-ttu-id="92414-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="92414-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92414-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="92414-110">Child elements</span></span>

|<span data-ttu-id="92414-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92414-111">**Element**</span></span>|<span data-ttu-id="92414-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92414-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92414-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="92414-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="92414-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="92414-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="92414-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="92414-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="92414-116">Identifica as pastas do Microsoft Exchange Server que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="92414-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92414-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="92414-117">Parent elements</span></span>

|<span data-ttu-id="92414-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92414-118">**Element**</span></span>|<span data-ttu-id="92414-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92414-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92414-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="92414-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="92414-121">Define uma solicitação para obter uma pasta do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="92414-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="92414-122">Este é a expressão XPath para esse elemento:`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="92414-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="92414-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="92414-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="92414-124">Define uma solicitação para excluir pastas do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="92414-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="92414-125">Este é a expressão XPath para esse elemento:`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="92414-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="92414-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="92414-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="92414-127">Define uma solicitação para excluir pastas do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="92414-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="92414-128">Este é a expressão XPath para esse elemento:`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="92414-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="92414-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="92414-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="92414-130">Define uma solicitação para mover uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92414-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="92414-131">Este é a expressão XPath para esse elemento:`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="92414-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="92414-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="92414-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="92414-133">Define uma solicitação para copiar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92414-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="92414-134">Este é a expressão XPath para esse elemento:`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="92414-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="92414-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="92414-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="92414-136">Representa uma assinatura para uma inscrição de notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="92414-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="92414-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="92414-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="92414-138">Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.</span><span class="sxs-lookup"><span data-stu-id="92414-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92414-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="92414-139">Remarks</span></span>

<span data-ttu-id="92414-140">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="92414-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92414-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="92414-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92414-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="92414-142">Namespace</span></span>  <br/> |<span data-ttu-id="92414-143">http://schemas.microsoft.com/exchange/services/2006/messages e http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="92414-143">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="92414-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="92414-144">Schema Name</span></span>  <br/> |<span data-ttu-id="92414-145">Esquema de mensagens; Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="92414-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="92414-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="92414-146">Validation File</span></span>  <br/> |<span data-ttu-id="92414-147">Messages.xsd; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92414-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92414-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="92414-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="92414-149">False</span><span class="sxs-lookup"><span data-stu-id="92414-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92414-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="92414-150">See also</span></span>



[<span data-ttu-id="92414-151">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="92414-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="92414-152">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="92414-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="92414-153">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="92414-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="92414-154">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="92414-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="92414-155">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="92414-155">Subscribe operation</span></span>](subscribe-operation.md)

