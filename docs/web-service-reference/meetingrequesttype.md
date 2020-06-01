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
description: O elemento MeetingRequestType descreve o tipo da solicitação de reunião.
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465783"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="61d0e-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="61d0e-103">MeetingRequestType</span></span>

<span data-ttu-id="61d0e-104">O elemento **MeetingRequestType** descreve o tipo da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="61d0e-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="61d0e-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="61d0e-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61d0e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61d0e-106">Attributes and elements</span></span>

<span data-ttu-id="61d0e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61d0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61d0e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61d0e-108">Attributes</span></span>

<span data-ttu-id="61d0e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61d0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61d0e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61d0e-110">Child elements</span></span>

<span data-ttu-id="61d0e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="61d0e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61d0e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61d0e-112">Parent elements</span></span>

|<span data-ttu-id="61d0e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61d0e-113">**Element**</span></span>|<span data-ttu-id="61d0e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61d0e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61d0e-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="61d0e-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="61d0e-116">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61d0e-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="61d0e-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="61d0e-117">Text value</span></span>

<span data-ttu-id="61d0e-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61d0e-118">A text value is required.</span></span> <span data-ttu-id="61d0e-119">A tabela a seguir lista os valores de texto possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="61d0e-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="61d0e-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="61d0e-120">**Value**</span></span>|<span data-ttu-id="61d0e-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61d0e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61d0e-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="61d0e-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="61d0e-123">Identifica a solicitação de reunião como uma atualização completa para uma solicitação existente.</span><span class="sxs-lookup"><span data-stu-id="61d0e-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="61d0e-124">Uma atualização completa atualizou o tempo e o conteúdo informativo.</span><span class="sxs-lookup"><span data-stu-id="61d0e-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="61d0e-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="61d0e-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="61d0e-126">Identifica a solicitação de reunião como somente com conteúdo atualizado de informações.</span><span class="sxs-lookup"><span data-stu-id="61d0e-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="61d0e-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="61d0e-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="61d0e-128">Identifica a solicitação de reunião como uma nova solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="61d0e-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="61d0e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61d0e-129">None</span></span>  <br/> |<span data-ttu-id="61d0e-130">Indica que o tipo de solicitação de reunião não está definido.</span><span class="sxs-lookup"><span data-stu-id="61d0e-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="61d0e-131">Atualizados</span><span class="sxs-lookup"><span data-stu-id="61d0e-131">Outdated</span></span>  <br/> |<span data-ttu-id="61d0e-132">Identifica a solicitação de reunião como desatualizada.</span><span class="sxs-lookup"><span data-stu-id="61d0e-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="61d0e-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="61d0e-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="61d0e-134">Indica que a solicitação de reunião pertence a uma entidade de segurança que encaminhou mensagens de reunião para um representante e tem suas cópias marcadas como informativas.</span><span class="sxs-lookup"><span data-stu-id="61d0e-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="61d0e-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="61d0e-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="61d0e-136">Identifica a solicitação de reunião como uma atualização silenciosa para uma reunião existente.</span><span class="sxs-lookup"><span data-stu-id="61d0e-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61d0e-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="61d0e-137">Remarks</span></span>

<span data-ttu-id="61d0e-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="61d0e-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61d0e-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61d0e-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61d0e-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="61d0e-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61d0e-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61d0e-141">Schema Name</span></span>  <br/> |<span data-ttu-id="61d0e-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="61d0e-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="61d0e-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61d0e-143">Validation File</span></span>  <br/> |<span data-ttu-id="61d0e-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61d0e-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61d0e-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="61d0e-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="61d0e-146">False</span><span class="sxs-lookup"><span data-stu-id="61d0e-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61d0e-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="61d0e-147">See also</span></span>



- [<span data-ttu-id="61d0e-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="61d0e-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

