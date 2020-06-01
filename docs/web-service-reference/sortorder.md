---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: O elemento SortOrder define como os itens são classificados em uma solicitação FindItem ou FindConversation.
ms.openlocfilehash: b520bb3ca6daadc777e7235b2b7420a12e425048
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468366"
---
# <a name="sortorder"></a><span data-ttu-id="4face-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="4face-103">SortOrder</span></span>

<span data-ttu-id="4face-104">O elemento **SortOrder** define como os itens são classificados em uma solicitação **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="4face-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="4face-105">**NonEmptyArrayOfFieldOrdersType**</span><span class="sxs-lookup"><span data-stu-id="4face-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4face-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4face-106">Attributes and elements</span></span>

<span data-ttu-id="4face-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4face-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4face-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4face-108">Attributes</span></span>

<span data-ttu-id="4face-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4face-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4face-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4face-110">Child elements</span></span>

|<span data-ttu-id="4face-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4face-111">**Element**</span></span>|<span data-ttu-id="4face-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4face-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4face-113">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="4face-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="4face-114">Representa um único campo pelo qual classificar os resultados e indica a direção da classificação.</span><span class="sxs-lookup"><span data-stu-id="4face-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="4face-115">Um ou mais desses elementos podem ser incluídos.</span><span class="sxs-lookup"><span data-stu-id="4face-115">One or more of these elements may be included.</span></span> <span data-ttu-id="4face-116">Os elementos [FieldOrder](fieldorder.md) são aplicados na ordem especificada para classificação.</span><span class="sxs-lookup"><span data-stu-id="4face-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4face-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4face-117">Parent elements</span></span>

|<span data-ttu-id="4face-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4face-118">**Element**</span></span>|<span data-ttu-id="4face-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4face-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4face-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="4face-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="4face-121">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4face-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="4face-122">A seguir está a expressão XPath para este elemento:`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="4face-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="4face-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="4face-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="4face-124">Define uma solicitação para encontrar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4face-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4face-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4face-125">Text value</span></span>

<span data-ttu-id="4face-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4face-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4face-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="4face-127">Remarks</span></span>

<span data-ttu-id="4face-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4face-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4face-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4face-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4face-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="4face-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4face-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4face-131">Schema Name</span></span>  <br/> |<span data-ttu-id="4face-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4face-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4face-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4face-133">Validation File</span></span>  <br/> |<span data-ttu-id="4face-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4face-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4face-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4face-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="4face-136">False</span><span class="sxs-lookup"><span data-stu-id="4face-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4face-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="4face-137">See also</span></span>



[<span data-ttu-id="4face-138">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="4face-138">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="4face-139">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="4face-139">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="4face-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4face-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

