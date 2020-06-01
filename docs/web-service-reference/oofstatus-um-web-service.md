---
title: OofStatus (serviço Web da UM)
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
description: O elemento OofStatus contém um valor que indicaties o status da Unificação de mensagens do Office para o usuário que está fazendo uma solicitação de GetUMProperties (serviço Web da UM).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460572"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="b9a15-103">OofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="b9a15-104">O elemento **OofStatus** contém um valor que indicaties o status da Unificação de mensagens do Office para o usuário que está fazendo uma solicitação de [GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a15-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="b9a15-105">GetUMPropertiesResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="b9a15-106">OofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="b9a15-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b9a15-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9a15-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b9a15-108">Attributes and elements</span></span>

<span data-ttu-id="b9a15-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9a15-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9a15-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9a15-110">Attributes</span></span>

<span data-ttu-id="b9a15-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9a15-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9a15-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9a15-112">Child elements</span></span>

<span data-ttu-id="b9a15-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9a15-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9a15-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9a15-114">Parent elements</span></span>

|<span data-ttu-id="b9a15-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9a15-115">**Element**</span></span>|<span data-ttu-id="b9a15-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9a15-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a15-117">GetUMPropertiesResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="b9a15-118">Define uma resposta a uma solicitação de [operação do GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b9a15-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b9a15-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b9a15-119">Text value</span></span>

<span data-ttu-id="b9a15-120">Um valor de texto booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="b9a15-120">A Boolean text value is required.</span></span> <span data-ttu-id="b9a15-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="b9a15-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="b9a15-122">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b9a15-122">True</span></span>
    
- <span data-ttu-id="b9a15-123">Falso</span><span class="sxs-lookup"><span data-stu-id="b9a15-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="b9a15-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b9a15-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9a15-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9a15-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9a15-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b9a15-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b9a15-127">Mensagens</span><span class="sxs-lookup"><span data-stu-id="b9a15-127">Messages</span></span>  <br/> |
|<span data-ttu-id="b9a15-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b9a15-128">Validation File</span></span>  <br/> |<span data-ttu-id="b9a15-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9a15-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9a15-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b9a15-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9a15-131">False</span><span class="sxs-lookup"><span data-stu-id="b9a15-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9a15-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="b9a15-132">See also</span></span>



[<span data-ttu-id="b9a15-133">Operação GetUMProperties (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="b9a15-134">GetUMPropertiesResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="b9a15-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

