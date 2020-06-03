---
title: Ação (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: O elemento Action fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529690"
---
# <a name="action-pox"></a><span data-ttu-id="d2913-103">Ação (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-103">Action (POX)</span></span>

<span data-ttu-id="d2913-104">O elemento **Action** fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2913-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="d2913-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="d2913-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="d2913-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="d2913-108">Ação (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d2913-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d2913-109">Attributes and elements</span></span>

<span data-ttu-id="d2913-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2913-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2913-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2913-111">Attributes</span></span>

<span data-ttu-id="d2913-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2913-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2913-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2913-113">Child elements</span></span>

<span data-ttu-id="d2913-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2913-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2913-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2913-115">Parent elements</span></span>

|<span data-ttu-id="d2913-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2913-116">**Element**</span></span>|<span data-ttu-id="d2913-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2913-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2913-118">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d2913-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="d2913-119">Especifica as configurações de conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2913-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2913-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d2913-120">Text value</span></span>

<span data-ttu-id="d2913-121">O valor de texto indica se outra solicitação de descoberta automática é necessária para recuperar as informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="d2913-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="d2913-122">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="d2913-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="d2913-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d2913-123">**Value**</span></span>|<span data-ttu-id="d2913-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2913-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2913-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="d2913-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="d2913-126">Se esse valor for especificado, o elemento [RedirectUrl (POX)](redirecturl-pox.md) especificará a URL do servidor de acesso para cliente a ser usada na solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="d2913-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="d2913-127">O aplicativo cliente deve parar de redirecionamento após 10 redirecionamentos.</span><span class="sxs-lookup"><span data-stu-id="d2913-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="d2913-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="d2913-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="d2913-129">Se esse valor for especificado, o elemento [RedirectAddr (POX)](redirectaddr-pox.md) especificará o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="d2913-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="d2913-130">configurações</span><span class="sxs-lookup"><span data-stu-id="d2913-130">settings</span></span>  <br/> |<span data-ttu-id="d2913-131">Se esse valor for especificado, a resposta de descoberta automática conterá as configurações que são usadas para configurar a conta.</span><span class="sxs-lookup"><span data-stu-id="d2913-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="d2913-132">A maioria das configurações será encontrada no elemento [Protocol (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d2913-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2913-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="d2913-133">See also</span></span>

- [<span data-ttu-id="d2913-134">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="d2913-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

