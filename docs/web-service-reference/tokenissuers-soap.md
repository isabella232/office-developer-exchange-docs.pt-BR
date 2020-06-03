---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Os elementos TokenIssuers representam a coleção TokenIssuer (SOAP).
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457071"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="41e52-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41e52-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="41e52-104">Os elementos **TokenIssuers** representam a coleção [TokenIssuer (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="41e52-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="41e52-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="41e52-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41e52-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="41e52-106">Attributes and elements</span></span>

<span data-ttu-id="41e52-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41e52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41e52-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41e52-108">Attributes</span></span>

<span data-ttu-id="41e52-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="41e52-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41e52-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41e52-110">Child elements</span></span>

|<span data-ttu-id="41e52-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41e52-111">**Element**</span></span>|<span data-ttu-id="41e52-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e52-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41e52-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41e52-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="41e52-114">Especifica o [URI (SOAP)](uri-soap.md) e o [ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="41e52-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41e52-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41e52-115">Parent elements</span></span>

|<span data-ttu-id="41e52-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41e52-116">**Element**</span></span>|<span data-ttu-id="41e52-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e52-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41e52-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41e52-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="41e52-119">Contém a resposta de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="41e52-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41e52-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="41e52-120">Remarks</span></span>

<span data-ttu-id="41e52-121">O **TokenIssuers** representa uma coleção de elementos [TokenIssuer (SOAP)](tokenissuer-soap.md) a serem usados na descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="41e52-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="41e52-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="41e52-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41e52-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="41e52-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="41e52-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41e52-124">Schema Name</span></span>  <br/> |<span data-ttu-id="41e52-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="41e52-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="41e52-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41e52-126">Validation File</span></span>  <br/> |<span data-ttu-id="41e52-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="41e52-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41e52-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="41e52-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="41e52-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="41e52-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41e52-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="41e52-130">See also</span></span>



[<span data-ttu-id="41e52-131">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="41e52-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="41e52-132">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="41e52-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

