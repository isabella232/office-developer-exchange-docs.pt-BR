---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: O elemento LegacyDN identifica a caixa de correio de um usuário por nome distinto herdado.
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824243"
---
# <a name="legacydn-pox"></a><span data-ttu-id="d8ac3-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="d8ac3-103">LegacyDN (POX)</span></span>

<span data-ttu-id="d8ac3-104">O elemento **LegacyDN** identifica a caixa de correio de um usuário por nome distinto herdado.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d8ac3-105">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d8ac3-105">Attributes and elements</span></span>

<span data-ttu-id="d8ac3-106">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8ac3-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8ac3-107">Attributes</span></span>

<span data-ttu-id="d8ac3-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8ac3-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8ac3-109">Child elements</span></span>

<span data-ttu-id="d8ac3-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8ac3-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8ac3-111">Parent elements</span></span>

|<span data-ttu-id="d8ac3-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8ac3-112">**Element**</span></span>|<span data-ttu-id="d8ac3-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8ac3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8ac3-114">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="d8ac3-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="d8ac3-115">Contém a solicitação para o serviço Descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="d8ac3-116">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="d8ac3-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="d8ac3-117">Fornece informações específicas do usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8ac3-118">Text value</span><span class="sxs-lookup"><span data-stu-id="d8ac3-118">Text value</span></span>

<span data-ttu-id="d8ac3-119">O valor de texto representa o endereço de email legados de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8ac3-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8ac3-120">Remarks</span></span>

<span data-ttu-id="d8ac3-121">O [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é um elemento alternativo para uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="d8ac3-122">Ele é usado quando não existe uma caixa de correio em um computador que está executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="d8ac3-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d8ac3-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8ac3-123">See also</span></span>

- [<span data-ttu-id="d8ac3-124">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d8ac3-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

