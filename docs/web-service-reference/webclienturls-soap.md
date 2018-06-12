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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838057"
---
# <a name="webclienturls-soap"></a><span data-ttu-id="151a6-103">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-103">WebClientUrls (SOAP)</span></span>

<span data-ttu-id="151a6-104">O elemento **WebClientUrls** representa uma configuração de usuário que contém uma coleção de elementos de [WebClientUrl (SOAP)](webclienturl-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="151a6-104">The **WebClientUrls** element represents a user setting that contains a collection of [WebClientUrl (SOAP)](webclienturl-soap.md) elements.</span></span> 
  
[<span data-ttu-id="151a6-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="151a6-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="151a6-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrls>
     <WebClientUrl/>
</WebClientUrls>

```

 <span data-ttu-id="151a6-108">**WebClientUrls**</span><span class="sxs-lookup"><span data-stu-id="151a6-108">**WebClientUrls**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="151a6-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="151a6-109">Attributes and elements</span></span>

<span data-ttu-id="151a6-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="151a6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="151a6-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="151a6-111">Attributes</span></span>

<span data-ttu-id="151a6-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="151a6-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="151a6-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="151a6-113">Child elements</span></span>

|<span data-ttu-id="151a6-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="151a6-114">**Element**</span></span>|<span data-ttu-id="151a6-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="151a6-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="151a6-116">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-116">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md) <br/> |<span data-ttu-id="151a6-117">Representa uma URL de cliente do Exchange.</span><span class="sxs-lookup"><span data-stu-id="151a6-117">Represents an Exchange client URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="151a6-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="151a6-118">Parent elements</span></span>

|<span data-ttu-id="151a6-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="151a6-119">**Element**</span></span>|<span data-ttu-id="151a6-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="151a6-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="151a6-121">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-121">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="151a6-122">Representa uma resposta a uma solicitação GetUserSettings.</span><span class="sxs-lookup"><span data-stu-id="151a6-122">Represents a response to a GetUserSettings request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="151a6-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="151a6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="151a6-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="151a6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="151a6-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="151a6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="151a6-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="151a6-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="151a6-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="151a6-127">Validation File</span></span>  <br/> |<span data-ttu-id="151a6-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="151a6-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="151a6-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="151a6-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="151a6-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="151a6-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="151a6-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="151a6-131">See also</span></span>



[<span data-ttu-id="151a6-132">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="151a6-132">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)

