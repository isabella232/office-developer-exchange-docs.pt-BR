---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: O elemento TokenIssuer especifica o URI (SOAP) e o ponto de extremidade (SOAP) para o serviço de token de segurança.
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526323"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="37d9f-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37d9f-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="37d9f-104">O elemento **TokenIssuer** especifica o [URI (SOAP)](uri-soap.md) e o [ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="37d9f-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="37d9f-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="37d9f-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37d9f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="37d9f-106">Attributes and elements</span></span>

<span data-ttu-id="37d9f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="37d9f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37d9f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="37d9f-108">Attributes</span></span>

<span data-ttu-id="37d9f-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="37d9f-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37d9f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="37d9f-110">Child elements</span></span>

|<span data-ttu-id="37d9f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37d9f-111">**Element**</span></span>|<span data-ttu-id="37d9f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37d9f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37d9f-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37d9f-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="37d9f-114">O URI do serviço de token de segurança que emitiu o token de segurança.</span><span class="sxs-lookup"><span data-stu-id="37d9f-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="37d9f-115">Ponto de extremidade (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37d9f-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="37d9f-116">O URI do ponto de extremidade do serviço Web.</span><span class="sxs-lookup"><span data-stu-id="37d9f-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37d9f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="37d9f-117">Parent elements</span></span>

|<span data-ttu-id="37d9f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="37d9f-118">**Element**</span></span>|<span data-ttu-id="37d9f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="37d9f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37d9f-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="37d9f-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="37d9f-121">Representa uma coleção de URI de serviço de token de segurança [(SOAP)](uri-soap.md) e [ponto de extremidade (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="37d9f-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="37d9f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="37d9f-122">Remarks</span></span>

<span data-ttu-id="37d9f-123">Use o elemento **TokenIssuer** para especificar o serviço de token de segurança ao usar tokens de segurança.</span><span class="sxs-lookup"><span data-stu-id="37d9f-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="37d9f-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="37d9f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37d9f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="37d9f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="37d9f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="37d9f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="37d9f-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="37d9f-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="37d9f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="37d9f-128">Validation File</span></span>  <br/> |<span data-ttu-id="37d9f-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="37d9f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37d9f-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="37d9f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="37d9f-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="37d9f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37d9f-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="37d9f-132">See also</span></span>



[<span data-ttu-id="37d9f-133">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="37d9f-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="37d9f-134">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="37d9f-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

