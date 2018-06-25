---
title: OofStatus (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: O elemento OofStatus contém um valor que indicaties o status de Unificação de mensagens de ausência temporária para o usuário que está fazendo uma solicitação do GetUMProperties operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824650"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="b49b3-103">OofStatus (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="b49b3-104">O elemento **OofStatus** contém um valor que indicaties o status de Unificação de mensagens de ausência temporária para o usuário que está fazendo uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b49b3-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="b49b3-105">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="b49b3-106">OofStatus (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="b49b3-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b49b3-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b49b3-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b49b3-108">Attributes and elements</span></span>

<span data-ttu-id="b49b3-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b49b3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b49b3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b49b3-110">Attributes</span></span>

<span data-ttu-id="b49b3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b49b3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b49b3-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b49b3-112">Child elements</span></span>

<span data-ttu-id="b49b3-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b49b3-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b49b3-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b49b3-114">Parent elements</span></span>

|<span data-ttu-id="b49b3-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b49b3-115">**Element**</span></span>|<span data-ttu-id="b49b3-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b49b3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b49b3-117">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="b49b3-118">Define uma resposta a uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b49b3-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b49b3-119">Text value</span><span class="sxs-lookup"><span data-stu-id="b49b3-119">Text value</span></span>

<span data-ttu-id="b49b3-120">Um valor booleano de texto é necessário.</span><span class="sxs-lookup"><span data-stu-id="b49b3-120">A Boolean text value is required.</span></span> <span data-ttu-id="b49b3-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="b49b3-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="b49b3-122">True</span><span class="sxs-lookup"><span data-stu-id="b49b3-122">True</span></span>
    
- <span data-ttu-id="b49b3-123">False</span><span class="sxs-lookup"><span data-stu-id="b49b3-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="b49b3-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b49b3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b49b3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b49b3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b49b3-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b49b3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b49b3-127">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b49b3-127">Messages</span></span>  <br/> |
|<span data-ttu-id="b49b3-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b49b3-128">Validation File</span></span>  <br/> |<span data-ttu-id="b49b3-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b49b3-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b49b3-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b49b3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b49b3-131">False</span><span class="sxs-lookup"><span data-stu-id="b49b3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b49b3-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="b49b3-132">See also</span></span>



[<span data-ttu-id="b49b3-133">Operação de GetUMProperties (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="b49b3-134">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="b49b3-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

