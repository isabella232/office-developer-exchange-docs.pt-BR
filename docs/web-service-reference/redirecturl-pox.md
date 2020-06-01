---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: O elemento RedirectUrl contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática.
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468086"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="d6e88-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="d6e88-104">O elemento **RedirectUrl** contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d6e88-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="d6e88-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d6e88-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d6e88-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d6e88-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d6e88-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d6e88-109">Attributes and elements</span></span>

<span data-ttu-id="d6e88-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d6e88-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6e88-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="d6e88-111">Attributes</span></span>

<span data-ttu-id="d6e88-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6e88-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6e88-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d6e88-113">Child elements</span></span>

<span data-ttu-id="d6e88-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d6e88-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6e88-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d6e88-115">Parent elements</span></span>

|<span data-ttu-id="d6e88-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6e88-116">**Element**</span></span>|<span data-ttu-id="d6e88-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6e88-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6e88-118">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d6e88-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="d6e88-119">Especifica as configurações de conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="d6e88-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6e88-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d6e88-120">Text value</span></span>

<span data-ttu-id="d6e88-121">O valor de texto representa a URL do servidor de acesso para cliente que deve ser usado para obter as configurações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="d6e88-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d6e88-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6e88-122">Remarks</span></span>

<span data-ttu-id="d6e88-123">O aplicativo cliente deve parar de redirecionamento após 10 redirecionamentos.</span><span class="sxs-lookup"><span data-stu-id="d6e88-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d6e88-124">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d6e88-124">See also</span></span>



[<span data-ttu-id="d6e88-125">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="d6e88-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

