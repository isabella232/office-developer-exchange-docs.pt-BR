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
description: O elemento RecipientTrackingEvents representa uma coleção de um ou mais eventos de uma mensagem.
ms.openlocfilehash: c0b25a0e22d13bc1f26768b9b7089d96eb2e8cfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468478"
---
# <a name="recipienttrackingevents"></a><span data-ttu-id="3e45a-103">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="3e45a-103">RecipientTrackingEvents</span></span>

<span data-ttu-id="3e45a-104">O elemento **RecipientTrackingEvents** representa uma coleção de um ou mais eventos de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3e45a-104">The **RecipientTrackingEvents** element represents a collection of one or more events for a message.</span></span> 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 <span data-ttu-id="3e45a-105">**ArrayOfRecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="3e45a-105">**ArrayOfRecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e45a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3e45a-106">Attributes and elements</span></span>

<span data-ttu-id="3e45a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3e45a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e45a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3e45a-108">Attributes</span></span>

<span data-ttu-id="3e45a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e45a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e45a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3e45a-110">Child elements</span></span>

|<span data-ttu-id="3e45a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3e45a-111">**Element**</span></span>|<span data-ttu-id="3e45a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3e45a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e45a-113">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="3e45a-113">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="3e45a-114">Contém detalhes de um evento específico no relatório de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="3e45a-114">Contains details for a specific event in the tracking report.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e45a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3e45a-115">Parent elements</span></span>

|<span data-ttu-id="3e45a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3e45a-116">**Element**</span></span>|<span data-ttu-id="3e45a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3e45a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e45a-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3e45a-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="3e45a-119">Contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3e45a-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3e45a-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="3e45a-120">Remarks</span></span>

<span data-ttu-id="3e45a-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e45a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e45a-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3e45a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e45a-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="3e45a-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e45a-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3e45a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3e45a-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3e45a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e45a-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3e45a-126">Validation File</span></span>  <br/> |<span data-ttu-id="3e45a-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3e45a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e45a-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3e45a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e45a-129">False</span><span class="sxs-lookup"><span data-stu-id="3e45a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e45a-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="3e45a-130">See also</span></span>



[<span data-ttu-id="3e45a-131">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="3e45a-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="3e45a-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3e45a-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

