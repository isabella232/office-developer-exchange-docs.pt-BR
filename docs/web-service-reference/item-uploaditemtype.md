---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: O elemento item representa um único item a ser carregado em uma caixa de correio.
ms.openlocfilehash: 82c0fdf89c06ddfb812c2b2f1899b589eedeb7d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467547"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="e4c32-103">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="e4c32-103">Item (UploadItemType)</span></span>

<span data-ttu-id="e4c32-104">O elemento **Item** representa um único item a ser carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e4c32-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="e4c32-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="e4c32-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="e4c32-106">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="e4c32-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="e4c32-107">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="e4c32-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="e4c32-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="e4c32-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4c32-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e4c32-109">Attributes and elements</span></span>

<span data-ttu-id="e4c32-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e4c32-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4c32-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="e4c32-111">Attributes</span></span>

|<span data-ttu-id="e4c32-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e4c32-112">**Attribute**</span></span>|<span data-ttu-id="e4c32-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e4c32-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4c32-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="e4c32-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="e4c32-115">Especifica a ação para carregar um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e4c32-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="e4c32-116">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e4c32-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e4c32-117">**Isassociated**</span><span class="sxs-lookup"><span data-stu-id="e4c32-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="e4c32-118">Especifica se o item carregado é um item associado à pasta.</span><span class="sxs-lookup"><span data-stu-id="e4c32-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="e4c32-119">Este atributo é um valor booliano.</span><span class="sxs-lookup"><span data-stu-id="e4c32-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="e4c32-120">Um valor **true** indica que o item é um item associado à pasta.</span><span class="sxs-lookup"><span data-stu-id="e4c32-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="e4c32-121">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e4c32-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="e4c32-122">Atributo CreateAction</span><span class="sxs-lookup"><span data-stu-id="e4c32-122">CreateAction Attribute</span></span>

|<span data-ttu-id="e4c32-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e4c32-123">**Value**</span></span>|<span data-ttu-id="e4c32-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e4c32-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4c32-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="e4c32-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="e4c32-126">Indica que uma nova cópia do item original é carregada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e4c32-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="e4c32-127">O elemento [ItemId](itemid.md) não deve estar presente se o valor de CreateNew for usado.</span><span class="sxs-lookup"><span data-stu-id="e4c32-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="e4c32-128">O novo identificador de item é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4c32-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="e4c32-129">**Atualização**</span><span class="sxs-lookup"><span data-stu-id="e4c32-129">**Update**</span></span> <br/> |<span data-ttu-id="e4c32-130">Especifica que o item indicado pelo elemento **ItemId** será atualizado.</span><span class="sxs-lookup"><span data-stu-id="e4c32-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="e4c32-131">Um erro será retornado se o elemento **ItemId** não estiver presente ou se o item não existir na pasta identificada pelo elemento [ParentFolderId](parentfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4c32-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="e4c32-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="e4c32-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="e4c32-133">Indica que uma tentativa é feita pela primeira vez para atualizar o item.</span><span class="sxs-lookup"><span data-stu-id="e4c32-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="e4c32-134">Se o item não existir na pasta especificada pelo elemento **ParentFolderId** , um novo item é criado.</span><span class="sxs-lookup"><span data-stu-id="e4c32-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e4c32-135">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e4c32-135">Child elements</span></span>

|<span data-ttu-id="e4c32-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e4c32-136">**Element**</span></span>|<span data-ttu-id="e4c32-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e4c32-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c32-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e4c32-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e4c32-139">Representa o identificador da pasta pai onde um novo item é criado ou que contém o item a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="e4c32-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="e4c32-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="e4c32-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="e4c32-141">Contém o identificador exclusivo e a chave de alteração de um item a ser criado ou atualizado no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4c32-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e4c32-142">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="e4c32-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="e4c32-143">Contém os dados de um único item a ser carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e4c32-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e4c32-144">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e4c32-144">Parent elements</span></span>

|<span data-ttu-id="e4c32-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e4c32-145">**Element**</span></span>|<span data-ttu-id="e4c32-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e4c32-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c32-147">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="e4c32-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="e4c32-148">Contém uma matriz de itens para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e4c32-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4c32-149">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e4c32-149">Text value</span></span>

<span data-ttu-id="e4c32-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e4c32-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4c32-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="e4c32-151">Remarks</span></span>

<span data-ttu-id="e4c32-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e4c32-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4c32-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e4c32-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4c32-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4c32-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4c32-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e4c32-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e4c32-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e4c32-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4c32-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e4c32-157">Validation File</span></span>  <br/> |<span data-ttu-id="e4c32-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e4c32-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4c32-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e4c32-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4c32-160">False</span><span class="sxs-lookup"><span data-stu-id="e4c32-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4c32-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="e4c32-161">See also</span></span>



[<span data-ttu-id="e4c32-162">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="e4c32-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="e4c32-163">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="e4c32-163">UploadItems operation</span></span>](uploaditems-operation.md)

