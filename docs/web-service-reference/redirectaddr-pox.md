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
description: O elemento RedirectAddr Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825020"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="afaf5-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="afaf5-104">O elemento **RedirectAddr** Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="afaf5-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="afaf5-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="afaf5-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="afaf5-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="afaf5-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="afaf5-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="afaf5-109">Attributes and elements</span></span>

<span data-ttu-id="afaf5-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="afaf5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afaf5-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="afaf5-111">Attributes</span></span>

<span data-ttu-id="afaf5-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afaf5-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afaf5-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afaf5-113">Child elements</span></span>

<span data-ttu-id="afaf5-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afaf5-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afaf5-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afaf5-115">Parent elements</span></span>

|<span data-ttu-id="afaf5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afaf5-116">**Element**</span></span>|<span data-ttu-id="afaf5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afaf5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afaf5-118">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="afaf5-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="afaf5-119">Especifica as configurações da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="afaf5-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afaf5-120">Text value</span><span class="sxs-lookup"><span data-stu-id="afaf5-120">Text value</span></span>

<span data-ttu-id="afaf5-121">O valor de texto representa o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="afaf5-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="afaf5-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="afaf5-122">Remarks</span></span>

<span data-ttu-id="afaf5-123">Se esse elemento estiver presente na resposta da descoberta automática, fazer outra solicitação usando o valor de texto do elemento **RedirectAddr** .</span><span class="sxs-lookup"><span data-stu-id="afaf5-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="afaf5-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="afaf5-124">See also</span></span>



[<span data-ttu-id="afaf5-125">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="afaf5-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

