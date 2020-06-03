---
title: Resposta (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4c2bcdeb-95ce-4ffa-bd83-118af53b534f
description: O elemento Response contém a resposta a uma operação GetUserSettings (SOAP), GetDomainSettings Operation (SOAP) ou uma solicitação de operação do GetFederationInformation (SOAP).
ms.openlocfilehash: 90cb29dd4ce4026211a5b592f149c8190dc81d29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456413"
---
# <a name="response-soap"></a><span data-ttu-id="33ec4-103">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-103">Response (SOAP)</span></span>

<span data-ttu-id="33ec4-104">O elemento **Response** contém a resposta a uma [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings Operation (SOAP)](getdomainsettings-operation-soap.md)ou uma solicitação de [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="33ec4-104">The **Response** element contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md), [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</Response>
```

 <span data-ttu-id="33ec4-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="33ec4-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33ec4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="33ec4-106">Attributes and elements</span></span>

<span data-ttu-id="33ec4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="33ec4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33ec4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="33ec4-108">Attributes</span></span>

<span data-ttu-id="33ec4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33ec4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33ec4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="33ec4-110">Child elements</span></span>

|<span data-ttu-id="33ec4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="33ec4-111">**Element**</span></span>|<span data-ttu-id="33ec4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33ec4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33ec4-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="33ec4-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33ec4-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="33ec4-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="33ec4-116">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33ec4-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="33ec4-117">Userresponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="33ec4-118">Contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="33ec4-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33ec4-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="33ec4-119">Parent elements</span></span>

|<span data-ttu-id="33ec4-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="33ec4-120">**Element**</span></span>|<span data-ttu-id="33ec4-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="33ec4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33ec4-122">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-122">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="33ec4-123">Define uma resposta a um [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span><span class="sxs-lookup"><span data-stu-id="33ec4-123">Defines a response to a [GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md)</span></span> <br/> |
|[<span data-ttu-id="33ec4-124">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-124">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="33ec4-125">Define uma resposta a um [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="33ec4-125">Defines a response to a [GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="33ec4-126">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-126">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="33ec4-127">Define uma resposta a um [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span><span class="sxs-lookup"><span data-stu-id="33ec4-127">Defines a response to a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33ec4-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="33ec4-128">Text value</span></span>

<span data-ttu-id="33ec4-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33ec4-129">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33ec4-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="33ec4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33ec4-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="33ec4-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="33ec4-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="33ec4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="33ec4-133">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33ec4-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="33ec4-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="33ec4-134">Validation File</span></span>  <br/> |<span data-ttu-id="33ec4-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33ec4-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33ec4-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="33ec4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="33ec4-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="33ec4-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33ec4-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="33ec4-138">See also</span></span>



[<span data-ttu-id="33ec4-139">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="33ec4-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)


[<span data-ttu-id="33ec4-140">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="33ec4-140">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="33ec4-141">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="33ec4-141">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

