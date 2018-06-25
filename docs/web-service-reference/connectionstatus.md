---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: O elemento ConnectionStatus fornece uma descrição de texto do status de uma assinatura de streaming.
ms.openlocfilehash: 567308d79eaccba24230deddf5d78a724b8746af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751428"
---
# <a name="connectionstatus"></a><span data-ttu-id="1d46d-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="1d46d-103">ConnectionStatus</span></span>

<span data-ttu-id="1d46d-104">O elemento **ConnectionStatus** fornece uma descrição de texto do status de uma assinatura de streaming.</span><span class="sxs-lookup"><span data-stu-id="1d46d-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="1d46d-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="1d46d-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d46d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1d46d-106">Attributes and elements</span></span>

<span data-ttu-id="1d46d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1d46d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d46d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1d46d-108">Attributes</span></span>

<span data-ttu-id="1d46d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1d46d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d46d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1d46d-110">Child elements</span></span>

<span data-ttu-id="1d46d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1d46d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d46d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1d46d-112">Parent elements</span></span>

|<span data-ttu-id="1d46d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1d46d-113">**Element**</span></span>|<span data-ttu-id="1d46d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1d46d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d46d-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d46d-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="1d46d-116">Contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="1d46d-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d46d-117">Text value</span><span class="sxs-lookup"><span data-stu-id="1d46d-117">Text value</span></span>

<span data-ttu-id="1d46d-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="1d46d-118">A text value is required.</span></span> <span data-ttu-id="1d46d-119">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="1d46d-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="1d46d-120">OK</span><span class="sxs-lookup"><span data-stu-id="1d46d-120">OK</span></span>
    
- <span data-ttu-id="1d46d-121">Closed</span><span class="sxs-lookup"><span data-stu-id="1d46d-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1d46d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="1d46d-122">Remarks</span></span>

<span data-ttu-id="1d46d-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1d46d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d46d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1d46d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d46d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d46d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d46d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1d46d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1d46d-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1d46d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d46d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1d46d-128">Validation File</span></span>  <br/> |<span data-ttu-id="1d46d-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1d46d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d46d-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1d46d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d46d-131">False</span><span class="sxs-lookup"><span data-stu-id="1d46d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d46d-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="1d46d-132">See also</span></span>



[<span data-ttu-id="1d46d-133">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="1d46d-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="1d46d-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1d46d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

