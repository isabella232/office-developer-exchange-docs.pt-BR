---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: O elemento DomainRequired indica se o domínio é necessário para autenticação.
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751914"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="ad0a8-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-103">DomainRequired (POX)</span></span>

<span data-ttu-id="ad0a8-104">O elemento **DomainRequired** indica se o domínio é necessário para autenticação.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="ad0a8-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="ad0a8-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="ad0a8-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="ad0a8-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="ad0a8-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ad0a8-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ad0a8-110">Attributes and elements</span></span>

<span data-ttu-id="ad0a8-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad0a8-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="ad0a8-112">Attributes</span></span>

<span data-ttu-id="ad0a8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad0a8-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ad0a8-114">Child elements</span></span>

<span data-ttu-id="ad0a8-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad0a8-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ad0a8-116">Parent elements</span></span>

|<span data-ttu-id="ad0a8-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ad0a8-117">**Element**</span></span>|<span data-ttu-id="ad0a8-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ad0a8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad0a8-119">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="ad0a8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ad0a8-120">Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad0a8-121">Text value</span><span class="sxs-lookup"><span data-stu-id="ad0a8-121">Text value</span></span>

<span data-ttu-id="ad0a8-122">O valor de texto indica se o domínio é necessário para autenticação.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="ad0a8-123">Os valores possíveis são **Ativar** e **Desativar**.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="ad0a8-124">Se o valor estiver **ligado**, a solicitação subsequente deve conter o domínio da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad0a8-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="ad0a8-125">Remarks</span></span>

<span data-ttu-id="ad0a8-126">Se o domínio não for especificado no elemento [LoginName POX ()](loginname-pox.md) ou o elemento **LoginName** não foi especificado, o usuário deve digitar o domínio antes de autenticação terá êxito.</span><span class="sxs-lookup"><span data-stu-id="ad0a8-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ad0a8-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="ad0a8-127">See also</span></span>

- [<span data-ttu-id="ad0a8-128">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="ad0a8-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

