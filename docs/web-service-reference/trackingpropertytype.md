---
title: TrackingPropertyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TrackingPropertyType
api_type:
- schema
ms.assetid: 1d0f219b-1063-4eaa-9d3b-da384a544f89
description: O elemento TrackingPropertyType representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de controle de mensagens.
ms.openlocfilehash: 7812b52dd57fed0a9b6f1a8fc4e77660932a60dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468079"
---
# <a name="trackingpropertytype"></a><span data-ttu-id="58462-103">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="58462-103">TrackingPropertyType</span></span>

<span data-ttu-id="58462-104">O elemento **TrackingPropertyType** representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="58462-104">The **TrackingPropertyType** element represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span> 
  
[<span data-ttu-id="58462-105">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="58462-105">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
[<span data-ttu-id="58462-106">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="58462-106">TrackingPropertyType</span></span>](trackingpropertytype.md)
  
```xml
<TrackingPropertyType>
   <Name/>
   <Value/>
</TrackingPropertyType>
```

 <span data-ttu-id="58462-107">**TrackingPropertyType**</span><span class="sxs-lookup"><span data-stu-id="58462-107">**TrackingPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58462-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58462-108">Attributes and elements</span></span>

<span data-ttu-id="58462-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58462-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58462-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="58462-110">Attributes</span></span>

<span data-ttu-id="58462-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58462-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58462-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58462-112">Child elements</span></span>

|<span data-ttu-id="58462-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58462-113">**Element**</span></span>|<span data-ttu-id="58462-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58462-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58462-115">Nome (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="58462-115">Name (Message Tracking)</span></span>](name-message-tracking.md) <br/> |<span data-ttu-id="58462-116">Define um nome para a propriedade do relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="58462-116">Defines a name for the message tracking report property.</span></span>  <br/> |
|[<span data-ttu-id="58462-117">Valor (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="58462-117">Value (Message Tracking)</span></span>](value-message-tracking.md) <br/> |<span data-ttu-id="58462-118">Define um valor para a propriedade do relatório de controle de mensagens.</span><span class="sxs-lookup"><span data-stu-id="58462-118">Defines a value for the message tracking report property.</span></span> <span data-ttu-id="58462-119">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="58462-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58462-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58462-120">Parent elements</span></span>

|<span data-ttu-id="58462-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58462-121">**Element**</span></span>|<span data-ttu-id="58462-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58462-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58462-123">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="58462-123">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="58462-124">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="58462-124">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58462-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="58462-125">Text value</span></span>

<span data-ttu-id="58462-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58462-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58462-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="58462-127">Remarks</span></span>

<span data-ttu-id="58462-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="58462-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58462-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58462-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58462-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="58462-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="58462-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58462-131">Schema Name</span></span>  <br/> |<span data-ttu-id="58462-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="58462-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="58462-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58462-133">Validation File</span></span>  <br/> |<span data-ttu-id="58462-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="58462-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="58462-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="58462-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="58462-136">False</span><span class="sxs-lookup"><span data-stu-id="58462-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58462-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="58462-137">See also</span></span>



- [<span data-ttu-id="58462-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58462-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

