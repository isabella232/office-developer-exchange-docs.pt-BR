---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: O elemento DeletedOccurrence representa uma ocorrência excluída de um item de calendário recorrente.
ms.openlocfilehash: f12a2ba20f87f7803e492d8422b68c8ecdf9d797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751736"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="cbd1a-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="cbd1a-103">DeletedOccurrence</span></span>

<span data-ttu-id="cbd1a-104">O elemento **DeletedOccurrence** representa uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="cbd1a-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="cbd1a-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbd1a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cbd1a-106">Attributes and elements</span></span>

<span data-ttu-id="cbd1a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbd1a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cbd1a-108">Attributes</span></span>

<span data-ttu-id="cbd1a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbd1a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cbd1a-110">Child elements</span></span>

|<span data-ttu-id="cbd1a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cbd1a-111">**Element**</span></span>|<span data-ttu-id="cbd1a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cbd1a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbd1a-113">Start</span><span class="sxs-lookup"><span data-stu-id="cbd1a-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="cbd1a-114">Representa a hora de início de uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cbd1a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cbd1a-115">Parent elements</span></span>

|<span data-ttu-id="cbd1a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cbd1a-116">**Element**</span></span>|<span data-ttu-id="cbd1a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cbd1a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbd1a-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="cbd1a-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="cbd1a-119">Contém uma matriz de ocorrências excluídas de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cbd1a-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="cbd1a-120">Remarks</span></span>

<span data-ttu-id="cbd1a-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cbd1a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbd1a-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cbd1a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbd1a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="cbd1a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbd1a-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cbd1a-124">Schema name</span></span>  <br/> |<span data-ttu-id="cbd1a-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cbd1a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbd1a-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cbd1a-126">Validation file</span></span>  <br/> |<span data-ttu-id="cbd1a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cbd1a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbd1a-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cbd1a-128">Can be empty</span></span>  <br/> |<span data-ttu-id="cbd1a-129">False</span><span class="sxs-lookup"><span data-stu-id="cbd1a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbd1a-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="cbd1a-130">See also</span></span>

- [<span data-ttu-id="cbd1a-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cbd1a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="cbd1a-132">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="cbd1a-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

