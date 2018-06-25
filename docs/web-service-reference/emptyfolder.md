---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: O elemento de EmptyFolder define uma solicitação para esvaziar a uma pasta em uma caixa de correio no armazenamento do Exchange. Opcionalmente, subpastas também podem ser excluídas quando a pasta será esvaziada.
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752037"
---
# <a name="emptyfolder"></a><span data-ttu-id="33621-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="33621-104">EmptyFolder</span></span>

<span data-ttu-id="33621-105">O elemento de **EmptyFolder** define uma solicitação para esvaziar a uma pasta em uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33621-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="33621-106">Opcionalmente, subpastas também podem ser excluídas quando a pasta será esvaziada.</span><span class="sxs-lookup"><span data-stu-id="33621-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="33621-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="33621-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33621-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="33621-108">Attributes and elements</span></span>

<span data-ttu-id="33621-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="33621-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33621-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="33621-110">Attributes</span></span>

|<span data-ttu-id="33621-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="33621-111">**Attribute**</span></span>|<span data-ttu-id="33621-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33621-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33621-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="33621-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="33621-114">Especifica como uma pasta é esvaziada.</span><span class="sxs-lookup"><span data-stu-id="33621-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="33621-115">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="33621-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="33621-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="33621-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="33621-117">Especifica se as subpastas estão a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="33621-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="33621-118">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="33621-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="33621-119">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="33621-119">DeleteType Attribute</span></span>

|<span data-ttu-id="33621-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="33621-120">**Value**</span></span>|<span data-ttu-id="33621-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33621-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="33621-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="33621-122">HardDelete</span></span>  <br/> |<span data-ttu-id="33621-123">Uma mensagens e pastas são removidas permanentemente do repositório.</span><span class="sxs-lookup"><span data-stu-id="33621-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="33621-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="33621-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="33621-125">Uma mensagens e pastas são movidas para o dumpster se o dumpster está habilitado.</span><span class="sxs-lookup"><span data-stu-id="33621-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="33621-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="33621-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="33621-127">Uma mensagens e pastas são movidas para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="33621-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="33621-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="33621-128">Child elements</span></span>

|<span data-ttu-id="33621-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="33621-129">**Element**</span></span>|<span data-ttu-id="33621-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33621-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33621-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="33621-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="33621-132">Contém uma matriz de identificadores de pasta que são usados para identificar pastas para excluir.</span><span class="sxs-lookup"><span data-stu-id="33621-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33621-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="33621-133">Parent elements</span></span>

<span data-ttu-id="33621-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="33621-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="33621-135">Text value</span><span class="sxs-lookup"><span data-stu-id="33621-135">Text value</span></span>

<span data-ttu-id="33621-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="33621-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33621-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="33621-137">Remarks</span></span>

<span data-ttu-id="33621-138">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33621-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33621-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="33621-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33621-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="33621-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33621-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="33621-141">Schema Name</span></span>  <br/> |<span data-ttu-id="33621-142">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="33621-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="33621-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="33621-143">Validation File</span></span>  <br/> |<span data-ttu-id="33621-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33621-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33621-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="33621-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="33621-146">False</span><span class="sxs-lookup"><span data-stu-id="33621-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33621-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="33621-147">See also</span></span>



[<span data-ttu-id="33621-148">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="33621-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

