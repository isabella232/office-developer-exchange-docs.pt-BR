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
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837805"
---
# <a name="ttl-pox"></a><span data-ttu-id="8c126-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-103">TTL (POX)</span></span>

<span data-ttu-id="8c126-104">O elemento **TTL** Especifica o tempo de vida, em horas, durante o qual as configurações permanecem válidas.</span><span class="sxs-lookup"><span data-stu-id="8c126-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="8c126-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8c126-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8c126-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8c126-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8c126-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8c126-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8c126-110">Attributes and elements</span></span>

<span data-ttu-id="8c126-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8c126-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c126-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8c126-112">Attributes</span></span>

<span data-ttu-id="8c126-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c126-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c126-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8c126-114">Child elements</span></span>

<span data-ttu-id="8c126-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8c126-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c126-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8c126-116">Parent elements</span></span>

|<span data-ttu-id="8c126-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8c126-117">**Element**</span></span>|<span data-ttu-id="8c126-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8c126-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c126-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="8c126-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8c126-120">Contém as especificações para conectar um cliente para o computador do Exchange Server 2007 em que a função de servidor acesso para cliente está instalada.</span><span class="sxs-lookup"><span data-stu-id="8c126-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c126-121">Text value</span><span class="sxs-lookup"><span data-stu-id="8c126-121">Text value</span></span>

<span data-ttu-id="8c126-122">O valor de texto representa o tempo de vida, em horas, durante o qual as configurações permanecem válidas.</span><span class="sxs-lookup"><span data-stu-id="8c126-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="8c126-123">Um valor de zero indica que redescoberta não é necessária.</span><span class="sxs-lookup"><span data-stu-id="8c126-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="8c126-124">Se nenhum valor for especificado, o valor padrão para esse elemento é 1 hora.</span><span class="sxs-lookup"><span data-stu-id="8c126-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8c126-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="8c126-125">Remarks</span></span>

<span data-ttu-id="8c126-126">Após a hora em que é representada pelo elemento **TTL** decorrido, as configurações devem ser redescobertas usando uma solicitação de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="8c126-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8c126-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c126-127">See also</span></span>



[<span data-ttu-id="8c126-128">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="8c126-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

