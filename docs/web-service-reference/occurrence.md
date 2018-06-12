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
description: O elemento de ocorrência representa uma única ocorrência de modificação de um item de calendário recorrente.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824653"
---
# <a name="occurrence"></a><span data-ttu-id="3acb0-103">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="3acb0-103">Occurrence</span></span>

<span data-ttu-id="3acb0-104">O elemento de **ocorrência** representa uma única ocorrência de modificação de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3acb0-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="3acb0-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="3acb0-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3acb0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3acb0-106">Attributes and elements</span></span>

<span data-ttu-id="3acb0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3acb0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3acb0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3acb0-108">Attributes</span></span>

<span data-ttu-id="3acb0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3acb0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3acb0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3acb0-110">Child elements</span></span>

|<span data-ttu-id="3acb0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3acb0-111">**Element**</span></span>|<span data-ttu-id="3acb0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3acb0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3acb0-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="3acb0-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3acb0-114">Contém a chave exclusiva de identificador e alteração de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3acb0-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3acb0-115">Start</span><span class="sxs-lookup"><span data-stu-id="3acb0-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="3acb0-116">Representa a hora de início de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3acb0-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3acb0-117">End</span><span class="sxs-lookup"><span data-stu-id="3acb0-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3acb0-118">Representa a hora de término de uma ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3acb0-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3acb0-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="3acb0-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="3acb0-120">Representa a hora de início original de um item de calendário recorrente a uma ocorrência modificada.</span><span class="sxs-lookup"><span data-stu-id="3acb0-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3acb0-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3acb0-121">Parent elements</span></span>

|<span data-ttu-id="3acb0-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3acb0-122">**Element**</span></span>|<span data-ttu-id="3acb0-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3acb0-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3acb0-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="3acb0-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="3acb0-125">Contém uma coleção de recorrente ocorrências de item de calendário que foram modificados para que sejam diferentes do que o item de recorrência mestre.</span><span class="sxs-lookup"><span data-stu-id="3acb0-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3acb0-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="3acb0-126">Remarks</span></span>

<span data-ttu-id="3acb0-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3acb0-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3acb0-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3acb0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3acb0-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3acb0-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3acb0-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3acb0-130">Schema name</span></span>  <br/> |<span data-ttu-id="3acb0-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3acb0-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3acb0-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3acb0-132">Validation file</span></span>  <br/> |<span data-ttu-id="3acb0-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3acb0-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3acb0-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3acb0-134">Can be empty</span></span>  <br/> |<span data-ttu-id="3acb0-135">False</span><span class="sxs-lookup"><span data-stu-id="3acb0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3acb0-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="3acb0-136">See also</span></span>

- [<span data-ttu-id="3acb0-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3acb0-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

