---
title: Cancelar assinatura
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 5584db5f-553a-47ce-85fb-f9902c9990ab
description: O elemento Unsubscribe contém as propriedades usadas para cancelar uma assinatura.
ms.openlocfilehash: bab797ff74a921e3e93c993229bc6d6d289e0c5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837867"
---
# <a name="unsubscribe"></a><span data-ttu-id="d12f0-103">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="d12f0-103">Unsubscribe</span></span>

<span data-ttu-id="d12f0-104">O elemento **Unsubscribe** contém as propriedades usadas para cancelar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d12f0-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="d12f0-105">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="d12f0-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="d12f0-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="d12f0-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d12f0-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d12f0-107">Attributes and elements</span></span>

<span data-ttu-id="d12f0-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d12f0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d12f0-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="d12f0-109">Attributes</span></span>

<span data-ttu-id="d12f0-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d12f0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d12f0-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d12f0-111">Child elements</span></span>

|<span data-ttu-id="d12f0-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d12f0-112">**Element**</span></span>|<span data-ttu-id="d12f0-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d12f0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d12f0-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="d12f0-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="d12f0-115">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d12f0-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d12f0-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d12f0-116">Parent elements</span></span>

<span data-ttu-id="d12f0-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d12f0-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d12f0-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="d12f0-118">Remarks</span></span>

<span data-ttu-id="d12f0-119">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d12f0-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d12f0-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d12f0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d12f0-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="d12f0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d12f0-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d12f0-122">Schema name</span></span>  <br/> |<span data-ttu-id="d12f0-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d12f0-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d12f0-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d12f0-124">Validation file</span></span>  <br/> |<span data-ttu-id="d12f0-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d12f0-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d12f0-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d12f0-126">Can be empty</span></span>  <br/> |<span data-ttu-id="d12f0-127">False</span><span class="sxs-lookup"><span data-stu-id="d12f0-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d12f0-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="d12f0-128">See also</span></span>



[<span data-ttu-id="d12f0-129">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="d12f0-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d12f0-130">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="d12f0-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d12f0-131">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="d12f0-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

