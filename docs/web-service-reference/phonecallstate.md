---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: O elemento PhoneCallState Especifica o estado atual de uma chamada telefônica.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824761"
---
# <a name="phonecallstate"></a><span data-ttu-id="e7f16-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="e7f16-103">PhoneCallState</span></span>

<span data-ttu-id="e7f16-104">O elemento **PhoneCallState** Especifica o estado atual de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="e7f16-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="e7f16-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="e7f16-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7f16-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e7f16-106">Attributes and elements</span></span>

<span data-ttu-id="e7f16-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7f16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7f16-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7f16-108">Attributes</span></span>

<span data-ttu-id="e7f16-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7f16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7f16-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7f16-110">Child elements</span></span>

<span data-ttu-id="e7f16-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7f16-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7f16-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7f16-112">Parent elements</span></span>

|<span data-ttu-id="e7f16-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7f16-113">**Element**</span></span>|<span data-ttu-id="e7f16-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f16-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f16-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="e7f16-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="e7f16-116">Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="e7f16-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7f16-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e7f16-117">Text value</span></span>

<span data-ttu-id="e7f16-118">A tabela a seguir lista os valores possíveis para o elemento **PhoneCallState** .</span><span class="sxs-lookup"><span data-stu-id="e7f16-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="e7f16-119">**Valores de elemento PhoneCallState**</span><span class="sxs-lookup"><span data-stu-id="e7f16-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="e7f16-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e7f16-120">**Value**</span></span>|<span data-ttu-id="e7f16-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f16-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f16-122">Ocioso</span><span class="sxs-lookup"><span data-stu-id="e7f16-122">Idle</span></span>  <br/> |<span data-ttu-id="e7f16-123">Estado inicial de chamada.</span><span class="sxs-lookup"><span data-stu-id="e7f16-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="e7f16-124">Connecting</span><span class="sxs-lookup"><span data-stu-id="e7f16-124">Connecting</span></span>  <br/> |<span data-ttu-id="e7f16-125">O sistema está discando essa chamada.</span><span class="sxs-lookup"><span data-stu-id="e7f16-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="e7f16-126">Alertado</span><span class="sxs-lookup"><span data-stu-id="e7f16-126">Alerted</span></span>  <br/> |<span data-ttu-id="e7f16-127">A chamada está no estado de alerta (telefone está tocando).</span><span class="sxs-lookup"><span data-stu-id="e7f16-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="e7f16-128">Connected</span><span class="sxs-lookup"><span data-stu-id="e7f16-128">Connected</span></span>  <br/> |<span data-ttu-id="e7f16-129">A chamada está no estado conectado.</span><span class="sxs-lookup"><span data-stu-id="e7f16-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="e7f16-130">Disconnected</span><span class="sxs-lookup"><span data-stu-id="e7f16-130">Disconnected</span></span>  <br/> |<span data-ttu-id="e7f16-131">A chamada é desconectada.</span><span class="sxs-lookup"><span data-stu-id="e7f16-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="e7f16-132">Entrada</span><span class="sxs-lookup"><span data-stu-id="e7f16-132">Incoming</span></span>  <br/> |<span data-ttu-id="e7f16-133">A chamada é entrada.</span><span class="sxs-lookup"><span data-stu-id="e7f16-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="e7f16-134">Transferindo</span><span class="sxs-lookup"><span data-stu-id="e7f16-134">Transferring</span></span>  <br/> |<span data-ttu-id="e7f16-135">A chamada está sendo transferida para outro destino.</span><span class="sxs-lookup"><span data-stu-id="e7f16-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="e7f16-136">Encaminhamento</span><span class="sxs-lookup"><span data-stu-id="e7f16-136">Forwarding</span></span>  <br/> |<span data-ttu-id="e7f16-137">A chamada está sendo encaminhada para outro destino.</span><span class="sxs-lookup"><span data-stu-id="e7f16-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7f16-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="e7f16-138">Remarks</span></span>

<span data-ttu-id="e7f16-139">O esquema que descreve este elemento está localizado no diretório /ews/ do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e7f16-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7f16-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e7f16-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7f16-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7f16-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7f16-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7f16-142">Schema Name</span></span>  <br/> |<span data-ttu-id="e7f16-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e7f16-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7f16-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7f16-144">Validation File</span></span>  <br/> |<span data-ttu-id="e7f16-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7f16-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7f16-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e7f16-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="e7f16-147">False</span><span class="sxs-lookup"><span data-stu-id="e7f16-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7f16-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="e7f16-148">See also</span></span>



- [<span data-ttu-id="e7f16-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7f16-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

