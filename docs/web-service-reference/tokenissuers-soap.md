---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Os elementos TokenIssuers representa a coleção de TokenIssuer (SOAP).
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837768"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="02219-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02219-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="02219-104">Os elementos **TokenIssuers** representa a coleção de [TokenIssuer (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="02219-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="02219-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="02219-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02219-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="02219-106">Attributes and elements</span></span>

<span data-ttu-id="02219-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="02219-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02219-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="02219-108">Attributes</span></span>

<span data-ttu-id="02219-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="02219-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02219-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="02219-110">Child elements</span></span>

|<span data-ttu-id="02219-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="02219-111">**Element**</span></span>|<span data-ttu-id="02219-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02219-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02219-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02219-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="02219-114">Especifica o [Uri (SOAP)](uri-soap.md) e o [Ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="02219-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02219-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="02219-115">Parent elements</span></span>

|<span data-ttu-id="02219-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="02219-116">**Element**</span></span>|<span data-ttu-id="02219-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02219-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02219-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="02219-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="02219-119">Contém a resposta de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="02219-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02219-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="02219-120">Remarks</span></span>

<span data-ttu-id="02219-121">O **TokenIssuers** representa uma coleção de elementos de [TokenIssuer (SOAP)](tokenissuer-soap.md) a ser usado na detecção automática.</span><span class="sxs-lookup"><span data-stu-id="02219-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="02219-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="02219-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02219-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="02219-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="02219-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="02219-124">Schema Name</span></span>  <br/> |<span data-ttu-id="02219-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="02219-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="02219-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="02219-126">Validation File</span></span>  <br/> |<span data-ttu-id="02219-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02219-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02219-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="02219-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="02219-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="02219-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02219-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="02219-130">See also</span></span>



[<span data-ttu-id="02219-131">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="02219-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="02219-132">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="02219-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

