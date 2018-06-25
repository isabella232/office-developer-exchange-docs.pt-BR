---
title: WebClientUrls (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fdfe6059-a861-4fa2-a20e-ee6ab820bee9
description: O elemento WebClientUrls representa uma configuração de usuário que contém uma coleção de elementos de WebClientUrl (SOAP).
ms.openlocfilehash: 8d5d6aec67ab183743d7aae9f5d1f303d2949cd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838057"
---
# <a name="webclienturls-soap"></a><span data-ttu-id="ce79e-103">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-103">WebClientUrls (SOAP)</span></span>

<span data-ttu-id="ce79e-104">O elemento **WebClientUrls** representa uma configuração de usuário que contém uma coleção de elementos de [WebClientUrl (SOAP)](webclienturl-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ce79e-104">The **WebClientUrls** element represents a user setting that contains a collection of [WebClientUrl (SOAP)](webclienturl-soap.md) elements.</span></span> 
  
[<span data-ttu-id="ce79e-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="ce79e-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="ce79e-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrls>
     <WebClientUrl/>
</WebClientUrls>

```

 <span data-ttu-id="ce79e-108">**WebClientUrls**</span><span class="sxs-lookup"><span data-stu-id="ce79e-108">**WebClientUrls**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce79e-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ce79e-109">Attributes and elements</span></span>

<span data-ttu-id="ce79e-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ce79e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce79e-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="ce79e-111">Attributes</span></span>

<span data-ttu-id="ce79e-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ce79e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce79e-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ce79e-113">Child elements</span></span>

|<span data-ttu-id="ce79e-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce79e-114">**Element**</span></span>|<span data-ttu-id="ce79e-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce79e-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce79e-116">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-116">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md) <br/> |<span data-ttu-id="ce79e-117">Representa uma URL de cliente do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce79e-117">Represents an Exchange client URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce79e-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ce79e-118">Parent elements</span></span>

|<span data-ttu-id="ce79e-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce79e-119">**Element**</span></span>|<span data-ttu-id="ce79e-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce79e-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce79e-121">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-121">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="ce79e-122">Representa uma resposta a uma solicitação GetUserSettings.</span><span class="sxs-lookup"><span data-stu-id="ce79e-122">Represents a response to a GetUserSettings request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="ce79e-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ce79e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce79e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce79e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ce79e-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ce79e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ce79e-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="ce79e-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ce79e-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ce79e-127">Validation File</span></span>  <br/> |<span data-ttu-id="ce79e-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce79e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce79e-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ce79e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce79e-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ce79e-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce79e-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="ce79e-131">See also</span></span>



[<span data-ttu-id="ce79e-132">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce79e-132">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)

