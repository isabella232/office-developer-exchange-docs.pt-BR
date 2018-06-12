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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751749"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="e72db-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="e72db-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="e72db-104">O elemento **DeleteFromFolderStateDefinition** Especifica o estado quando um item é excluído de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e72db-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="e72db-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="e72db-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e72db-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e72db-106">Attributes and elements</span></span>

<span data-ttu-id="e72db-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e72db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e72db-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e72db-108">Attributes</span></span>

<span data-ttu-id="e72db-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e72db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e72db-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e72db-110">Child elements</span></span>

|<span data-ttu-id="e72db-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e72db-111">**Element**</span></span>|<span data-ttu-id="e72db-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e72db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e72db-113">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="e72db-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="e72db-114">Especifica a data da ocorrência de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="e72db-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e72db-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="e72db-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="e72db-116">Especifica um valor Boolean que indica se uma ocorrência de um item do calendário está presente.</span><span class="sxs-lookup"><span data-stu-id="e72db-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e72db-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e72db-117">Parent elements</span></span>

|<span data-ttu-id="e72db-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e72db-118">**Element**</span></span>|<span data-ttu-id="e72db-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e72db-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e72db-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="e72db-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="e72db-121">Especifica uma definição de estado.</span><span class="sxs-lookup"><span data-stu-id="e72db-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e72db-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e72db-122">Remarks</span></span>

<span data-ttu-id="e72db-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e72db-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e72db-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e72db-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e72db-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e72db-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e72db-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="e72db-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e72db-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e72db-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e72db-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="e72db-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="e72db-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e72db-129">Validation File</span></span>  <br/> |<span data-ttu-id="e72db-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e72db-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e72db-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e72db-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e72db-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="e72db-132">See also</span></span>

- [<span data-ttu-id="e72db-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e72db-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

