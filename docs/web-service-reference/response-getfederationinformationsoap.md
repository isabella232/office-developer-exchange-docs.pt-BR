---
title: Resposta (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: O elemento de resposta contém as informações de resposta GetFederationInformation operação (SOAP).
ms.openlocfilehash: 946cba56d7503a0e20ec59640f4f1258c00a844e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825171"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="5d2bc-103">Resposta (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="5d2bc-104">O elemento de **resposta** contém as informações de resposta [GetFederationInformation operação (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5d2bc-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="5d2bc-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="5d2bc-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d2bc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5d2bc-106">Attributes and elements</span></span>

<span data-ttu-id="5d2bc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d2bc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d2bc-108">Attributes</span></span>

<span data-ttu-id="5d2bc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d2bc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d2bc-110">Child elements</span></span>

|<span data-ttu-id="5d2bc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d2bc-111">**Element**</span></span>|<span data-ttu-id="5d2bc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d2bc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d2bc-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="5d2bc-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="5d2bc-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="5d2bc-116">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="5d2bc-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="5d2bc-118">Define o local de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="5d2bc-119">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="5d2bc-120">Representa a coleção de domínio, as configurações para o qual são retornadas em uma [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou os domínios que a organização tem federados em uma [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="5d2bc-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d2bc-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d2bc-121">Parent elements</span></span>

|<span data-ttu-id="5d2bc-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d2bc-122">**Element**</span></span>|<span data-ttu-id="5d2bc-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d2bc-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d2bc-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="5d2bc-125">Define uma resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5d2bc-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d2bc-126">Text value</span><span class="sxs-lookup"><span data-stu-id="5d2bc-126">Text value</span></span>

<span data-ttu-id="5d2bc-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d2bc-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d2bc-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5d2bc-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d2bc-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d2bc-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5d2bc-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d2bc-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5d2bc-131">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5d2bc-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5d2bc-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d2bc-132">Validation File</span></span>  <br/> |<span data-ttu-id="5d2bc-133">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d2bc-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d2bc-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5d2bc-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d2bc-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5d2bc-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d2bc-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="5d2bc-136">See also</span></span>



[<span data-ttu-id="5d2bc-137">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5d2bc-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

