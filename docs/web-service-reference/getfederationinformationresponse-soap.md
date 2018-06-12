---
title: GetFederationInformationResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: O elemento GetFederationInformationResponse contém a resposta de operação (SOAP) GetFederationInformation.
ms.openlocfilehash: 28b002b45968278ad4c7160b4eed29721422646d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752498"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="86ddf-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="86ddf-104">O elemento **GetFederationInformationResponse** contém a resposta de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="86ddf-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="86ddf-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="86ddf-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86ddf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="86ddf-106">Attributes and elements</span></span>

<span data-ttu-id="86ddf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="86ddf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86ddf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="86ddf-108">Attributes</span></span>

<span data-ttu-id="86ddf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="86ddf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86ddf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="86ddf-110">Child elements</span></span>

|<span data-ttu-id="86ddf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="86ddf-111">**Element**</span></span>|<span data-ttu-id="86ddf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="86ddf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86ddf-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="86ddf-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="86ddf-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="86ddf-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="86ddf-116">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="86ddf-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="86ddf-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="86ddf-118">Define o local de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86ddf-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="86ddf-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="86ddf-120">Representa uma coleção de tokens de segurança, que contêm pontos de extremidade e identificadores de serviço de token de segurança.</span><span class="sxs-lookup"><span data-stu-id="86ddf-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="86ddf-121">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="86ddf-122">Representa os domínios que as configurações para o qual são retornadas em uma operação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou os domínios que a organização tem federados em uma [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) Operação **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="86ddf-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86ddf-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="86ddf-123">Parent elements</span></span>

<span data-ttu-id="86ddf-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="86ddf-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="86ddf-125">Text value</span><span class="sxs-lookup"><span data-stu-id="86ddf-125">Text value</span></span>

<span data-ttu-id="86ddf-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="86ddf-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86ddf-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="86ddf-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86ddf-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="86ddf-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="86ddf-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="86ddf-129">Schema Name</span></span>  <br/> |<span data-ttu-id="86ddf-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="86ddf-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="86ddf-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="86ddf-131">Validation File</span></span>  <br/> |<span data-ttu-id="86ddf-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="86ddf-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="86ddf-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="86ddf-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="86ddf-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="86ddf-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86ddf-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="86ddf-135">See also</span></span>



[<span data-ttu-id="86ddf-136">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="86ddf-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

