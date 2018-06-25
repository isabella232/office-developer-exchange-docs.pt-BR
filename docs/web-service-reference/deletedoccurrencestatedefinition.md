---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: O DeletedOccurrenceStateDefinition Especifica o estado de uma ocorrência excluído de um item de calendário.
ms.openlocfilehash: ad0434d604ee78ebf1905b60857929e1af4d45f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751738"
---
# <a name="deletedoccurrencestatedefinition"></a><span data-ttu-id="543cf-103">DeletedOccurrenceStateDefinition</span><span class="sxs-lookup"><span data-stu-id="543cf-103">DeletedOccurrenceStateDefinition</span></span>

<span data-ttu-id="543cf-104">O **DeletedOccurrenceStateDefinition** Especifica o estado de uma ocorrência excluído de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="543cf-104">The **DeletedOccurrenceStateDefinition** specifies the state for a deleted occurrence of a calendar item.</span></span> 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 <span data-ttu-id="543cf-105">**DeletedOccurrenceStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="543cf-105">**DeletedOccurrenceStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="543cf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="543cf-106">Attributes and elements</span></span>

<span data-ttu-id="543cf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="543cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="543cf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="543cf-108">Attributes</span></span>

<span data-ttu-id="543cf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="543cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="543cf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="543cf-110">Child elements</span></span>

|<span data-ttu-id="543cf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="543cf-111">**Element**</span></span>|<span data-ttu-id="543cf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="543cf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="543cf-113">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="543cf-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="543cf-114">Especifica a data da ocorrência de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="543cf-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="543cf-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="543cf-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="543cf-116">Especifica um valor Boolean que indica se uma ocorrência de um item do calendário está presente.</span><span class="sxs-lookup"><span data-stu-id="543cf-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="543cf-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="543cf-117">Parent elements</span></span>

|<span data-ttu-id="543cf-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="543cf-118">**Element**</span></span>|<span data-ttu-id="543cf-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="543cf-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="543cf-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="543cf-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="543cf-121">Especifica uma definição de estado.</span><span class="sxs-lookup"><span data-stu-id="543cf-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="543cf-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="543cf-122">Remarks</span></span>

<span data-ttu-id="543cf-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="543cf-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="543cf-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="543cf-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="543cf-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="543cf-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="543cf-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="543cf-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="543cf-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="543cf-127">Schema Name</span></span>  <br/> |<span data-ttu-id="543cf-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="543cf-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="543cf-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="543cf-129">Validation File</span></span>  <br/> |<span data-ttu-id="543cf-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="543cf-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="543cf-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="543cf-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="543cf-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="543cf-132">See also</span></span>

- [<span data-ttu-id="543cf-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="543cf-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

