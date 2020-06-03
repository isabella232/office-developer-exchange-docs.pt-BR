---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: O elemento WebClientUrl representa a URL de um cliente da Web do Exchange.
ms.openlocfilehash: bcf9c8d4fe80de8af4c9500e5e850558a8451d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464970"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="da924-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="da924-104">O elemento **WebClientUrl** representa a URL de um cliente da Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="da924-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="da924-105">Usersetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="da924-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="da924-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="da924-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="da924-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da924-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="da924-109">Attributes and elements</span></span>

<span data-ttu-id="da924-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="da924-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da924-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="da924-111">Attributes</span></span>

<span data-ttu-id="da924-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da924-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da924-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="da924-113">Child elements</span></span>

|<span data-ttu-id="da924-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="da924-114">**Element**</span></span>|<span data-ttu-id="da924-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="da924-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da924-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="da924-117">Representa o método de autenticação a ser usado ao acessar a URL especificada.</span><span class="sxs-lookup"><span data-stu-id="da924-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="da924-118">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="da924-119">Representa o endereço da Web da URL.</span><span class="sxs-lookup"><span data-stu-id="da924-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da924-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="da924-120">Parent elements</span></span>

|<span data-ttu-id="da924-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="da924-121">**Element**</span></span>|<span data-ttu-id="da924-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="da924-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da924-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="da924-124">Representa uma configuração de usuário que contém uma coleção de elementos **WebClientUrl** .</span><span class="sxs-lookup"><span data-stu-id="da924-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="da924-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="da924-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da924-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="da924-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="da924-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="da924-127">Schema Name</span></span>  <br/> |<span data-ttu-id="da924-128">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="da924-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="da924-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="da924-129">Validation File</span></span>  <br/> |<span data-ttu-id="da924-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="da924-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da924-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="da924-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="da924-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="da924-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da924-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="da924-133">See also</span></span>



[<span data-ttu-id="da924-134">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="da924-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="da924-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

