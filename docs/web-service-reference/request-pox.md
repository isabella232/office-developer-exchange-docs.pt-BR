---
title: Solicitação (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: O elemento Request contém a solicitação para o serviço de descoberta automática.
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459543"
---
# <a name="request-pox"></a><span data-ttu-id="0d499-103">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-103">Request (POX)</span></span>

<span data-ttu-id="0d499-104">O elemento **Request** contém a solicitação para o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="0d499-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="0d499-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="0d499-106">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0d499-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0d499-107">Attributes and elements</span></span>

<span data-ttu-id="0d499-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d499-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d499-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d499-109">Attributes</span></span>

<span data-ttu-id="0d499-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d499-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d499-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d499-111">Child elements</span></span>

|<span data-ttu-id="0d499-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d499-112">**Element**</span></span>|<span data-ttu-id="0d499-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d499-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d499-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="0d499-115">Identifica o esquema para uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="0d499-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="0d499-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="0d499-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="0d499-117">Identifica o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0d499-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="0d499-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="0d499-119">Identifica a caixa de correio de um usuário com o nome diferenciado herdado.</span><span class="sxs-lookup"><span data-stu-id="0d499-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d499-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d499-120">Parent elements</span></span>

|<span data-ttu-id="0d499-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d499-121">**Element**</span></span>|<span data-ttu-id="0d499-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d499-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d499-123">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="0d499-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="0d499-124">O elemento raiz em uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="0d499-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d499-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d499-125">See also</span></span>

- [<span data-ttu-id="0d499-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="0d499-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

