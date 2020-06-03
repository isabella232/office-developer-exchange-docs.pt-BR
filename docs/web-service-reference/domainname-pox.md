---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: O elemento DomainName especifica o domínio do usuário.
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458422"
---
# <a name="domainname-pox"></a><span data-ttu-id="8d6c9-103">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-103">DomainName (POX)</span></span>

<span data-ttu-id="8d6c9-104">O elemento **DomainName** especifica o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d6c9-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="8d6c9-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="8d6c9-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="8d6c9-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="8d6c9-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="8d6c9-109">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8d6c9-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8d6c9-110">Attributes and elements</span></span>

<span data-ttu-id="8d6c9-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d6c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d6c9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d6c9-112">Attributes</span></span>

<span data-ttu-id="8d6c9-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d6c9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d6c9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d6c9-114">Child elements</span></span>

<span data-ttu-id="8d6c9-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d6c9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d6c9-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d6c9-116">Parent elements</span></span>

|<span data-ttu-id="8d6c9-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d6c9-117">**Element**</span></span>|<span data-ttu-id="8d6c9-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d6c9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d6c9-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8d6c9-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8d6c9-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8d6c9-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d6c9-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8d6c9-121">Text value</span></span>

<span data-ttu-id="8d6c9-122">O valor de texto especifica o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d6c9-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d6c9-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d6c9-123">Remarks</span></span>

<span data-ttu-id="8d6c9-124">Se nenhum valor for especificado, a autenticação padrão será usar o endereço de email como um formato de nome principal de usuário (UPN).</span><span class="sxs-lookup"><span data-stu-id="8d6c9-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="8d6c9-125">Por exemplo: \<Username\> @ \<Domain\> .</span><span class="sxs-lookup"><span data-stu-id="8d6c9-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8d6c9-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="8d6c9-126">See also</span></span>

- [<span data-ttu-id="8d6c9-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="8d6c9-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

