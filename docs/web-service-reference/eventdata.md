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
description: O elemento EventData representa os dados associados à etapa de processamento do evento.
ms.openlocfilehash: ef5da21a3300a6939c60d62584b46ca48b071853
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526176"
---
# <a name="eventdata"></a><span data-ttu-id="215e5-103">EventData</span><span class="sxs-lookup"><span data-stu-id="215e5-103">EventData</span></span>

<span data-ttu-id="215e5-104">O elemento **EVENTDATA** representa os dados associados à etapa de processamento do evento.</span><span class="sxs-lookup"><span data-stu-id="215e5-104">The **EventData** element represents data that is associated with the processing step for the event.</span></span> 
  
```XML
<EventData>
   <String/>
</EventData>
```

 <span data-ttu-id="215e5-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="215e5-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="215e5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="215e5-106">Attributes and elements</span></span>

<span data-ttu-id="215e5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="215e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="215e5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="215e5-108">Attributes</span></span>

<span data-ttu-id="215e5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="215e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="215e5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="215e5-110">Child elements</span></span>

|<span data-ttu-id="215e5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="215e5-111">**Element**</span></span>|<span data-ttu-id="215e5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="215e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="215e5-113">String</span><span class="sxs-lookup"><span data-stu-id="215e5-113">String</span></span>](string.md) <br/> |<span data-ttu-id="215e5-114">Contém uma cadeia de caracteres que identifica um evento.</span><span class="sxs-lookup"><span data-stu-id="215e5-114">Contains a string that identifies an event.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="215e5-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="215e5-115">Parent elements</span></span>

|<span data-ttu-id="215e5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="215e5-116">**Element**</span></span>|<span data-ttu-id="215e5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="215e5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="215e5-118">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="215e5-118">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="215e5-119">Contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="215e5-119">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="215e5-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="215e5-120">Text value</span></span>

<span data-ttu-id="215e5-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="215e5-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="215e5-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="215e5-122">Remarks</span></span>

<span data-ttu-id="215e5-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="215e5-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="215e5-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="215e5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="215e5-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="215e5-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="215e5-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="215e5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="215e5-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="215e5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="215e5-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="215e5-128">Validation File</span></span>  <br/> |<span data-ttu-id="215e5-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="215e5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="215e5-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="215e5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="215e5-131">False</span><span class="sxs-lookup"><span data-stu-id="215e5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="215e5-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="215e5-132">See also</span></span>



- [<span data-ttu-id="215e5-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="215e5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

