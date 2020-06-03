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
description: O elemento FolderIds contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem copiadas, movidas, obtidas, excluídas ou monitoradas para notificações de eventos.
ms.openlocfilehash: ff0476f72c7da088bd2b39f58ab560dcc82197e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530990"
---
# <a name="folderids"></a><span data-ttu-id="8937a-103">FolderIds</span><span class="sxs-lookup"><span data-stu-id="8937a-103">FolderIds</span></span>

<span data-ttu-id="8937a-104">O elemento **FolderIds** contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem copiadas, movidas, obtidas, excluídas ou monitoradas para notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="8937a-104">The **FolderIds** element contains an array of folder identifiers that are used to identify folders to copy, move, get, delete, or monitor for event notifications.</span></span> 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 <span data-ttu-id="8937a-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="8937a-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8937a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8937a-106">Attributes and elements</span></span>

<span data-ttu-id="8937a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8937a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8937a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8937a-108">Attributes</span></span>

<span data-ttu-id="8937a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8937a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8937a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8937a-110">Child elements</span></span>

|<span data-ttu-id="8937a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8937a-111">**Element**</span></span>|<span data-ttu-id="8937a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8937a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8937a-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="8937a-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8937a-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8937a-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="8937a-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8937a-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="8937a-116">Identifica as pastas do Microsoft Exchange Server que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="8937a-116">Identifies Microsoft Exchange Server folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8937a-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8937a-117">Parent elements</span></span>

|<span data-ttu-id="8937a-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8937a-118">**Element**</span></span>|<span data-ttu-id="8937a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8937a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8937a-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-120">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="8937a-121">Define uma solicitação para obter uma pasta do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8937a-121">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="8937a-122">A seguir está a expressão XPath para este elemento:`/GetFolder`</span><span class="sxs-lookup"><span data-stu-id="8937a-122">The following is the XPath expression to this element:  `/GetFolder`</span></span> <br/> |
|[<span data-ttu-id="8937a-123">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-123">DeleteFolder</span></span>](deletefolder.md) <br/> |<span data-ttu-id="8937a-124">Define uma solicitação para excluir pastas do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8937a-124">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="8937a-125">A seguir está a expressão XPath para este elemento:`/DeleteFolder`</span><span class="sxs-lookup"><span data-stu-id="8937a-125">The following is the XPath expression to this element:  `/DeleteFolder`</span></span> <br/> |
|[<span data-ttu-id="8937a-126">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-126">EmptyFolder</span></span>](emptyfolder.md) <br/> |<span data-ttu-id="8937a-127">Define uma solicitação para excluir pastas do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8937a-127">Defines a request to delete folders from the Exchange store.</span></span>  <br/> <span data-ttu-id="8937a-128">A seguir está a expressão XPath para este elemento:`/EmptyFolder`</span><span class="sxs-lookup"><span data-stu-id="8937a-128">The following is the XPath expression to this element:  `/EmptyFolder`</span></span> <br/> |
|[<span data-ttu-id="8937a-129">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-129">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="8937a-130">Define uma solicitação para mover uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8937a-130">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="8937a-131">A seguir está a expressão XPath para este elemento:`/MoveFolder`</span><span class="sxs-lookup"><span data-stu-id="8937a-131">The following is the XPath expression to this element:  `/MoveFolder`</span></span> <br/> |
|[<span data-ttu-id="8937a-132">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-132">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="8937a-133">Define uma solicitação para copiar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8937a-133">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="8937a-134">A seguir está a expressão XPath para este elemento:`/CopyFolder`</span><span class="sxs-lookup"><span data-stu-id="8937a-134">The following is the XPath expression to this element:  `/CopyFolder`</span></span> <br/> |
|[<span data-ttu-id="8937a-135">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8937a-135">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="8937a-136">Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.</span><span class="sxs-lookup"><span data-stu-id="8937a-136">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="8937a-137">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8937a-137">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="8937a-138">Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.</span><span class="sxs-lookup"><span data-stu-id="8937a-138">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8937a-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="8937a-139">Remarks</span></span>

<span data-ttu-id="8937a-140">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8937a-140">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8937a-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8937a-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8937a-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="8937a-142">Namespace</span></span>  <br/> |<span data-ttu-id="8937a-143">https://schemas.microsoft.com/exchange/services/2006/messages e https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="8937a-143">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="8937a-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8937a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="8937a-145">Esquema de mensagens; Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8937a-145">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="8937a-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8937a-146">Validation File</span></span>  <br/> |<span data-ttu-id="8937a-147">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8937a-147">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8937a-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8937a-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="8937a-149">False</span><span class="sxs-lookup"><span data-stu-id="8937a-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8937a-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="8937a-150">See also</span></span>



[<span data-ttu-id="8937a-151">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-151">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="8937a-152">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-152">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="8937a-153">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-153">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="8937a-154">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="8937a-154">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="8937a-155">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="8937a-155">Subscribe operation</span></span>](subscribe-operation.md)

