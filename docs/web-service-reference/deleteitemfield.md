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
description: O elemento DeleteItemField representa uma operação para excluir uma determinada propriedade de um item durante uma chamada de UpdateItem.
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751754"
---
# <a name="deleteitemfield"></a><span data-ttu-id="ed722-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ed722-103">DeleteItemField</span></span>

<span data-ttu-id="ed722-104">O elemento **DeleteItemField** representa uma operação para excluir uma determinada propriedade de um item durante uma chamada de UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="ed722-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="ed722-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ed722-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="ed722-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ed722-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="ed722-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ed722-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="ed722-108">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="ed722-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="ed722-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ed722-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 <span data-ttu-id="ed722-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="ed722-110">**DeleteItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed722-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ed722-111">Attributes and elements</span></span>

<span data-ttu-id="ed722-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed722-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed722-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed722-113">Attributes</span></span>

<span data-ttu-id="ed722-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed722-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed722-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed722-115">Child elements</span></span>

|<span data-ttu-id="ed722-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed722-116">**Element**</span></span>|<span data-ttu-id="ed722-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed722-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed722-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ed722-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ed722-119">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="ed722-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ed722-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ed722-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ed722-121">Identifica a membros individuais de uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="ed722-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="ed722-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ed722-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ed722-123">Identifica as propriedades estendidas de MAPI.</span><span class="sxs-lookup"><span data-stu-id="ed722-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed722-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed722-124">Parent elements</span></span>

|<span data-ttu-id="ed722-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed722-125">**Element**</span></span>|<span data-ttu-id="ed722-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed722-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed722-127">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="ed722-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="ed722-128">Contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="ed722-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="ed722-129">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ed722-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ed722-130">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ed722-130">Remarks</span></span>

<span data-ttu-id="ed722-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ed722-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed722-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ed722-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed722-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed722-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed722-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed722-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ed722-135">esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ed722-135">types schema</span></span>  <br/> |
|<span data-ttu-id="ed722-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed722-136">Validation File</span></span>  <br/> |<span data-ttu-id="ed722-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed722-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed722-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ed722-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed722-139">False</span><span class="sxs-lookup"><span data-stu-id="ed722-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed722-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="ed722-140">See also</span></span>

- [<span data-ttu-id="ed722-141">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ed722-141">UpdateItem operation</span></span>](updateitem-operation.md)

