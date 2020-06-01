---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: O elemento SPA indica se a autenticação de senha segura (SPA) é necessária.
ms.openlocfilehash: cf57b3a6046b1b9b030b7cae81381189eee92c1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467638"
---
# <a name="spa-pox"></a><span data-ttu-id="4eb1f-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-103">SPA (POX)</span></span>

<span data-ttu-id="4eb1f-104">O elemento **Spa** indica se a autenticação de senha segura (Spa) é necessária.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="4eb1f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4eb1f-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4eb1f-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4eb1f-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="4eb1f-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4eb1f-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4eb1f-110">Attributes and elements</span></span>

<span data-ttu-id="4eb1f-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4eb1f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="4eb1f-112">Attributes</span></span>

<span data-ttu-id="4eb1f-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4eb1f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4eb1f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4eb1f-114">Child elements</span></span>

<span data-ttu-id="4eb1f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4eb1f-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4eb1f-116">Parent elements</span></span>

|<span data-ttu-id="4eb1f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4eb1f-117">**Element**</span></span>|<span data-ttu-id="4eb1f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4eb1f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4eb1f-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4eb1f-120">Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4eb1f-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4eb1f-121">Text value</span></span>

<span data-ttu-id="4eb1f-122">O valor de texto indica se a SPA é necessária.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="4eb1f-123">Se o valor do texto estiver **ativado**, o Spa será obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4eb1f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="4eb1f-124">Remarks</span></span>

<span data-ttu-id="4eb1f-125">Se esse elemento não estiver presente, o valor padrão será definido como **ativado**.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4eb1f-126">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4eb1f-126">See also</span></span>



[<span data-ttu-id="4eb1f-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="4eb1f-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

