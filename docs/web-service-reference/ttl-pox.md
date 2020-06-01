---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: O elemento TTL especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas.
ms.openlocfilehash: 9a17cbe4e669d1afe9f3ef4a24f2a9a2889a7d52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467379"
---
# <a name="ttl-pox"></a><span data-ttu-id="bfa2b-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-103">TTL (POX)</span></span>

<span data-ttu-id="bfa2b-104">O elemento **TTL** especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="bfa2b-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="bfa2b-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="bfa2b-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="bfa2b-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="bfa2b-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="bfa2b-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bfa2b-110">Attributes and elements</span></span>

<span data-ttu-id="bfa2b-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfa2b-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="bfa2b-112">Attributes</span></span>

<span data-ttu-id="bfa2b-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfa2b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfa2b-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bfa2b-114">Child elements</span></span>

<span data-ttu-id="bfa2b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bfa2b-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bfa2b-116">Parent elements</span></span>

|<span data-ttu-id="bfa2b-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bfa2b-117">**Element**</span></span>|<span data-ttu-id="bfa2b-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bfa2b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfa2b-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="bfa2b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="bfa2b-120">Contém as especificações para conectar um cliente ao computador do Exchange Server 2007 no qual a função de servidor de acesso para cliente está instalada.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bfa2b-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bfa2b-121">Text value</span></span>

<span data-ttu-id="bfa2b-122">O valor de texto representa o tempo de vida, em horas, durante o qual as configurações permanecem válidas.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="bfa2b-123">Um valor igual a zero indica que a redescoberta não é necessária.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="bfa2b-124">Se nenhum valor for especificado, o valor padrão para esse elemento será 1 hora.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bfa2b-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="bfa2b-125">Remarks</span></span>

<span data-ttu-id="bfa2b-126">Após o tempo que é representado pelo elemento **TTL** ter decorrido, as configurações devem ser redescobertas usando uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="bfa2b-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bfa2b-127">Também consulte</span><span class="sxs-lookup"><span data-stu-id="bfa2b-127">See also</span></span>



[<span data-ttu-id="bfa2b-128">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="bfa2b-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

