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
ms.openlocfilehash: 269c1176913cd642f93987462286dd1fee3a7339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751740"
---
# <a name="deletedoccurrences"></a><span data-ttu-id="3bd33-103">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="3bd33-103">DeletedOccurrences</span></span>

<span data-ttu-id="3bd33-104">O elemento **DeletedOccurrences** contém uma matriz de ocorrências excluídas de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3bd33-104">The **DeletedOccurrences** element contains an array of deleted occurrences of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrences>
   <DeletedOccurrence/>
</DeletedOccurrences>
```

 <span data-ttu-id="3bd33-105">**NonEmptyArrayOfDeletedOccurrencesType**</span><span class="sxs-lookup"><span data-stu-id="3bd33-105">**NonEmptyArrayOfDeletedOccurrencesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3bd33-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3bd33-106">Attributes and elements</span></span>

<span data-ttu-id="3bd33-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3bd33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3bd33-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3bd33-108">Attributes</span></span>

<span data-ttu-id="3bd33-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3bd33-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3bd33-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3bd33-110">Child elements</span></span>

|<span data-ttu-id="3bd33-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3bd33-111">**Element**</span></span>|<span data-ttu-id="3bd33-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3bd33-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bd33-113">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="3bd33-113">DeletedOccurrence</span></span>](deletedoccurrence.md) <br/> |<span data-ttu-id="3bd33-114">Representa uma ocorrência excluída de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="3bd33-114">Represents a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3bd33-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3bd33-115">Parent elements</span></span>

|<span data-ttu-id="3bd33-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3bd33-116">**Element**</span></span>|<span data-ttu-id="3bd33-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3bd33-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3bd33-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3bd33-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3bd33-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bd33-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3bd33-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3bd33-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3bd33-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3bd33-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3bd33-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3bd33-122">Remarks</span></span>

<span data-ttu-id="3bd33-123">Esse elemento é válido se o valor de texto de RecurringMaster é usado para o elemento [CalendarItemType](calendaritemtype.md) .</span><span class="sxs-lookup"><span data-stu-id="3bd33-123">This element is valid if the RecurringMaster text value is used for the [CalendarItemType](calendaritemtype.md) element.</span></span> 
  
<span data-ttu-id="3bd33-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3bd33-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3bd33-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3bd33-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3bd33-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="3bd33-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3bd33-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3bd33-127">Schema name</span></span>  <br/> |<span data-ttu-id="3bd33-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3bd33-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3bd33-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3bd33-129">Validation file</span></span>  <br/> |<span data-ttu-id="3bd33-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3bd33-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3bd33-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3bd33-131">Can be empty</span></span>  <br/> |<span data-ttu-id="3bd33-132">False</span><span class="sxs-lookup"><span data-stu-id="3bd33-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3bd33-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="3bd33-133">See also</span></span>

- [<span data-ttu-id="3bd33-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3bd33-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- [<span data-ttu-id="3bd33-135">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="3bd33-135">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

