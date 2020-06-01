---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: O elemento DeleteFromFolderStateDefinition especifica o estado quando um item é excluído de uma pasta.
ms.openlocfilehash: 0ea8c61a6839790869781d5d87ca81772b2e38d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455720"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="6584e-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="6584e-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="6584e-104">O elemento **DeleteFromFolderStateDefinition** especifica o estado quando um item é excluído de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6584e-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="6584e-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="6584e-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6584e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6584e-106">Attributes and elements</span></span>

<span data-ttu-id="6584e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6584e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6584e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6584e-108">Attributes</span></span>

<span data-ttu-id="6584e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6584e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6584e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6584e-110">Child elements</span></span>

|<span data-ttu-id="6584e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6584e-111">**Element**</span></span>|<span data-ttu-id="6584e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6584e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6584e-113">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="6584e-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="6584e-114">Especifica a data da ocorrência de um item do calendário.</span><span class="sxs-lookup"><span data-stu-id="6584e-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6584e-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="6584e-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="6584e-116">Especifica um valor Boolean que indica se uma ocorrência do item de calendário está presente.</span><span class="sxs-lookup"><span data-stu-id="6584e-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6584e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6584e-117">Parent elements</span></span>

|<span data-ttu-id="6584e-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6584e-118">**Element**</span></span>|<span data-ttu-id="6584e-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6584e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6584e-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="6584e-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="6584e-121">Especifica uma definição de estado.</span><span class="sxs-lookup"><span data-stu-id="6584e-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6584e-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6584e-122">Remarks</span></span>

<span data-ttu-id="6584e-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6584e-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6584e-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6584e-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6584e-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6584e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6584e-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6584e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6584e-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6584e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6584e-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="6584e-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="6584e-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6584e-129">Validation File</span></span>  <br/> |<span data-ttu-id="6584e-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6584e-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6584e-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6584e-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6584e-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="6584e-132">See also</span></span>

- [<span data-ttu-id="6584e-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6584e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

