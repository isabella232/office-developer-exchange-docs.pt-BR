---
title: GetCallInfoResponse (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: O elemento de GetCallInfoResponse define uma resposta a uma solicitação do GetCallInfo operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752421"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="725a2-103">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="725a2-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="725a2-104">O elemento de **GetCallInfoResponse** define uma resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="725a2-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="725a2-105">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="725a2-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="725a2-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="725a2-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="725a2-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="725a2-107">Attributes and elements</span></span>

<span data-ttu-id="725a2-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="725a2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="725a2-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="725a2-109">Attributes</span></span>

<span data-ttu-id="725a2-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="725a2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="725a2-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="725a2-111">Child elements</span></span>

|<span data-ttu-id="725a2-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="725a2-112">**Element**</span></span>|<span data-ttu-id="725a2-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="725a2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="725a2-114">CallState</span><span class="sxs-lookup"><span data-stu-id="725a2-114">CallState</span></span>  <br/> |<span data-ttu-id="725a2-115">Contém um valor que indica o status de uma chamada para o qual a [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) informações solicitadas.</span><span class="sxs-lookup"><span data-stu-id="725a2-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="725a2-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="725a2-116">EventCause</span></span>  <br/> |<span data-ttu-id="725a2-117">Contém um valor que indica a causa de um evento para uma chamada para o qual a [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) informações solicitadas.</span><span class="sxs-lookup"><span data-stu-id="725a2-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="725a2-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="725a2-118">Parent elements</span></span>

<span data-ttu-id="725a2-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="725a2-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="725a2-120">Text value</span><span class="sxs-lookup"><span data-stu-id="725a2-120">Text value</span></span>

<span data-ttu-id="725a2-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="725a2-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="725a2-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="725a2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="725a2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="725a2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="725a2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="725a2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="725a2-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="725a2-125">Messages</span></span>  <br/> |
|<span data-ttu-id="725a2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="725a2-126">Validation File</span></span>  <br/> |<span data-ttu-id="725a2-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="725a2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="725a2-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="725a2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="725a2-129">False</span><span class="sxs-lookup"><span data-stu-id="725a2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="725a2-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="725a2-130">See also</span></span>



[<span data-ttu-id="725a2-131">Operação de GetCallInfo (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="725a2-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="725a2-132">CallState (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="725a2-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="725a2-133">EventCause (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="725a2-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

