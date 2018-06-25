---
title: EventData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventData
api_type:
- schema
ms.assetid: 74acdbad-d6ee-47e6-82fb-e45ecaaa0500
description: O elemento EventData representa os dados que está associados com a etapa de processamento para o evento.
ms.openlocfilehash: 2bf38cd4fd956580b31b6e455b947066f07f5593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752105"
---
# <a name="eventdata"></a><span data-ttu-id="4c572-103">EventData</span><span class="sxs-lookup"><span data-stu-id="4c572-103">EventData</span></span>

<span data-ttu-id="4c572-104">O elemento **EventData** representa os dados que está associados com a etapa de processamento para o evento.</span><span class="sxs-lookup"><span data-stu-id="4c572-104">The **EventData** element represents data that is associated with the processing step for the event.</span></span> 
  
```XML
<EventData>
   <String/>
</EventData>
```

 <span data-ttu-id="4c572-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="4c572-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c572-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4c572-106">Attributes and elements</span></span>

<span data-ttu-id="4c572-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4c572-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c572-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4c572-108">Attributes</span></span>

<span data-ttu-id="4c572-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4c572-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c572-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4c572-110">Child elements</span></span>

|<span data-ttu-id="4c572-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4c572-111">**Element**</span></span>|<span data-ttu-id="4c572-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c572-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c572-113">String</span><span class="sxs-lookup"><span data-stu-id="4c572-113">String</span></span>](string.md) <br/> |<span data-ttu-id="4c572-114">Contém uma cadeia de caracteres que identifica um evento.</span><span class="sxs-lookup"><span data-stu-id="4c572-114">Contains a string that identifies an event.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c572-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4c572-115">Parent elements</span></span>

|<span data-ttu-id="4c572-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4c572-116">**Element**</span></span>|<span data-ttu-id="4c572-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c572-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c572-118">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="4c572-118">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="4c572-119">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="4c572-119">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4c572-120">Text value</span><span class="sxs-lookup"><span data-stu-id="4c572-120">Text value</span></span>

<span data-ttu-id="4c572-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4c572-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4c572-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="4c572-122">Remarks</span></span>

<span data-ttu-id="4c572-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c572-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c572-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4c572-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c572-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="4c572-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c572-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4c572-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4c572-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4c572-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c572-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4c572-128">Validation File</span></span>  <br/> |<span data-ttu-id="4c572-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c572-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c572-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4c572-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c572-131">False</span><span class="sxs-lookup"><span data-stu-id="4c572-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c572-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="4c572-132">See also</span></span>



- [<span data-ttu-id="4c572-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4c572-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

