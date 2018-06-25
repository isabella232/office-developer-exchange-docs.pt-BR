---
title: Resposta SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: O elemento de resposta contém a resposta a uma operação de GetUserSettings (SOAP), a operação de GetDomainSettings (SOAP) ou uma solicitação de operação (SOAP) GetFederationInformation.
ms.openlocfilehash: 240c8e1f904ad685b51c1f657b2bc18e14fd985e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825179"
---
# <a name="response-soap"></a><span data-ttu-id="9a6cc-103">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-103">Response (SOAP)</span></span>

<span data-ttu-id="9a6cc-104">O elemento de **resposta** contém a resposta a uma [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md), [a operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="9a6cc-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="9a6cc-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="9a6cc-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a6cc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9a6cc-106">Attributes and elements</span></span>

<span data-ttu-id="9a6cc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a6cc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9a6cc-108">Attributes</span></span>

<span data-ttu-id="9a6cc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a6cc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9a6cc-110">Child elements</span></span>

|<span data-ttu-id="9a6cc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9a6cc-111">**Element**</span></span>|<span data-ttu-id="9a6cc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9a6cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a6cc-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="9a6cc-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="9a6cc-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="9a6cc-116">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="9a6cc-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="9a6cc-118">Contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a6cc-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9a6cc-119">Parent elements</span></span>

|<span data-ttu-id="9a6cc-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9a6cc-120">**Element**</span></span>|<span data-ttu-id="9a6cc-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9a6cc-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a6cc-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="9a6cc-123">Define uma resposta a um [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="9a6cc-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="9a6cc-125">Define uma resposta a um [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="9a6cc-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="9a6cc-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="9a6cc-127">Define uma resposta a um [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="9a6cc-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a6cc-128">Text value</span><span class="sxs-lookup"><span data-stu-id="9a6cc-128">Text value</span></span>

<span data-ttu-id="9a6cc-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a6cc-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a6cc-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9a6cc-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a6cc-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a6cc-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9a6cc-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9a6cc-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9a6cc-133">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="9a6cc-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9a6cc-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9a6cc-134">Validation File</span></span>  <br/> |<span data-ttu-id="9a6cc-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a6cc-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a6cc-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9a6cc-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a6cc-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9a6cc-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a6cc-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="9a6cc-138">See also</span></span>



[<span data-ttu-id="9a6cc-139">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9a6cc-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="9a6cc-140">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="9a6cc-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="9a6cc-141">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9a6cc-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

