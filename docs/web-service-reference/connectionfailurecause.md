---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: O elemento ConnectionFailureCause Especifica o motivo para uma desconexão de uma chamada telefônica.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751426"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="28e5e-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="28e5e-103">ConnectionFailureCause</span></span>

<span data-ttu-id="28e5e-104">O elemento **ConnectionFailureCause** Especifica o motivo para uma desconexão de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="28e5e-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="28e5e-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="28e5e-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28e5e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="28e5e-106">Attributes and elements</span></span>

<span data-ttu-id="28e5e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="28e5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28e5e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="28e5e-108">Attributes</span></span>

<span data-ttu-id="28e5e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="28e5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28e5e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="28e5e-110">Child elements</span></span>

<span data-ttu-id="28e5e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="28e5e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28e5e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="28e5e-112">Parent elements</span></span>

|<span data-ttu-id="28e5e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="28e5e-113">**Element**</span></span>|<span data-ttu-id="28e5e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="28e5e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28e5e-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="28e5e-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="28e5e-116">Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="28e5e-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28e5e-117">Text value</span><span class="sxs-lookup"><span data-stu-id="28e5e-117">Text value</span></span>

<span data-ttu-id="28e5e-118">A tabela a seguir lista os valores possíveis para o elemento **ConnectionFailureCause** .</span><span class="sxs-lookup"><span data-stu-id="28e5e-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="28e5e-119">**Valores de elemento ConnectionFailureCause**</span><span class="sxs-lookup"><span data-stu-id="28e5e-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="28e5e-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="28e5e-120">**Value**</span></span>|<span data-ttu-id="28e5e-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="28e5e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28e5e-122">None</span><span class="sxs-lookup"><span data-stu-id="28e5e-122">None</span></span>  <br/> |<span data-ttu-id="28e5e-123">Estado de chamada não for desconectado ou o motivo de desconexão não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="28e5e-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="28e5e-124">UserBusy</span><span class="sxs-lookup"><span data-stu-id="28e5e-124">UserBusy</span></span>  <br/> |<span data-ttu-id="28e5e-125">A linha da parte chamada estava ocupada.</span><span class="sxs-lookup"><span data-stu-id="28e5e-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="28e5e-126">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="28e5e-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="28e5e-127">A parte chamada não atendida.</span><span class="sxs-lookup"><span data-stu-id="28e5e-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="28e5e-128">Unavailable</span><span class="sxs-lookup"><span data-stu-id="28e5e-128">Unavailable</span></span>  <br/> |<span data-ttu-id="28e5e-129">O número da parte chamada não estava disponível.</span><span class="sxs-lookup"><span data-stu-id="28e5e-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="28e5e-130">Outro</span><span class="sxs-lookup"><span data-stu-id="28e5e-130">Other</span></span>  <br/> |<span data-ttu-id="28e5e-131">Pega-tudo por outros motivos desconectar.</span><span class="sxs-lookup"><span data-stu-id="28e5e-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28e5e-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="28e5e-132">Remarks</span></span>

<span data-ttu-id="28e5e-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="28e5e-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28e5e-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="28e5e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28e5e-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="28e5e-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28e5e-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="28e5e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="28e5e-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="28e5e-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="28e5e-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="28e5e-138">Validation File</span></span>  <br/> |<span data-ttu-id="28e5e-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28e5e-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28e5e-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="28e5e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="28e5e-141">False</span><span class="sxs-lookup"><span data-stu-id="28e5e-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28e5e-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="28e5e-142">See also</span></span>



- [<span data-ttu-id="28e5e-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="28e5e-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

