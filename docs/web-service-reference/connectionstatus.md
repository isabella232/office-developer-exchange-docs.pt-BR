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
ms.openlocfilehash: 928537201041950011ae06444e3c412228d252ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462714"
---
# <a name="connectionstatus"></a><span data-ttu-id="e72a2-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="e72a2-103">ConnectionStatus</span></span>

<span data-ttu-id="e72a2-104">O elemento **ConnectionStatus** fornece uma descrição de texto do status de uma assinatura de streaming.</span><span class="sxs-lookup"><span data-stu-id="e72a2-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="e72a2-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="e72a2-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e72a2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e72a2-106">Attributes and elements</span></span>

<span data-ttu-id="e72a2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e72a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e72a2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e72a2-108">Attributes</span></span>

<span data-ttu-id="e72a2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e72a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e72a2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e72a2-110">Child elements</span></span>

<span data-ttu-id="e72a2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e72a2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e72a2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e72a2-112">Parent elements</span></span>

|<span data-ttu-id="e72a2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e72a2-113">**Element**</span></span>|<span data-ttu-id="e72a2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e72a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e72a2-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e72a2-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="e72a2-116">Contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e72a2-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e72a2-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e72a2-117">Text value</span></span>

<span data-ttu-id="e72a2-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e72a2-118">A text value is required.</span></span> <span data-ttu-id="e72a2-119">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="e72a2-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="e72a2-120">OK</span><span class="sxs-lookup"><span data-stu-id="e72a2-120">OK</span></span>
    
- <span data-ttu-id="e72a2-121">Fechado</span><span class="sxs-lookup"><span data-stu-id="e72a2-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e72a2-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="e72a2-122">Remarks</span></span>

<span data-ttu-id="e72a2-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e72a2-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e72a2-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e72a2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e72a2-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e72a2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e72a2-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e72a2-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e72a2-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e72a2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e72a2-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e72a2-128">Validation File</span></span>  <br/> |<span data-ttu-id="e72a2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e72a2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e72a2-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e72a2-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e72a2-131">False</span><span class="sxs-lookup"><span data-stu-id="e72a2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e72a2-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="e72a2-132">See also</span></span>



[<span data-ttu-id="e72a2-133">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="e72a2-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="e72a2-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e72a2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

