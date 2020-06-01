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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459543"
---
# <a name="request-pox"></a><span data-ttu-id="a073e-103">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-103">Request (POX)</span></span>

<span data-ttu-id="a073e-104">O elemento **Request** contém a solicitação para o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="a073e-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="a073e-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="a073e-106">Solicitação (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-106">Request (POX)</span></span>](request-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="a073e-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a073e-107">Attributes and elements</span></span>

<span data-ttu-id="a073e-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a073e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a073e-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="a073e-109">Attributes</span></span>

<span data-ttu-id="a073e-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a073e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a073e-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a073e-111">Child elements</span></span>

|<span data-ttu-id="a073e-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a073e-112">**Element**</span></span>|<span data-ttu-id="a073e-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a073e-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a073e-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="a073e-115">Identifica o esquema para uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="a073e-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="a073e-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a073e-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="a073e-117">Identifica o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="a073e-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="a073e-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="a073e-119">Identifica a caixa de correio de um usuário com o nome diferenciado herdado.</span><span class="sxs-lookup"><span data-stu-id="a073e-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a073e-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a073e-120">Parent elements</span></span>

|<span data-ttu-id="a073e-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a073e-121">**Element**</span></span>|<span data-ttu-id="a073e-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a073e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a073e-123">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="a073e-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="a073e-124">O elemento raiz em uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="a073e-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a073e-125">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a073e-125">See also</span></span>

- [<span data-ttu-id="a073e-126">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="a073e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

