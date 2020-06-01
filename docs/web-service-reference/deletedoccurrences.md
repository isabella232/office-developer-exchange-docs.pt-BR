---
title: DeletedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrences
api_type:
- schema
ms.assetid: 736fb305-9528-4be8-ad37-65d7556edbf2
description: O elemento DeletedOccurrences contém uma matriz de ocorrências excluídas de um item de calendário recorrente.
ms.openlocfilehash: be39ff95b5529481a36b7549e638818a20e01283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463703"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="ed150-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="ed150-103">DeletedOccurrences</span></span>

<span data-ttu-id="ed150-104">O elemento **DeletedOccurrences** contém uma matriz de ocorrências excluídas de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ed150-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="ed150-105">**NonEmptyArrayOfDeletedOccurrencesType**</span><span class="sxs-lookup"><span data-stu-id="ed150-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed150-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ed150-106">Attributes and elements</span></span>

<span data-ttu-id="ed150-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed150-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed150-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed150-108">Attributes</span></span>

<span data-ttu-id="ed150-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed150-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed150-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed150-110">Child elements</span></span>

|<span data-ttu-id="ed150-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed150-111">**Element**</span></span>|<span data-ttu-id="ed150-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed150-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed150-113">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="ed150-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="ed150-114">Representa uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="ed150-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed150-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed150-115">Parent elements</span></span>

|<span data-ttu-id="ed150-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed150-116">**Element**</span></span>|<span data-ttu-id="ed150-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed150-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed150-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ed150-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ed150-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed150-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ed150-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ed150-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ed150-121">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed150-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ed150-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed150-122">Remarks</span></span>

<span data-ttu-id="ed150-123">Este elemento é válido se o valor de texto RecurringMaster é usado para o elemento [CalendarItemType](calendaritemtype.md) .</span><span class="sxs-lookup"><span data-stu-id="ed150-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="ed150-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ed150-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed150-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ed150-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed150-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed150-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed150-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed150-127">Schema name</span></span>  <br/> |<span data-ttu-id="ed150-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ed150-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed150-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed150-129">Validation file</span></span>  <br/> |<span data-ttu-id="ed150-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ed150-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed150-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ed150-131">Can be empty</span></span>  <br/> |<span data-ttu-id="ed150-132">False</span><span class="sxs-lookup"><span data-stu-id="ed150-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed150-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="ed150-133">See also</span></span>

- [<span data-ttu-id="ed150-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ed150-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="ed150-135">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="ed150-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

