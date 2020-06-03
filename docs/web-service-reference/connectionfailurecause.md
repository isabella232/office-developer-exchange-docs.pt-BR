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
description: O elemento ConnectionFailureCause especifica a razão para uma desconexão de uma chamada telefônica.
ms.openlocfilehash: 6385641eaee140a114906703232974d51d5ce344
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529445"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="96825-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="96825-103">ConnectionFailureCause</span></span>

<span data-ttu-id="96825-104">O elemento **ConnectionFailureCause** especifica a razão para uma desconexão de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="96825-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="96825-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="96825-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96825-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96825-106">Attributes and elements</span></span>

<span data-ttu-id="96825-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96825-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96825-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="96825-108">Attributes</span></span>

<span data-ttu-id="96825-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96825-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96825-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96825-110">Child elements</span></span>

<span data-ttu-id="96825-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96825-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96825-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96825-112">Parent elements</span></span>

|<span data-ttu-id="96825-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96825-113">**Element**</span></span>|<span data-ttu-id="96825-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96825-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96825-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="96825-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="96825-116">Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="96825-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96825-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="96825-117">Text value</span></span>

<span data-ttu-id="96825-118">A tabela a seguir lista os valores possíveis para o elemento **ConnectionFailureCause** .</span><span class="sxs-lookup"><span data-stu-id="96825-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="96825-119">**Valores do elemento ConnectionFailureCause**</span><span class="sxs-lookup"><span data-stu-id="96825-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="96825-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="96825-120">**Value**</span></span>|<span data-ttu-id="96825-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96825-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96825-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96825-122">None</span></span>  <br/> |<span data-ttu-id="96825-123">O estado de chamada não é desconectado ou o motivo da desconexão não é conhecido.</span><span class="sxs-lookup"><span data-stu-id="96825-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="96825-124">Userbusy</span><span class="sxs-lookup"><span data-stu-id="96825-124">UserBusy</span></span>  <br/> |<span data-ttu-id="96825-125">A linha do participante chamada estava ocupada.</span><span class="sxs-lookup"><span data-stu-id="96825-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="96825-126">NOANSWER</span><span class="sxs-lookup"><span data-stu-id="96825-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="96825-127">A parte chamada não respondeu.</span><span class="sxs-lookup"><span data-stu-id="96825-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="96825-128">Indisponível</span><span class="sxs-lookup"><span data-stu-id="96825-128">Unavailable</span></span>  <br/> |<span data-ttu-id="96825-129">O número da parte chamada não estava disponível.</span><span class="sxs-lookup"><span data-stu-id="96825-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="96825-130">Outros</span><span class="sxs-lookup"><span data-stu-id="96825-130">Other</span></span>  <br/> |<span data-ttu-id="96825-131">Catch-tudo por outros motivos de desconexão.</span><span class="sxs-lookup"><span data-stu-id="96825-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="96825-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="96825-132">Remarks</span></span>

<span data-ttu-id="96825-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="96825-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96825-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96825-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96825-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="96825-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96825-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96825-136">Schema Name</span></span>  <br/> |<span data-ttu-id="96825-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="96825-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="96825-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96825-138">Validation File</span></span>  <br/> |<span data-ttu-id="96825-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="96825-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96825-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96825-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="96825-141">False</span><span class="sxs-lookup"><span data-stu-id="96825-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96825-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="96825-142">See also</span></span>



- [<span data-ttu-id="96825-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96825-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

