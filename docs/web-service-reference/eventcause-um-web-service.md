---
title: EventCause (serviço Web da UM)
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
description: O elemento EventCause contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de operação do GetCallInfo (serviço Web da UM).
ms.openlocfilehash: 9d49fd4b16236d0dd87889fbbd039f2e271a5968
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458674"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="1cf4a-103">EventCause (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-103">EventCause (UM web service)</span></span>

<span data-ttu-id="1cf4a-104">O elemento **EventCause** contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="1cf4a-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="1cf4a-105">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="1cf4a-106">EventCause (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="1cf4a-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="1cf4a-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cf4a-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1cf4a-108">Attributes and elements</span></span>

<span data-ttu-id="1cf4a-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1cf4a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cf4a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1cf4a-110">Attributes</span></span>

<span data-ttu-id="1cf4a-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cf4a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cf4a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1cf4a-112">Child elements</span></span>

<span data-ttu-id="1cf4a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1cf4a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1cf4a-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1cf4a-114">Parent elements</span></span>

|<span data-ttu-id="1cf4a-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1cf4a-115">**Element**</span></span>|<span data-ttu-id="1cf4a-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1cf4a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cf4a-117">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="1cf4a-118">Define uma resposta a uma solicitação de [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="1cf4a-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1cf4a-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="1cf4a-119">Text value</span></span>

<span data-ttu-id="1cf4a-120">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cf4a-120">A text value is required.</span></span> <span data-ttu-id="1cf4a-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="1cf4a-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="1cf4a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cf4a-122">None</span></span>
    
- <span data-ttu-id="1cf4a-123">Userbusy</span><span class="sxs-lookup"><span data-stu-id="1cf4a-123">UserBusy</span></span>
    
- <span data-ttu-id="1cf4a-124">NOANSWER</span><span class="sxs-lookup"><span data-stu-id="1cf4a-124">NoAnswer</span></span>
    
- <span data-ttu-id="1cf4a-125">Outros</span><span class="sxs-lookup"><span data-stu-id="1cf4a-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="1cf4a-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1cf4a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cf4a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1cf4a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cf4a-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1cf4a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1cf4a-129">Mensagens</span><span class="sxs-lookup"><span data-stu-id="1cf4a-129">Messages</span></span>  <br/> |
|<span data-ttu-id="1cf4a-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1cf4a-130">Validation File</span></span>  <br/> |<span data-ttu-id="1cf4a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cf4a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cf4a-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1cf4a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cf4a-133">False</span><span class="sxs-lookup"><span data-stu-id="1cf4a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cf4a-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="1cf4a-134">See also</span></span>



[<span data-ttu-id="1cf4a-135">Operação GetCallInfo (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="1cf4a-136">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1cf4a-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

