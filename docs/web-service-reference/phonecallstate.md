---
title: Chamada do telefonema
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
description: O elemento callstate especifica o estado atual de uma chamada telefônica.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468527"
---
# <a name="phonecallstate"></a><span data-ttu-id="2ce3d-103">Chamada do telefonema</span><span class="sxs-lookup"><span data-stu-id="2ce3d-103">PhoneCallState</span></span>

<span data-ttu-id="2ce3d-104">O **elemento** callstate especifica o estado atual de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="2ce3d-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ce3d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2ce3d-106">Attributes and elements</span></span>

<span data-ttu-id="2ce3d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ce3d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2ce3d-108">Attributes</span></span>

<span data-ttu-id="2ce3d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ce3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ce3d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2ce3d-110">Child elements</span></span>

<span data-ttu-id="2ce3d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ce3d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2ce3d-112">Parent elements</span></span>

|<span data-ttu-id="2ce3d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-113">**Element**</span></span>|<span data-ttu-id="2ce3d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ce3d-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="2ce3d-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="2ce3d-116">Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ce3d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2ce3d-117">Text value</span></span>

<span data-ttu-id="2ce3d-118">A tabela a seguir lista os valores possíveis para o elemento de **chamada de chamada** .</span><span class="sxs-lookup"><span data-stu-id="2ce3d-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="2ce3d-119">**Valores do elemento de chamada do telefonema**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="2ce3d-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-120">**Value**</span></span>|<span data-ttu-id="2ce3d-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2ce3d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2ce3d-122">Estado</span><span class="sxs-lookup"><span data-stu-id="2ce3d-122">Idle</span></span>  <br/> |<span data-ttu-id="2ce3d-123">Estado de chamada inicial.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-124">Connecting</span><span class="sxs-lookup"><span data-stu-id="2ce3d-124">Connecting</span></span>  <br/> |<span data-ttu-id="2ce3d-125">O sistema está discando esta chamada.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-126">Alertado</span><span class="sxs-lookup"><span data-stu-id="2ce3d-126">Alerted</span></span>  <br/> |<span data-ttu-id="2ce3d-127">A chamada está em estado de alerta (o telefone está tocando).</span><span class="sxs-lookup"><span data-stu-id="2ce3d-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="2ce3d-128">Conectado</span><span class="sxs-lookup"><span data-stu-id="2ce3d-128">Connected</span></span>  <br/> |<span data-ttu-id="2ce3d-129">A chamada está no estado conectado.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-130">Disconnected</span><span class="sxs-lookup"><span data-stu-id="2ce3d-130">Disconnected</span></span>  <br/> |<span data-ttu-id="2ce3d-131">A chamada é desconectada.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-132">Electrónico</span><span class="sxs-lookup"><span data-stu-id="2ce3d-132">Incoming</span></span>  <br/> |<span data-ttu-id="2ce3d-133">A chamada é de entrada.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-134">Transfer</span><span class="sxs-lookup"><span data-stu-id="2ce3d-134">Transferring</span></span>  <br/> |<span data-ttu-id="2ce3d-135">A chamada está sendo transferida para outro destino.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="2ce3d-136">Encaminhamento</span><span class="sxs-lookup"><span data-stu-id="2ce3d-136">Forwarding</span></span>  <br/> |<span data-ttu-id="2ce3d-137">A chamada está sendo encaminhada para outro destino.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2ce3d-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="2ce3d-138">Remarks</span></span>

<span data-ttu-id="2ce3d-139">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2ce3d-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ce3d-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2ce3d-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ce3d-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="2ce3d-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ce3d-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2ce3d-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2ce3d-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2ce3d-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ce3d-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2ce3d-144">Validation File</span></span>  <br/> |<span data-ttu-id="2ce3d-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2ce3d-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ce3d-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2ce3d-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ce3d-147">False</span><span class="sxs-lookup"><span data-stu-id="2ce3d-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ce3d-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="2ce3d-148">See also</span></span>



- [<span data-ttu-id="2ce3d-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2ce3d-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

