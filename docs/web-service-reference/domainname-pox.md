---
title: DomainName POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: O elemento DomainName Especifica o domínio do usuário.
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751918"
---
# <a name="domainname-pox"></a><span data-ttu-id="9a03e-103">DomainName POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-103">DomainName (POX)</span></span>

<span data-ttu-id="9a03e-104">O elemento **DomainName** Especifica o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a03e-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="9a03e-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="9a03e-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="9a03e-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="9a03e-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="9a03e-109">DomainName POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9a03e-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9a03e-110">Attributes and elements</span></span>

<span data-ttu-id="9a03e-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9a03e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a03e-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="9a03e-112">Attributes</span></span>

<span data-ttu-id="9a03e-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a03e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a03e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9a03e-114">Child elements</span></span>

<span data-ttu-id="9a03e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a03e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a03e-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9a03e-116">Parent elements</span></span>

|<span data-ttu-id="9a03e-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9a03e-117">**Element**</span></span>|<span data-ttu-id="9a03e-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9a03e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a03e-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9a03e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9a03e-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9a03e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a03e-121">Text value</span><span class="sxs-lookup"><span data-stu-id="9a03e-121">Text value</span></span>

<span data-ttu-id="9a03e-122">O valor de texto Especifica o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a03e-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a03e-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9a03e-123">Remarks</span></span>

<span data-ttu-id="9a03e-124">Se nenhum valor for especificado, a autenticação padrão é usar o endereço de email como um formato de nome principal (UPN) do usuário.</span><span class="sxs-lookup"><span data-stu-id="9a03e-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="9a03e-125">Por exemplo: \<Username\>@\<domínio\>.</span><span class="sxs-lookup"><span data-stu-id="9a03e-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9a03e-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="9a03e-126">See also</span></span>

- [<span data-ttu-id="9a03e-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="9a03e-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

