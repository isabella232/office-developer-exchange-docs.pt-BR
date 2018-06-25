---
title: Item (UploadItemType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ab7058f2-615f-4393-a0d4-af76727f37e9
description: O elemento de Item representa um único item para carregar em uma caixa de correio.
ms.openlocfilehash: 8fecef9a2368a44e38633eb9fddaa8197620f6a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824138"
---
# <a name="item-uploaditemtype"></a><span data-ttu-id="5f7e6-103">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="5f7e6-103">Item (UploadItemType)</span></span>

<span data-ttu-id="5f7e6-104">O elemento de **Item** representa um único item para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-104">The **Item** element represents a single item to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="5f7e6-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="5f7e6-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="5f7e6-106">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="5f7e6-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
[<span data-ttu-id="5f7e6-107">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="5f7e6-107">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
  
```XML
<Item CreateAction="" IsAssociated="">
   <ParentFolderId/>
   <ItemId/>
   <Data/>
</Item>
```

 <span data-ttu-id="5f7e6-108">**UploadItemType**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-108">**UploadItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f7e6-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5f7e6-109">Attributes and elements</span></span>

<span data-ttu-id="5f7e6-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f7e6-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="5f7e6-111">Attributes</span></span>

|<span data-ttu-id="5f7e6-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-112">**Attribute**</span></span>|<span data-ttu-id="5f7e6-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5f7e6-114">**CreateAction**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-114">**CreateAction**</span></span> <br/> |<span data-ttu-id="5f7e6-115">Especifica a ação para carregar um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-115">Specifies the action for uploading an item into a mailbox.</span></span> <span data-ttu-id="5f7e6-116">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="5f7e6-117">**IsAssociated**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-117">**IsAssociated**</span></span> <br/> |<span data-ttu-id="5f7e6-118">Especifica se o item carregado é um item de pasta associada.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-118">Specifies whether the uploaded item is a folder associated item.</span></span> <span data-ttu-id="5f7e6-119">Este atributo é um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-119">This attribute is a Boolean value.</span></span> <span data-ttu-id="5f7e6-120">Um valor **true** indica que o item é uma pasta associada item.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-120">A value of **true** indicates that the item is a folder associated item.</span></span> <span data-ttu-id="5f7e6-121">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-121">This attribute is optional.</span></span>  <br/> |
   
#### <a name="createaction-attribute"></a><span data-ttu-id="5f7e6-122">Atributo CreateAction</span><span class="sxs-lookup"><span data-stu-id="5f7e6-122">CreateAction Attribute</span></span>

|<span data-ttu-id="5f7e6-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-123">**Value**</span></span>|<span data-ttu-id="5f7e6-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5f7e6-125">**CreateNew**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-125">**CreateNew**</span></span> <br/> |<span data-ttu-id="5f7e6-126">Indica que uma nova cópia do item original é carregada na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-126">Indicates that a new copy of the original item is uploaded to the mailbox.</span></span> <span data-ttu-id="5f7e6-127">O elemento [ItemId](itemid.md) não deve estar presente se o valor CreateNew é usado.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-127">The [ItemId](itemid.md) element must not be present if the CreateNew value is used.</span></span> <span data-ttu-id="5f7e6-128">O novo item identificador é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-128">The new item identifier is returned in the response.</span></span>  <br/> |
|<span data-ttu-id="5f7e6-129">**Update**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-129">**Update**</span></span> <br/> |<span data-ttu-id="5f7e6-130">Especifica que o item indicado pelo elemento **ItemId** será atualizado.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-130">Specifies that the item indicated by the **ItemId** element will be updated.</span></span> <span data-ttu-id="5f7e6-131">Um erro será retornado se o elemento **ItemId** não estiver presente ou se o item não existir na pasta identificada pelo elemento [ParentFolderId](parentfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="5f7e6-131">An error is returned if the **ItemId** element is not present or if the item does not exist in the folder identified by the [ParentFolderId](parentfolderid.md) element.</span></span>  <br/> |
|<span data-ttu-id="5f7e6-132">**UpdateOrCreate**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-132">**UpdateOrCreate**</span></span> <br/> |<span data-ttu-id="5f7e6-133">Indica o primeiro é feita uma tentativa de atualizar o item.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-133">Indicates that an attempt is first made to update the item.</span></span> <span data-ttu-id="5f7e6-134">Se o item não existir na pasta especificada pelo elemento **ParentFolderId** , um novo item for criado.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-134">If the item does not exist in the folder specified by the **ParentFolderId** element, a new item is created.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5f7e6-135">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5f7e6-135">Child elements</span></span>

|<span data-ttu-id="5f7e6-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-136">**Element**</span></span>|<span data-ttu-id="5f7e6-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f7e6-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5f7e6-138">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5f7e6-139">Representa o identificador da pasta pai onde um novo item for criado ou que contém o item a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-139">Represents the identifier of the parent folder where a new item is created or that contains the item to update.</span></span>  <br/> |
|[<span data-ttu-id="5f7e6-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="5f7e6-140">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5f7e6-141">Contém o identificador e alterar a chave exclusiva de um item para criar ou atualizar no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-141">Contains the unique identifier and change key of an item to create or update in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5f7e6-142">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="5f7e6-142">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="5f7e6-143">Contém os dados de um único item para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-143">Contains the data of a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5f7e6-144">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5f7e6-144">Parent elements</span></span>

|<span data-ttu-id="5f7e6-145">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-145">**Element**</span></span>|<span data-ttu-id="5f7e6-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f7e6-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f7e6-147">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="5f7e6-147">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="5f7e6-148">Contém uma matriz de item para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-148">Contains an array of item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f7e6-149">Text value</span><span class="sxs-lookup"><span data-stu-id="5f7e6-149">Text value</span></span>

<span data-ttu-id="5f7e6-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5f7e6-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f7e6-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="5f7e6-151">Remarks</span></span>

<span data-ttu-id="5f7e6-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5f7e6-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f7e6-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5f7e6-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f7e6-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="5f7e6-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f7e6-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5f7e6-155">Schema Name</span></span>  <br/> |<span data-ttu-id="5f7e6-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5f7e6-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f7e6-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5f7e6-157">Validation File</span></span>  <br/> |<span data-ttu-id="5f7e6-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5f7e6-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f7e6-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5f7e6-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="5f7e6-160">False</span><span class="sxs-lookup"><span data-stu-id="5f7e6-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f7e6-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="5f7e6-161">See also</span></span>



[<span data-ttu-id="5f7e6-162">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="5f7e6-162">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="5f7e6-163">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="5f7e6-163">UploadItems operation</span></span>](uploaditems-operation.md)

