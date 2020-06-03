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
description: O elemento GetFederationInformationResponse contém a resposta de operação do GetFederationInformation (SOAP).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460040"
---
# <a name="getfederationinformationresponse-soap"></a><span data-ttu-id="53530-103">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-103">GetFederationInformationResponse (SOAP)</span></span>

<span data-ttu-id="53530-104">O elemento **GetFederationInformationResponse** contém a resposta de [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="53530-104">The **GetFederationInformationResponse** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span> 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
```

 <span data-ttu-id="53530-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="53530-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53530-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="53530-106">Attributes and elements</span></span>

<span data-ttu-id="53530-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="53530-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53530-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="53530-108">Attributes</span></span>

<span data-ttu-id="53530-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53530-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53530-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="53530-110">Child elements</span></span>

|<span data-ttu-id="53530-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="53530-111">**Element**</span></span>|<span data-ttu-id="53530-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="53530-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53530-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="53530-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="53530-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="53530-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="53530-116">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="53530-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="53530-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="53530-118">Define o local de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53530-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="53530-119">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-119">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="53530-120">Representa uma coleção de tokens de segurança, que contêm identificadores de serviço de token de segurança e pontos de extremidade.</span><span class="sxs-lookup"><span data-stu-id="53530-120">Represents a collection of security tokens, which contain security token service identifiers and endpoints.</span></span>  <br/> |
|[<span data-ttu-id="53530-121">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-121">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="53530-122">Representa os domínios em que as configurações para as quais são retornadas em uma operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** ou os domínios que a organização tem federado em uma operação de **GetFederationInformation** de [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="53530-122">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) **GetDomainSettings** operation or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) **GetFederationInformation** operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="53530-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="53530-123">Parent elements</span></span>

<span data-ttu-id="53530-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53530-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="53530-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="53530-125">Text value</span></span>

<span data-ttu-id="53530-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53530-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53530-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="53530-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53530-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="53530-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="53530-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="53530-129">Schema Name</span></span>  <br/> |<span data-ttu-id="53530-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="53530-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="53530-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="53530-131">Validation File</span></span>  <br/> |<span data-ttu-id="53530-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="53530-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53530-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="53530-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="53530-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="53530-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53530-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="53530-135">See also</span></span>



[<span data-ttu-id="53530-136">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="53530-136">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

