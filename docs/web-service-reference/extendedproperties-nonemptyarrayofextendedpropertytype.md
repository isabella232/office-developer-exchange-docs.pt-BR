---
title: ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: O elemento ExtendedProperties Especifica uma matriz de propriedades adicionais.
ms.openlocfilehash: b92108ecde63d4a3ac3cc80861c204c4d1950cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752180"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a><span data-ttu-id="6ef21-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="6ef21-103">ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)</span></span>

<span data-ttu-id="6ef21-104">O elemento **ExtendedProperties** Especifica uma matriz de propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="6ef21-104">The **ExtendedProperties** element specifies an array of additional properties.</span></span> 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 <span data-ttu-id="6ef21-105">**NonEmptyArrayOfExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="6ef21-105">**NonEmptyArrayOfExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ef21-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6ef21-106">Attributes and elements</span></span>

<span data-ttu-id="6ef21-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ef21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ef21-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ef21-108">Attributes</span></span>

<span data-ttu-id="6ef21-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ef21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ef21-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ef21-110">Child elements</span></span>

|<span data-ttu-id="6ef21-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ef21-111">**Element**</span></span>|<span data-ttu-id="6ef21-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ef21-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ef21-113">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6ef21-113">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6ef21-114">Identifica as propriedades estendidas de MAPI em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="6ef21-114">Identifies extended MAPI properties on folders and items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ef21-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ef21-115">Parent elements</span></span>

|<span data-ttu-id="6ef21-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ef21-116">**Element**</span></span>|<span data-ttu-id="6ef21-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ef21-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ef21-118">ImGroup</span><span class="sxs-lookup"><span data-stu-id="6ef21-118">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="6ef21-119">Representa um grupo de mensagens instantâneo.</span><span class="sxs-lookup"><span data-stu-id="6ef21-119">Represents an instant messaging group.</span></span>  <br/> |
|[<span data-ttu-id="6ef21-120">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="6ef21-120">SearchPreviewItem</span></span>](searchpreviewitem.md) <br/> |<span data-ttu-id="6ef21-121">Especifica os primeiros 256 caracteres de um item de caixa de correio para visualização sem abrir o item.</span><span class="sxs-lookup"><span data-stu-id="6ef21-121">Specifies the first 256 characters of a mailbox item for preview without opening the item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6ef21-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ef21-122">Remarks</span></span>

<span data-ttu-id="6ef21-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6ef21-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6ef21-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ef21-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ef21-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6ef21-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ef21-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ef21-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ef21-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ef21-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6ef21-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="6ef21-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="6ef21-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ef21-129">Validation File</span></span>  <br/> |<span data-ttu-id="6ef21-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6ef21-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ef21-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6ef21-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6ef21-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ef21-132">See also</span></span>



- [<span data-ttu-id="6ef21-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6ef21-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

