---
title: RecipientTrackingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvents
api_type:
- schema
ms.assetid: c4f729aa-674e-43b2-97f2-bf49740b0a34
description: O elemento RecipientTrackingEvents representa uma coleção de eventos de um ou mais de uma mensagem.
ms.openlocfilehash: 5fa5df422eff533891d021b77d5443b314d36244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824993"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="f2d42-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="f2d42-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="f2d42-104">O elemento **RecipientTrackingEvents** representa uma coleção de eventos de um ou mais de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="f2d42-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="f2d42-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="f2d42-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2d42-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f2d42-106">Attributes and elements</span></span>

<span data-ttu-id="f2d42-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f2d42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2d42-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f2d42-108">Attributes</span></span>

<span data-ttu-id="f2d42-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f2d42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2d42-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f2d42-110">Child elements</span></span>

|<span data-ttu-id="f2d42-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2d42-111">**Element**</span></span>|<span data-ttu-id="f2d42-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2d42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2d42-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="f2d42-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="f2d42-114">Contém detalhes para um evento específico no relatório de controle.</span><span class="sxs-lookup"><span data-stu-id="f2d42-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2d42-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f2d42-115">Parent elements</span></span>

|<span data-ttu-id="f2d42-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f2d42-116">**Element**</span></span>|<span data-ttu-id="f2d42-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f2d42-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2d42-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f2d42-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="f2d42-119">Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f2d42-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2d42-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2d42-120">Remarks</span></span>

<span data-ttu-id="f2d42-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f2d42-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2d42-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f2d42-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2d42-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f2d42-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2d42-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f2d42-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f2d42-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f2d42-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2d42-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f2d42-126">Validation File</span></span>  <br/> |<span data-ttu-id="f2d42-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2d42-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2d42-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f2d42-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2d42-129">False</span><span class="sxs-lookup"><span data-stu-id="f2d42-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2d42-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="f2d42-130">See also</span></span>



[<span data-ttu-id="f2d42-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f2d42-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f2d42-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f2d42-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

