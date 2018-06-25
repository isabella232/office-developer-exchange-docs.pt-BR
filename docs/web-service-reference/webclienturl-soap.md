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
description: O elemento WebClientUrl representa a URL de um cliente da web do Exchange.
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838062"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="1f6ff-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="1f6ff-104">O elemento **WebClientUrl** representa a URL de um cliente da web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f6ff-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="1f6ff-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="1f6ff-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="1f6ff-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="1f6ff-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="1f6ff-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f6ff-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1f6ff-109">Attributes and elements</span></span>

<span data-ttu-id="1f6ff-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1f6ff-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f6ff-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="1f6ff-111">Attributes</span></span>

<span data-ttu-id="1f6ff-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1f6ff-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f6ff-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1f6ff-113">Child elements</span></span>

|<span data-ttu-id="1f6ff-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1f6ff-114">**Element**</span></span>|<span data-ttu-id="1f6ff-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f6ff-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f6ff-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="1f6ff-117">Representa o método de autenticação a ser usado ao acessar a URL especificada.</span><span class="sxs-lookup"><span data-stu-id="1f6ff-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="1f6ff-118">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="1f6ff-119">Representa o endereço da web para a URL.</span><span class="sxs-lookup"><span data-stu-id="1f6ff-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f6ff-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1f6ff-120">Parent elements</span></span>

|<span data-ttu-id="1f6ff-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1f6ff-121">**Element**</span></span>|<span data-ttu-id="1f6ff-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f6ff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f6ff-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="1f6ff-124">Representa uma configuração de usuário que contém uma coleção de elementos de **WebClientUrl** .</span><span class="sxs-lookup"><span data-stu-id="1f6ff-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="1f6ff-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1f6ff-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f6ff-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f6ff-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1f6ff-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1f6ff-127">Schema Name</span></span>  <br/> |<span data-ttu-id="1f6ff-128">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="1f6ff-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1f6ff-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1f6ff-129">Validation File</span></span>  <br/> |<span data-ttu-id="1f6ff-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1f6ff-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f6ff-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1f6ff-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f6ff-132">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="1f6ff-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f6ff-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="1f6ff-133">See also</span></span>



[<span data-ttu-id="1f6ff-134">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="1f6ff-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1f6ff-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

