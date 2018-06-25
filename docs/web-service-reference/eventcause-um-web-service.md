---
title: EventCause (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: O elemento EventCause contém um valor que indica a causa para um evento de chamada em resposta a uma solicitação do GetCallInfo operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752103"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="19d69-103">EventCause (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-103">EventCause (UM web service)</span></span>

<span data-ttu-id="19d69-104">O elemento **EventCause** contém um valor que indica a causa para um evento de chamada em resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="19d69-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="19d69-105">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="19d69-106">EventCause (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="19d69-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="19d69-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19d69-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="19d69-108">Attributes and elements</span></span>

<span data-ttu-id="19d69-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19d69-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19d69-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="19d69-110">Attributes</span></span>

<span data-ttu-id="19d69-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19d69-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19d69-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19d69-112">Child elements</span></span>

<span data-ttu-id="19d69-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19d69-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19d69-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19d69-114">Parent elements</span></span>

|<span data-ttu-id="19d69-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19d69-115">**Element**</span></span>|<span data-ttu-id="19d69-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19d69-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19d69-117">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="19d69-118">Define uma resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="19d69-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19d69-119">Text value</span><span class="sxs-lookup"><span data-stu-id="19d69-119">Text value</span></span>

<span data-ttu-id="19d69-120">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="19d69-120">A text value is required.</span></span> <span data-ttu-id="19d69-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="19d69-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="19d69-122">None</span><span class="sxs-lookup"><span data-stu-id="19d69-122">None</span></span>
    
- <span data-ttu-id="19d69-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="19d69-123">UserBusy</span></span>
    
- <span data-ttu-id="19d69-124">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="19d69-124">NoAnswer</span></span>
    
- <span data-ttu-id="19d69-125">Outro</span><span class="sxs-lookup"><span data-stu-id="19d69-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="19d69-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="19d69-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19d69-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="19d69-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19d69-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19d69-128">Schema Name</span></span>  <br/> |<span data-ttu-id="19d69-129">Mensagens</span><span class="sxs-lookup"><span data-stu-id="19d69-129">Messages</span></span>  <br/> |
|<span data-ttu-id="19d69-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19d69-130">Validation File</span></span>  <br/> |<span data-ttu-id="19d69-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19d69-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19d69-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="19d69-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="19d69-133">False</span><span class="sxs-lookup"><span data-stu-id="19d69-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19d69-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="19d69-134">See also</span></span>



[<span data-ttu-id="19d69-135">Operação de GetCallInfo (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="19d69-136">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="19d69-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

