---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: O elemento MeetingRequestType descreve o tipo de solicitação de reunião.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824432"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="8b67c-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="8b67c-103">MeetingRequestType</span></span>

<span data-ttu-id="8b67c-104">O elemento **MeetingRequestType** descreve o tipo de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="8b67c-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="8b67c-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="8b67c-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b67c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8b67c-106">Attributes and elements</span></span>

<span data-ttu-id="8b67c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8b67c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b67c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8b67c-108">Attributes</span></span>

<span data-ttu-id="8b67c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8b67c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b67c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8b67c-110">Child elements</span></span>

<span data-ttu-id="8b67c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8b67c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b67c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8b67c-112">Parent elements</span></span>

|<span data-ttu-id="8b67c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b67c-113">**Element**</span></span>|<span data-ttu-id="8b67c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b67c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b67c-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8b67c-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8b67c-116">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b67c-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b67c-117">Text value</span><span class="sxs-lookup"><span data-stu-id="8b67c-117">Text value</span></span>

<span data-ttu-id="8b67c-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="8b67c-118">A text value is required.</span></span> <span data-ttu-id="8b67c-119">A tabela a seguir lista os valores de texto possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="8b67c-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="8b67c-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="8b67c-120">**Value**</span></span>|<span data-ttu-id="8b67c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b67c-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b67c-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="8b67c-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="8b67c-123">Identifica a solicitação de reunião como uma atualização completa para uma solicitação existente.</span><span class="sxs-lookup"><span data-stu-id="8b67c-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="8b67c-124">Uma atualização completa atualizou o tempo e o conteúdo informativo.</span><span class="sxs-lookup"><span data-stu-id="8b67c-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="8b67c-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="8b67c-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="8b67c-126">Identifica a solicitação de reunião como contendo apenas atualizados conteúdo informativo.</span><span class="sxs-lookup"><span data-stu-id="8b67c-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="8b67c-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8b67c-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="8b67c-128">Identifica a solicitação de reunião como uma nova solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="8b67c-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="8b67c-129">None</span><span class="sxs-lookup"><span data-stu-id="8b67c-129">None</span></span>  <br/> |<span data-ttu-id="8b67c-130">Indica o tipo de solicitação de reunião não está definido.</span><span class="sxs-lookup"><span data-stu-id="8b67c-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="8b67c-131">Desatualizadas</span><span class="sxs-lookup"><span data-stu-id="8b67c-131">Outdated</span></span>  <br/> |<span data-ttu-id="8b67c-132">Identifica a solicitação de reunião como desatualizados.</span><span class="sxs-lookup"><span data-stu-id="8b67c-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="8b67c-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="8b67c-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="8b67c-134">Indica que a solicitação de reunião pertence a uma entidade de segurança que tem encaminhadas mensagens de reunião para um representante e tem suas cópias marcadas como informativas.</span><span class="sxs-lookup"><span data-stu-id="8b67c-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="8b67c-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="8b67c-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="8b67c-136">Identifica a solicitação de reunião como uma atualização silenciosa a uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="8b67c-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b67c-137">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8b67c-137">Remarks</span></span>

<span data-ttu-id="8b67c-138">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8b67c-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b67c-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8b67c-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b67c-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b67c-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b67c-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8b67c-141">Schema Name</span></span>  <br/> |<span data-ttu-id="8b67c-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8b67c-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b67c-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8b67c-143">Validation File</span></span>  <br/> |<span data-ttu-id="8b67c-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b67c-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b67c-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8b67c-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b67c-146">False</span><span class="sxs-lookup"><span data-stu-id="8b67c-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b67c-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="8b67c-147">See also</span></span>



- [<span data-ttu-id="8b67c-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8b67c-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

