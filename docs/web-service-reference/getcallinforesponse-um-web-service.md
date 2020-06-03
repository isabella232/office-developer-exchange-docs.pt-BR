---
title: GetCallInfoResponse (serviço Web da UM)
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
description: O elemento GetCallInfoResponse define uma resposta a uma solicitação de operação GetCallInfo (serviço Web da UM).
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461202"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="04501-103">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="04501-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="04501-104">O elemento **GetCallInfoResponse** define uma resposta a uma solicitação de [operação GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="04501-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="04501-105">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="04501-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="04501-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="04501-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04501-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="04501-107">Attributes and elements</span></span>

<span data-ttu-id="04501-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="04501-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04501-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="04501-109">Attributes</span></span>

<span data-ttu-id="04501-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04501-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04501-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="04501-111">Child elements</span></span>

|<span data-ttu-id="04501-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04501-112">**Element**</span></span>|<span data-ttu-id="04501-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04501-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04501-114">Callstate</span><span class="sxs-lookup"><span data-stu-id="04501-114">CallState</span></span>  <br/> |<span data-ttu-id="04501-115">Contém um valor que indica o status de uma chamada para a qual a [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) solicitou informações.</span><span class="sxs-lookup"><span data-stu-id="04501-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="04501-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="04501-116">EventCause</span></span>  <br/> |<span data-ttu-id="04501-117">Contém um valor que indica a causa de um evento para uma chamada para a qual a [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) solicitou informações.</span><span class="sxs-lookup"><span data-stu-id="04501-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04501-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="04501-118">Parent elements</span></span>

<span data-ttu-id="04501-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04501-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="04501-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="04501-120">Text value</span></span>

<span data-ttu-id="04501-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04501-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04501-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="04501-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04501-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="04501-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04501-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="04501-124">Schema Name</span></span>  <br/> |<span data-ttu-id="04501-125">Mensagens</span><span class="sxs-lookup"><span data-stu-id="04501-125">Messages</span></span>  <br/> |
|<span data-ttu-id="04501-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="04501-126">Validation File</span></span>  <br/> |<span data-ttu-id="04501-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04501-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04501-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="04501-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="04501-129">False</span><span class="sxs-lookup"><span data-stu-id="04501-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04501-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="04501-130">See also</span></span>



[<span data-ttu-id="04501-131">Operação GetCallInfo (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="04501-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="04501-132">Callstate (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="04501-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="04501-133">EventCause (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="04501-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

