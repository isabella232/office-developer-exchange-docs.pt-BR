---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: O elemento DeleteFromFolderStateDefinition Especifica o estado quando um item é excluído de uma pasta.
ms.openlocfilehash: 7b6374b9fa55d3b08569e8ac9e247dd6e5bebc24
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751749"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="044a8-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="044a8-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="044a8-104">O elemento **DeleteFromFolderStateDefinition** Especifica o estado quando um item é excluído de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="044a8-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="044a8-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="044a8-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="044a8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="044a8-106">Attributes and elements</span></span>

<span data-ttu-id="044a8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="044a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="044a8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="044a8-108">Attributes</span></span>

<span data-ttu-id="044a8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="044a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="044a8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="044a8-110">Child elements</span></span>

|<span data-ttu-id="044a8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="044a8-111">**Element**</span></span>|<span data-ttu-id="044a8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="044a8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="044a8-113">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="044a8-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="044a8-114">Especifica a data da ocorrência de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="044a8-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="044a8-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="044a8-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="044a8-116">Especifica um valor Boolean que indica se uma ocorrência de um item do calendário está presente.</span><span class="sxs-lookup"><span data-stu-id="044a8-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="044a8-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="044a8-117">Parent elements</span></span>

|<span data-ttu-id="044a8-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="044a8-118">**Element**</span></span>|<span data-ttu-id="044a8-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="044a8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="044a8-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="044a8-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="044a8-121">Especifica uma definição de estado.</span><span class="sxs-lookup"><span data-stu-id="044a8-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="044a8-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="044a8-122">Remarks</span></span>

<span data-ttu-id="044a8-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="044a8-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="044a8-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="044a8-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="044a8-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="044a8-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="044a8-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="044a8-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="044a8-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="044a8-127">Schema Name</span></span>  <br/> |<span data-ttu-id="044a8-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="044a8-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="044a8-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="044a8-129">Validation File</span></span>  <br/> |<span data-ttu-id="044a8-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="044a8-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="044a8-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="044a8-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="044a8-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="044a8-132">See also</span></span>

- [<span data-ttu-id="044a8-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="044a8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

