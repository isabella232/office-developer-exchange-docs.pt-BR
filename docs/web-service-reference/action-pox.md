---
title: Ação POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: O elemento Action fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752209"
---
# <a name="action-pox"></a><span data-ttu-id="213a2-103">Ação POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-103">Action (POX)</span></span>

<span data-ttu-id="213a2-104">O elemento **Action** fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="213a2-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="213a2-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="213a2-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="213a2-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="213a2-108">Ação POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="213a2-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="213a2-109">Attributes and elements</span></span>

<span data-ttu-id="213a2-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="213a2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="213a2-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="213a2-111">Attributes</span></span>

<span data-ttu-id="213a2-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="213a2-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="213a2-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="213a2-113">Child elements</span></span>

<span data-ttu-id="213a2-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="213a2-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="213a2-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="213a2-115">Parent elements</span></span>

|<span data-ttu-id="213a2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="213a2-116">**Element**</span></span>|<span data-ttu-id="213a2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="213a2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="213a2-118">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="213a2-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="213a2-119">Especifica as configurações da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="213a2-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="213a2-120">Text value</span><span class="sxs-lookup"><span data-stu-id="213a2-120">Text value</span></span>

<span data-ttu-id="213a2-121">O valor de texto representa se outra solicitação de descoberta automática é necessária recuperar informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="213a2-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="213a2-122">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="213a2-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="213a2-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="213a2-123">**Value**</span></span>|<span data-ttu-id="213a2-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="213a2-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="213a2-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="213a2-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="213a2-126">Se esse valor for especificado, o elemento [RedirectUrl POX ()](redirecturl-pox.md) especificará a URL do servidor de acesso para cliente a ser usado na solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="213a2-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="213a2-127">O aplicativo cliente deve parar redirecionando após 10 redirecionamentos.</span><span class="sxs-lookup"><span data-stu-id="213a2-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="213a2-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="213a2-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="213a2-129">Se esse valor for especificado, o elemento [RedirectAddr (POX)](redirectaddr-pox.md) especificará o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="213a2-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="213a2-130">configurações</span><span class="sxs-lookup"><span data-stu-id="213a2-130">settings</span></span>  <br/> |<span data-ttu-id="213a2-131">Se esse valor for especificado, a resposta da descoberta automática contém configurações que são usadas para configurar a conta.</span><span class="sxs-lookup"><span data-stu-id="213a2-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="213a2-132">A maioria das configurações será encontrada no elemento de [Protocolo (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="213a2-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="213a2-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="213a2-133">See also</span></span>

- [<span data-ttu-id="213a2-134">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="213a2-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

