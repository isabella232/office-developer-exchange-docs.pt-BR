---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: O elemento DeleteItemField representa uma operação para excluir uma determinada propriedade de um item durante uma chamada UpdateItem.
ms.openlocfilehash: e6f5ee8a1130d7c040f3ddd94021eff6d4a758b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455671"
---
# <a name="deleteitemfield"></a><span data-ttu-id="a2971-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="a2971-103">DeleteItemField</span></span>

<span data-ttu-id="a2971-104">O elemento **DeleteItemField** representa uma operação para excluir uma determinada propriedade de um item durante uma chamada UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="a2971-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="a2971-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a2971-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="a2971-106">Alterações</span><span class="sxs-lookup"><span data-stu-id="a2971-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="a2971-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a2971-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="a2971-108">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="a2971-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="a2971-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="a2971-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

```xml
<DeleteItemField>
   <IndexedFieldURI/> 
</DeleteItemField>
```

```xml
<DeleteItemField>
   <ExtendedFieldURI/>
</DeleteItemField>
```

<span data-ttu-id="a2971-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="a2971-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a2971-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a2971-111">Attributes and elements</span></span>

<span data-ttu-id="a2971-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a2971-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2971-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="a2971-113">Attributes</span></span>

<span data-ttu-id="a2971-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2971-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2971-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2971-115">Child elements</span></span>

|<span data-ttu-id="a2971-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2971-116">**Element**</span></span>|<span data-ttu-id="a2971-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2971-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2971-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="a2971-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="a2971-119">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="a2971-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="a2971-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a2971-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="a2971-121">Identifica membros individuais de uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="a2971-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="a2971-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a2971-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="a2971-123">Identifica as propriedades de MAPI estendidas.</span><span class="sxs-lookup"><span data-stu-id="a2971-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2971-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a2971-124">Parent elements</span></span>

|<span data-ttu-id="a2971-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2971-125">**Element**</span></span>|<span data-ttu-id="a2971-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2971-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2971-127">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="a2971-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="a2971-128">Contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="a2971-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="a2971-129">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a2971-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2971-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2971-130">Remarks</span></span>

<span data-ttu-id="a2971-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a2971-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2971-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a2971-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2971-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2971-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2971-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a2971-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a2971-135">esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a2971-135">types schema</span></span>  <br/> |
|<span data-ttu-id="a2971-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a2971-136">Validation File</span></span>  <br/> |<span data-ttu-id="a2971-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2971-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2971-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a2971-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2971-139">False</span><span class="sxs-lookup"><span data-stu-id="a2971-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2971-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2971-140">See also</span></span>

- [<span data-ttu-id="a2971-141">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a2971-141">UpdateItem operation</span></span>](updateitem-operation.md)

