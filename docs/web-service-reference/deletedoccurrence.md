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
ms.openlocfilehash: 814a81934786963ae5e7ea3a40406834c27b64ce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457834"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="b6dd3-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="b6dd3-103">DeletedOccurrence</span></span>

<span data-ttu-id="b6dd3-104">O elemento **DeletedOccurrence** representa uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="b6dd3-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="b6dd3-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="b6dd3-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6dd3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b6dd3-106">Attributes and elements</span></span>

<span data-ttu-id="b6dd3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b6dd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6dd3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b6dd3-108">Attributes</span></span>

<span data-ttu-id="b6dd3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6dd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6dd3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b6dd3-110">Child elements</span></span>

|<span data-ttu-id="b6dd3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6dd3-111">**Element**</span></span>|<span data-ttu-id="b6dd3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6dd3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6dd3-113">Start</span><span class="sxs-lookup"><span data-stu-id="b6dd3-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="b6dd3-114">Representa a hora de início de uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="b6dd3-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6dd3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b6dd3-115">Parent elements</span></span>

|<span data-ttu-id="b6dd3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6dd3-116">**Element**</span></span>|<span data-ttu-id="b6dd3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6dd3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6dd3-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="b6dd3-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="b6dd3-119">Contém uma matriz de ocorrências excluídas de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="b6dd3-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6dd3-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="b6dd3-120">Remarks</span></span>

<span data-ttu-id="b6dd3-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b6dd3-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6dd3-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b6dd3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6dd3-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6dd3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6dd3-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b6dd3-124">Schema name</span></span>  <br/> |<span data-ttu-id="b6dd3-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b6dd3-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6dd3-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b6dd3-126">Validation file</span></span>  <br/> |<span data-ttu-id="b6dd3-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b6dd3-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6dd3-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b6dd3-128">Can be empty</span></span>  <br/> |<span data-ttu-id="b6dd3-129">False</span><span class="sxs-lookup"><span data-stu-id="b6dd3-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6dd3-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6dd3-130">See also</span></span>

- [<span data-ttu-id="b6dd3-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6dd3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="b6dd3-132">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="b6dd3-132">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

