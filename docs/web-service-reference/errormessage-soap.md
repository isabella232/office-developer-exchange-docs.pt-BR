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
description: O elemento ErrorMessage representa uma mensagem que está associada a um código de erro retornado pelo serviço de descoberta automática.
ms.openlocfilehash: 4ebaf91fe26083cf241826e1fc16ac184fddf57c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530639"
---
# <a name="errormessage-soap"></a><span data-ttu-id="f817d-103">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-103">ErrorMessage (SOAP)</span></span>

<span data-ttu-id="f817d-104">O elemento **ErrorMessage** representa uma mensagem que está associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f817d-104">The **ErrorMessage** element represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorMessage/>
```

 <span data-ttu-id="f817d-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="f817d-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f817d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f817d-106">Attributes and elements</span></span>

<span data-ttu-id="f817d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f817d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f817d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f817d-108">Attributes</span></span>

<span data-ttu-id="f817d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f817d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f817d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f817d-110">Child elements</span></span>

<span data-ttu-id="f817d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f817d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f817d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f817d-112">Parent elements</span></span>

|<span data-ttu-id="f817d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f817d-113">**Element**</span></span>|<span data-ttu-id="f817d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f817d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f817d-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="f817d-116">Representa o tipo base para todas as respostas retornadas pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f817d-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f817d-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="f817d-118">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="f817d-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="f817d-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="f817d-120">Contém a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="f817d-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="f817d-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="f817d-122">Contém a resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f817d-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f817d-123">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="f817d-124">Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="f817d-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f817d-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="f817d-126">Representa um erro retornado ao recuperar uma configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="f817d-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="f817d-127">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="f817d-128">Representa uma resposta a uma solicitação de [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="f817d-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f817d-129">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f817d-129">Text value</span></span>

<span data-ttu-id="f817d-130">O valor de texto representa a mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="f817d-130">The text value represents the error message.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f817d-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f817d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f817d-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f817d-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f817d-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f817d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f817d-134">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="f817d-134">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f817d-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f817d-135">Validation File</span></span>  <br/> |<span data-ttu-id="f817d-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f817d-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f817d-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f817d-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f817d-138">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="f817d-138">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f817d-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="f817d-139">See also</span></span>



[<span data-ttu-id="f817d-140">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-140">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="f817d-141">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-141">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="f817d-142">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f817d-142">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

