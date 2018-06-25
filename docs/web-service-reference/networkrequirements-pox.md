---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: O elemento NetworkRequirements contém os critérios que são usados para determinar se o computador cliente está em uma rede que satisfaça os requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824529"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="7ab3a-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="7ab3a-104">O elemento **NetworkRequirements** contém os critérios que são usados para determinar se o computador cliente está em uma rede que satisfaça os requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="7ab3a-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="7ab3a-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="7ab3a-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="7ab3a-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="7ab3a-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7ab3a-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7ab3a-110">Attributes and elements</span></span>

<span data-ttu-id="7ab3a-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ab3a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="7ab3a-112">Attributes</span></span>

<span data-ttu-id="7ab3a-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ab3a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7ab3a-114">Child elements</span></span>

|<span data-ttu-id="7ab3a-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ab3a-115">**Element**</span></span>|<span data-ttu-id="7ab3a-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ab3a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ab3a-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="7ab3a-118">Identifica o início de uma versão 4 (IPv4) do intervalo de IP endereços que são usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="7ab3a-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="7ab3a-120">Identifica a fim de uma versão 4 (IPv4) do intervalo de IP endereços que são usados para identificar um computador na rede.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="7ab3a-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="7ab3a-122">Identifica o início de uma versão 6 (IPv6) do intervalo de IP endereços que são usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="7ab3a-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="7ab3a-124">Identifica a fim de uma versão 6 (IPv6) do intervalo de IP endereços que são usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ab3a-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7ab3a-125">Parent elements</span></span>

|<span data-ttu-id="7ab3a-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7ab3a-126">**Element**</span></span>|<span data-ttu-id="7ab3a-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7ab3a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ab3a-128">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="7ab3a-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="7ab3a-129">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ab3a-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="7ab3a-130">Remarks</span></span>

<span data-ttu-id="7ab3a-131">Se o cliente de email não corresponder os requisitos de rede, ele deve tentar outros tipos de protocolo.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="7ab3a-132">Os provedores podem fornecer um conjunto de servidores com marcas de [Protocolo (POX)](protocol-pox.md) que não exigem autenticação, mas são necessários para a rede do provedor.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="7ab3a-133">Os provedores podem listar outro conjunto de servidores que exigem autenticação, mas não precisam estar em uma rede específica.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="7ab3a-134">O elemento **NetworkRequirements** é opcional.</span><span class="sxs-lookup"><span data-stu-id="7ab3a-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7ab3a-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="7ab3a-135">See also</span></span>



[<span data-ttu-id="7ab3a-136">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="7ab3a-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

