---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: O elemento RedirectAddr especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529872"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="c453d-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="c453d-104">O elemento **RedirectAddr** especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="c453d-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="c453d-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c453d-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c453d-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c453d-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c453d-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c453d-109">Attributes and elements</span></span>

<span data-ttu-id="c453d-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c453d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c453d-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="c453d-111">Attributes</span></span>

<span data-ttu-id="c453d-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c453d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c453d-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c453d-113">Child elements</span></span>

<span data-ttu-id="c453d-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c453d-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c453d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c453d-115">Parent elements</span></span>

|<span data-ttu-id="c453d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c453d-116">**Element**</span></span>|<span data-ttu-id="c453d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c453d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c453d-118">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="c453d-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="c453d-119">Especifica as configurações de conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="c453d-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c453d-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c453d-120">Text value</span></span>

<span data-ttu-id="c453d-121">O valor de texto representa o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="c453d-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c453d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c453d-122">Remarks</span></span>

<span data-ttu-id="c453d-123">Se esse elemento estiver presente na resposta de descoberta automática, faça outra solicitação usando o valor de texto do elemento **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="c453d-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c453d-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="c453d-124">See also</span></span>



[<span data-ttu-id="c453d-125">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="c453d-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

