---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: O elemento EmptyFolder define uma solicitação para esvaziar uma pasta em uma caixa de correio no repositório do Exchange. Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457274"
---
# <a name="emptyfolder"></a><span data-ttu-id="e6854-104">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="e6854-104">EmptyFolder</span></span>

<span data-ttu-id="e6854-105">O elemento **EmptyFolder** define uma solicitação para esvaziar uma pasta em uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6854-105">The **EmptyFolder** element defines a request to empty a folder in a mailbox in the Exchange store.</span></span> <span data-ttu-id="e6854-106">Opcionalmente, as subpastas também podem ser excluídas quando a pasta é esvaziada.</span><span class="sxs-lookup"><span data-stu-id="e6854-106">Optionally, subfolders can also be deleted when the folder is emptied.</span></span> 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 <span data-ttu-id="e6854-107">**EmptyFolderType**</span><span class="sxs-lookup"><span data-stu-id="e6854-107">**EmptyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6854-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e6854-108">Attributes and elements</span></span>

<span data-ttu-id="e6854-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e6854-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6854-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e6854-110">Attributes</span></span>

|<span data-ttu-id="e6854-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e6854-111">**Attribute**</span></span>|<span data-ttu-id="e6854-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6854-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e6854-113">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="e6854-113">**DeleteType**</span></span> <br/> |<span data-ttu-id="e6854-114">Especifica como uma pasta é esvaziada.</span><span class="sxs-lookup"><span data-stu-id="e6854-114">Specifies how a folder is emptied.</span></span> <span data-ttu-id="e6854-115">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e6854-115">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e6854-116">**DeleteSubFolders**</span><span class="sxs-lookup"><span data-stu-id="e6854-116">**DeleteSubFolders**</span></span> <br/> |<span data-ttu-id="e6854-117">Especifica se as subpastas devem ser excluídas.</span><span class="sxs-lookup"><span data-stu-id="e6854-117">Specifies whether subfolders are to be deleted.</span></span> <span data-ttu-id="e6854-118">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e6854-118">This attribute is required.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="e6854-119">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="e6854-119">DeleteType Attribute</span></span>

|<span data-ttu-id="e6854-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e6854-120">**Value**</span></span>|<span data-ttu-id="e6854-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6854-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e6854-122">HardDelete</span><span class="sxs-lookup"><span data-stu-id="e6854-122">HardDelete</span></span>  <br/> |<span data-ttu-id="e6854-123">As mensagens e pastas são removidas permanentemente da loja.</span><span class="sxs-lookup"><span data-stu-id="e6854-123">A messages and folders are permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="e6854-124">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="e6854-124">SoftDelete</span></span>  <br/> |<span data-ttu-id="e6854-125">As mensagens e pastas serão movidas para o dumpster se o dumpster estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="e6854-125">A messages and folders are moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="e6854-126">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="e6854-126">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="e6854-127">As mensagens e pastas são movidas para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e6854-127">A messages and folders are moved to the Deleted Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e6854-128">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e6854-128">Child elements</span></span>

|<span data-ttu-id="e6854-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e6854-129">**Element**</span></span>|<span data-ttu-id="e6854-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6854-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6854-131">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e6854-131">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="e6854-132">Contém uma matriz de identificadores de pasta que são usados para identificar pastas a serem excluídas.</span><span class="sxs-lookup"><span data-stu-id="e6854-132">Contains an array of folder identifiers that are used to identify folders to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6854-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e6854-133">Parent elements</span></span>

<span data-ttu-id="e6854-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6854-134">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e6854-135">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e6854-135">Text value</span></span>

<span data-ttu-id="e6854-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6854-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e6854-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="e6854-137">Remarks</span></span>

<span data-ttu-id="e6854-138">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6854-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6854-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e6854-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6854-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="e6854-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e6854-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e6854-141">Schema Name</span></span>  <br/> |<span data-ttu-id="e6854-142">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e6854-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="e6854-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e6854-143">Validation File</span></span>  <br/> |<span data-ttu-id="e6854-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e6854-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6854-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e6854-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6854-146">False</span><span class="sxs-lookup"><span data-stu-id="e6854-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6854-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="e6854-147">See also</span></span>



[<span data-ttu-id="e6854-148">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="e6854-148">EmptyFolder operation</span></span>](emptyfolder-operation.md)

