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
ms.openlocfilehash: d3d9c3bf9ad97cc0fdabf574c6505c797583838a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467211"
---
# <a name="unsubscribe"></a><span data-ttu-id="d1f4d-103">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="d1f4d-103">Unsubscribe</span></span>

<span data-ttu-id="d1f4d-104">O elemento **Unsubscribe** contém as propriedades usadas para cancelar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d1f4d-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="d1f4d-105">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="d1f4d-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="d1f4d-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="d1f4d-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1f4d-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d1f4d-107">Attributes and elements</span></span>

<span data-ttu-id="d1f4d-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1f4d-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1f4d-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1f4d-109">Attributes</span></span>

<span data-ttu-id="d1f4d-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1f4d-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1f4d-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1f4d-111">Child elements</span></span>

|<span data-ttu-id="d1f4d-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1f4d-112">**Element**</span></span>|<span data-ttu-id="d1f4d-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1f4d-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1f4d-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="d1f4d-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="d1f4d-115">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d1f4d-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1f4d-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1f4d-116">Parent elements</span></span>

<span data-ttu-id="d1f4d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1f4d-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d1f4d-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1f4d-118">Remarks</span></span>

<span data-ttu-id="d1f4d-119">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d1f4d-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1f4d-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d1f4d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1f4d-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1f4d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1f4d-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1f4d-122">Schema name</span></span>  <br/> |<span data-ttu-id="d1f4d-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d1f4d-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1f4d-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1f4d-124">Validation file</span></span>  <br/> |<span data-ttu-id="d1f4d-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d1f4d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1f4d-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d1f4d-126">Can be empty</span></span>  <br/> |<span data-ttu-id="d1f4d-127">False</span><span class="sxs-lookup"><span data-stu-id="d1f4d-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1f4d-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="d1f4d-128">See also</span></span>



[<span data-ttu-id="d1f4d-129">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="d1f4d-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d1f4d-130">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="d1f4d-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d1f4d-131">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="d1f4d-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

