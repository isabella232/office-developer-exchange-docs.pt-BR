---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: O elemento TokenIssuer Especifica o Uri (SOAP) e o ponto de extremidade (SOAP) para o serviço de token de segurança.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837756"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="d7013-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7013-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="d7013-104">O elemento **TokenIssuer** Especifica o [Uri (SOAP)](uri-soap.md) e o [Ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="d7013-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="d7013-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="d7013-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7013-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d7013-106">Attributes and elements</span></span>

<span data-ttu-id="d7013-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7013-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7013-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7013-108">Attributes</span></span>

<span data-ttu-id="d7013-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d7013-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7013-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7013-110">Child elements</span></span>

|<span data-ttu-id="d7013-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7013-111">**Element**</span></span>|<span data-ttu-id="d7013-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7013-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7013-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7013-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="d7013-114">O URI do serviço de token de segurança que emitiu o token de segurança.</span><span class="sxs-lookup"><span data-stu-id="d7013-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="d7013-115">Ponto de extremidade (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7013-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="d7013-116">URI do ponto de extremidade do serviço web.</span><span class="sxs-lookup"><span data-stu-id="d7013-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d7013-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7013-117">Parent elements</span></span>

|<span data-ttu-id="d7013-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7013-118">**Element**</span></span>|<span data-ttu-id="d7013-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7013-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7013-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d7013-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="d7013-121">Representa uma coleção de serviço de token de segurança [Uri (SOAP)](uri-soap.md) e o [Ponto de extremidade (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d7013-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7013-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d7013-122">Remarks</span></span>

<span data-ttu-id="d7013-123">Use o elemento **TokenIssuer** para especificar o serviço de token de segurança ao usar os tokens de segurança.</span><span class="sxs-lookup"><span data-stu-id="d7013-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d7013-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d7013-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7013-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7013-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d7013-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7013-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d7013-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d7013-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d7013-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7013-128">Validation File</span></span>  <br/> |<span data-ttu-id="d7013-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7013-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7013-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d7013-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7013-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d7013-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7013-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="d7013-132">See also</span></span>



[<span data-ttu-id="d7013-133">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="d7013-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="d7013-134">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d7013-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

