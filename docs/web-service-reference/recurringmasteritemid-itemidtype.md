---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: O elemento RecurringMasterItemId (ItemIdType) identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825010"
---
# <a name="recurringmasteritemid-itemidtype"></a><span data-ttu-id="6a5ed-103">RecurringMasterItemId (ItemIdType)</span><span class="sxs-lookup"><span data-stu-id="6a5ed-103">RecurringMasterItemId (ItemIdType)</span></span>

<span data-ttu-id="6a5ed-104">O elemento **RecurringMasterItemId (ItemIdType)** identifica um item-mestre recorrência identificando os identificadores de um dos seus itens relacionados ocorrência.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-104">The **RecurringMasterItemId (ItemIdType)** element identifies a recurrence master item by identifying the identifiers of one of its related occurrence items.</span></span> 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="6a5ed-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="6a5ed-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a5ed-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6a5ed-106">Attributes and elements</span></span>

<span data-ttu-id="6a5ed-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a5ed-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6a5ed-108">Attributes</span></span>

****

|<span data-ttu-id="6a5ed-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="6a5ed-109">**Attribute**</span></span>|<span data-ttu-id="6a5ed-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a5ed-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6a5ed-111">Id</span><span class="sxs-lookup"><span data-stu-id="6a5ed-111">Id</span></span>  <br/> |<span data-ttu-id="6a5ed-112">Identifica uma única ocorrência de um item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-112">Identifies a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6a5ed-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6a5ed-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6a5ed-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6a5ed-115">Identifica uma versão específica de uma única ocorrência de um item mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-115">Identifies a specific version of a single occurrence of a recurring master item.</span></span> <span data-ttu-id="6a5ed-116">Além disso, o item mestre recorrente também é identificado porque ele e a ocorrência única irá conter a mesma chave de alteração.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-116">Additionally, the recurring master item is also identified because it and the single occurrence will contain the same change key.</span></span> <span data-ttu-id="6a5ed-117">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-117">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6a5ed-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6a5ed-118">Child elements</span></span>

<span data-ttu-id="6a5ed-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a5ed-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6a5ed-120">Parent elements</span></span>

[<span data-ttu-id="6a5ed-121">Lembrete</span><span class="sxs-lookup"><span data-stu-id="6a5ed-121">Reminder</span></span>](reminder.md)
  
## <a name="remarks"></a><span data-ttu-id="6a5ed-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6a5ed-122">Remarks</span></span>

<span data-ttu-id="6a5ed-123">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6a5ed-123">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6a5ed-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a5ed-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a5ed-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6a5ed-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a5ed-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a5ed-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a5ed-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6a5ed-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6a5ed-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6a5ed-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a5ed-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6a5ed-129">Validation File</span></span>  <br/> |<span data-ttu-id="6a5ed-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a5ed-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a5ed-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6a5ed-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a5ed-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6a5ed-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a5ed-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="6a5ed-133">See also</span></span>



[<span data-ttu-id="6a5ed-134">Lembrete</span><span class="sxs-lookup"><span data-stu-id="6a5ed-134">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="6a5ed-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6a5ed-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

