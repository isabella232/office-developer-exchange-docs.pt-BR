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
description: O elemento NetworkRequirements contém os critérios usados para determinar se o computador cliente está em uma rede que atenda aos requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462721"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="f132e-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="f132e-104">O elemento **NetworkRequirements** contém os critérios usados para determinar se o computador cliente está em uma rede que atenda aos requisitos do provedor de serviços de Internet (ISP) para se conectar ao servidor.</span><span class="sxs-lookup"><span data-stu-id="f132e-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="f132e-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f132e-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f132e-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f132e-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f132e-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f132e-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f132e-110">Attributes and elements</span></span>

<span data-ttu-id="f132e-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f132e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f132e-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="f132e-112">Attributes</span></span>

<span data-ttu-id="f132e-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f132e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f132e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f132e-114">Child elements</span></span>

|<span data-ttu-id="f132e-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f132e-115">**Element**</span></span>|<span data-ttu-id="f132e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f132e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f132e-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="f132e-118">Identifica o início de um intervalo de endereços IP versão 4 (IPv4) usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="f132e-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="f132e-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="f132e-120">Identifica o final de um intervalo de endereços IP versão 4 (IPv4) usados para identificar um computador na rede.</span><span class="sxs-lookup"><span data-stu-id="f132e-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="f132e-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="f132e-122">Identifica o início de um intervalo de endereços IP versão 6 (IPv6) usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="f132e-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="f132e-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="f132e-124">Identifica o final de um intervalo de endereços IP versão 6 (IPv6) usados para identificar um computador em uma rede.</span><span class="sxs-lookup"><span data-stu-id="f132e-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f132e-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f132e-125">Parent elements</span></span>

|<span data-ttu-id="f132e-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f132e-126">**Element**</span></span>|<span data-ttu-id="f132e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f132e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f132e-128">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="f132e-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f132e-129">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f132e-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f132e-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="f132e-130">Remarks</span></span>

<span data-ttu-id="f132e-131">Se o cliente de email não corresponder aos requisitos de rede, ele deverá tentar outros tipos de protocolo.</span><span class="sxs-lookup"><span data-stu-id="f132e-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="f132e-132">Os ISPs podem fornecer um conjunto de marcas de servidor com [pox (com o protocolo)](protocol-pox.md) que não exigem autenticação, mas precisam estar na rede do provedor de Internet.</span><span class="sxs-lookup"><span data-stu-id="f132e-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="f132e-133">Os ISPs podem listar outro conjunto de servidores que exijam autenticação, mas que não precisam estar em uma rede específica.</span><span class="sxs-lookup"><span data-stu-id="f132e-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="f132e-134">O elemento **NetworkRequirements** é opcional.</span><span class="sxs-lookup"><span data-stu-id="f132e-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f132e-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="f132e-135">See also</span></span>



[<span data-ttu-id="f132e-136">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="f132e-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

