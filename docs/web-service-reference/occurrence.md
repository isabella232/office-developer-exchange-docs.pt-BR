---
title: Ocorrência
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: O elemento ocorrência representa uma única ocorrência modificada de um item de calendário recorrente.
ms.openlocfilehash: c3a6bcce23f0bb1125dbd2a5bb86e9b20039a4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466315"
---
# <a name="occurrence"></a><span data-ttu-id="5c5d8-103">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="5c5d8-103">Occurrence</span></span>

<span data-ttu-id="5c5d8-104">O elemento **ocorrência** representa uma única ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="5c5d8-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="5c5d8-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5c5d8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5c5d8-106">Attributes and elements</span></span>

<span data-ttu-id="5c5d8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c5d8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c5d8-108">Attributes</span></span>

<span data-ttu-id="5c5d8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c5d8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c5d8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c5d8-110">Child elements</span></span>

|<span data-ttu-id="5c5d8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c5d8-111">**Element**</span></span>|<span data-ttu-id="5c5d8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c5d8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c5d8-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="5c5d8-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5c5d8-114">Contém o identificador exclusivo e a chave de alteração de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c5d8-115">Start</span><span class="sxs-lookup"><span data-stu-id="5c5d8-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="5c5d8-116">Representa a hora de início de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c5d8-117">Ponto</span><span class="sxs-lookup"><span data-stu-id="5c5d8-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5c5d8-118">Representa a hora de término de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c5d8-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="5c5d8-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="5c5d8-120">Representa a hora de início original de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c5d8-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c5d8-121">Parent elements</span></span>

|<span data-ttu-id="5c5d8-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c5d8-122">**Element**</span></span>|<span data-ttu-id="5c5d8-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c5d8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c5d8-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="5c5d8-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="5c5d8-125">Contém uma coleção de ocorrências de itens de calendário recorrentes que foram modificadas para que sejam diferentes do item mestre de recorrência.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c5d8-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c5d8-126">Remarks</span></span>

<span data-ttu-id="5c5d8-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5c5d8-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c5d8-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5c5d8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c5d8-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c5d8-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c5d8-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c5d8-130">Schema name</span></span>  <br/> |<span data-ttu-id="5c5d8-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5c5d8-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c5d8-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c5d8-132">Validation file</span></span>  <br/> |<span data-ttu-id="5c5d8-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5c5d8-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c5d8-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5c5d8-134">Can be empty</span></span>  <br/> |<span data-ttu-id="5c5d8-135">False</span><span class="sxs-lookup"><span data-stu-id="5c5d8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c5d8-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c5d8-136">See also</span></span>

- [<span data-ttu-id="5c5d8-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c5d8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

