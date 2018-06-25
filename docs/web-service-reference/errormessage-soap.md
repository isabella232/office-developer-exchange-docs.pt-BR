---
title: ErrorMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b84dd664-4c49-42c9-a49f-2ec4a9f7588b
description: Elemento ErrorMessage representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.
ms.openlocfilehash: 888eedc9c7cbbd1aad5cba21e76d999699c7ed02
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752098"
---
# <a name="errormessage-soap"></a><span data-ttu-id="ec2fa-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="ec2fa-104">Elemento **ErrorMessage** representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="ec2fa-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="ec2fa-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec2fa-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ec2fa-106">Attributes and elements</span></span>

<span data-ttu-id="ec2fa-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec2fa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec2fa-108">Attributes</span></span>

<span data-ttu-id="ec2fa-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec2fa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec2fa-110">Child elements</span></span>

<span data-ttu-id="ec2fa-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec2fa-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec2fa-112">Parent elements</span></span>

|<span data-ttu-id="ec2fa-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec2fa-113">**Element**</span></span>|<span data-ttu-id="ec2fa-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec2fa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec2fa-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="ec2fa-116">Representa o tipo de base para todas as respostas que são retornados pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="ec2fa-118">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="ec2fa-120">Contém a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="ec2fa-122">Contém a resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ec2fa-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-123">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="ec2fa-124">Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ec2fa-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="ec2fa-126">Representa um erro retornado ao recuperar uma configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="ec2fa-127">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="ec2fa-128">Representa uma resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec2fa-129">Text value</span><span class="sxs-lookup"><span data-stu-id="ec2fa-129">Text value</span></span>

<span data-ttu-id="ec2fa-130">O valor de texto representa a mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="ec2fa-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec2fa-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ec2fa-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec2fa-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec2fa-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ec2fa-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec2fa-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ec2fa-134">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="ec2fa-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ec2fa-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec2fa-135">Validation File</span></span>  <br/> |<span data-ttu-id="ec2fa-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec2fa-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec2fa-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ec2fa-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec2fa-138">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ec2fa-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec2fa-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="ec2fa-139">See also</span></span>



[<span data-ttu-id="ec2fa-140">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="ec2fa-141">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="ec2fa-142">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ec2fa-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

