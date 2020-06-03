---
title: ErrorSubscriptionIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrorSubscriptionIds
api_type:
- schema
ms.assetid: e64e76ff-4d98-4082-9acc-a1114ae45f44
description: O elemento ErrorSubscriptionIds contém uma matriz de IDs de assinatura inválidas.
ms.openlocfilehash: bdc5c86560800464d677a9043607bed3f7872e32
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526183"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="8f0ad-103">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="8f0ad-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="8f0ad-104">O elemento **ErrorSubscriptionIds** contém uma matriz de IDs de assinatura inválidas.</span><span class="sxs-lookup"><span data-stu-id="8f0ad-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="8f0ad-105">**NonEmptyArrayOfSubscriptionIdsType**</span><span class="sxs-lookup"><span data-stu-id="8f0ad-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f0ad-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8f0ad-106">Attributes and elements</span></span>

<span data-ttu-id="8f0ad-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8f0ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f0ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8f0ad-108">Attributes</span></span>

<span data-ttu-id="8f0ad-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f0ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f0ad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8f0ad-110">Child elements</span></span>

|<span data-ttu-id="8f0ad-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f0ad-111">**Element**</span></span>|<span data-ttu-id="8f0ad-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f0ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f0ad-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="8f0ad-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="8f0ad-114">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="8f0ad-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f0ad-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8f0ad-115">Parent elements</span></span>

|<span data-ttu-id="8f0ad-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f0ad-116">**Element**</span></span>|<span data-ttu-id="8f0ad-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f0ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f0ad-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8f0ad-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="8f0ad-119">Contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8f0ad-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f0ad-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8f0ad-120">Text value</span></span>

<span data-ttu-id="8f0ad-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8f0ad-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8f0ad-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f0ad-122">Remarks</span></span>

<span data-ttu-id="8f0ad-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8f0ad-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f0ad-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8f0ad-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f0ad-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="8f0ad-125">Namespace</span></span>  <br/> |<span data-ttu-id="8f0ad-126">https://schemas.microsoft.com/exchange/services/2006/messages e https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="8f0ad-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="8f0ad-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8f0ad-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8f0ad-128">Esquema de mensagens; Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8f0ad-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="8f0ad-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8f0ad-129">Validation File</span></span>  <br/> |<span data-ttu-id="8f0ad-130">Messages. xsd; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8f0ad-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f0ad-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8f0ad-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f0ad-132">False</span><span class="sxs-lookup"><span data-stu-id="8f0ad-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f0ad-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f0ad-133">See also</span></span>



[<span data-ttu-id="8f0ad-134">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="8f0ad-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="8f0ad-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f0ad-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

