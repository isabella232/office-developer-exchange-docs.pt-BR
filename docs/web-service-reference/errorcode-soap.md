---
title: ErrorCode (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5e5ec861-0191-4ecb-a906-47ce8ed96381
description: O elemento ErrorCode representa um código de erro retornado pelo serviço de descoberta automática.
ms.openlocfilehash: d66167e51733ffcaa3d62a985d3e03e2ac80b715
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460089"
---
# <a name="errorcode-soap"></a><span data-ttu-id="51308-103">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-103">ErrorCode (SOAP)</span></span>

<span data-ttu-id="51308-104">O elemento **ErrorCode** representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="51308-104">The **ErrorCode** element represents an error code that is returned by the Autodiscover service.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="51308-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="51308-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51308-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="51308-106">Attributes and elements</span></span>

<span data-ttu-id="51308-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="51308-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51308-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="51308-108">Attributes</span></span>

<span data-ttu-id="51308-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51308-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51308-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="51308-110">Child elements</span></span>

<span data-ttu-id="51308-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51308-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51308-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="51308-112">Parent elements</span></span>

|<span data-ttu-id="51308-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="51308-113">**Element**</span></span>|<span data-ttu-id="51308-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51308-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51308-115">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-115">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md) <br/> |<span data-ttu-id="51308-116">Representa o tipo base para todas as respostas retornadas pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="51308-116">Represents the base type for all responses that are returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="51308-117">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-117">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="51308-118">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="51308-118">Contains the requested settings for the specified domain.</span></span>  <br/> |
|[<span data-ttu-id="51308-119">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-119">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="51308-120">Contém a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="51308-120">Contains the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
|[<span data-ttu-id="51308-121">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-121">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="51308-122">Contém a resposta a uma solicitação de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="51308-122">Contains the response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="51308-123">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-123">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="51308-124">Contém a resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="51308-124">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md)request.</span></span>  <br/> |
|[<span data-ttu-id="51308-125">UserSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-125">UserSettingError (SOAP)</span></span>](usersettingerror-soap.md) <br/> |<span data-ttu-id="51308-126">Representa um erro retornado ao recuperar uma configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="51308-126">Represents an error that is returned while retrieving a user setting.</span></span>  <br/> |
|[<span data-ttu-id="51308-127">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-127">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="51308-128">Representa uma resposta a uma solicitação de [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md) para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="51308-128">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51308-129">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="51308-129">Text value</span></span>

<span data-ttu-id="51308-130">O valor de texto representa o código de erro para uma resposta de erro de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="51308-130">The text value represents the error code for an Autodiscover error response.</span></span> <span data-ttu-id="51308-131">A tabela a seguir lista os valores de texto possíveis para o elemento **ErrorCode** .</span><span class="sxs-lookup"><span data-stu-id="51308-131">The following table lists the possible text values for the **ErrorCode** element.</span></span> 
  
|<span data-ttu-id="51308-132">**Valor de texto do código de erro**</span><span class="sxs-lookup"><span data-stu-id="51308-132">**Error code text value**</span></span>|<span data-ttu-id="51308-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51308-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="51308-134">NoError</span><span class="sxs-lookup"><span data-stu-id="51308-134">NoError</span></span>  <br/> |<span data-ttu-id="51308-135">Não há erro.</span><span class="sxs-lookup"><span data-stu-id="51308-135">There was no error.</span></span>  <br/> |
|<span data-ttu-id="51308-136">RedirectAddress</span><span class="sxs-lookup"><span data-stu-id="51308-136">RedirectAddress</span></span>  <br/> |<span data-ttu-id="51308-137">O chamador deve seguir o redirecionamento de endereço de email retornado pela descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="51308-137">The caller must follow the e-mail address redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="51308-138">RedirectUrl</span><span class="sxs-lookup"><span data-stu-id="51308-138">RedirectUrl</span></span>  <br/> |<span data-ttu-id="51308-139">O chamador deve seguir o redirecionamento de URL retornado pela descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="51308-139">The caller must follow the URL redirection that was returned by Autodiscover.</span></span>  <br/> |
|<span data-ttu-id="51308-140">InvalidUser</span><span class="sxs-lookup"><span data-stu-id="51308-140">InvalidUser</span></span>  <br/> |<span data-ttu-id="51308-141">O usuário que foi passado na solicitação é inválido.</span><span class="sxs-lookup"><span data-stu-id="51308-141">The user that was passed in the request is invalid.</span></span>  <br/> |
|<span data-ttu-id="51308-142">InvalidRequest</span><span class="sxs-lookup"><span data-stu-id="51308-142">InvalidRequest</span></span>  <br/> |<span data-ttu-id="51308-143">A solicitação é inválida.</span><span class="sxs-lookup"><span data-stu-id="51308-143">The request is invalid.</span></span>  <br/> |
|<span data-ttu-id="51308-144">InvalidSetting</span><span class="sxs-lookup"><span data-stu-id="51308-144">InvalidSetting</span></span>  <br/> |<span data-ttu-id="51308-145">Uma configuração especificada é inválida.</span><span class="sxs-lookup"><span data-stu-id="51308-145">A specified setting is invalid.</span></span>  <br/> |
|<span data-ttu-id="51308-146">SettingIsNotAvailable</span><span class="sxs-lookup"><span data-stu-id="51308-146">SettingIsNotAvailable</span></span>  <br/> |<span data-ttu-id="51308-147">Uma configuração especificada não está disponível.</span><span class="sxs-lookup"><span data-stu-id="51308-147">A specified setting is not available.</span></span>  <br/> |
|<span data-ttu-id="51308-148">ServerBusy</span><span class="sxs-lookup"><span data-stu-id="51308-148">ServerBusy</span></span>  <br/> |<span data-ttu-id="51308-149">O servidor está muito ocupado para processar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="51308-149">The server is too busy to process the request.</span></span>  <br/> |
|<span data-ttu-id="51308-150">InvalidDomain</span><span class="sxs-lookup"><span data-stu-id="51308-150">InvalidDomain</span></span>  <br/> |<span data-ttu-id="51308-151">O domínio solicitado não é válido.</span><span class="sxs-lookup"><span data-stu-id="51308-151">The requested domain is not valid.</span></span>  <br/> |
|<span data-ttu-id="51308-152">Não federado</span><span class="sxs-lookup"><span data-stu-id="51308-152">NotFederated</span></span>  <br/> |<span data-ttu-id="51308-153">A organização não é federada.</span><span class="sxs-lookup"><span data-stu-id="51308-153">The organization is not federated.</span></span>  <br/> |
|<span data-ttu-id="51308-154">InternalServerError</span><span class="sxs-lookup"><span data-stu-id="51308-154">InternalServerError</span></span>  <br/> |<span data-ttu-id="51308-155">Há um erro interno no servidor.</span><span class="sxs-lookup"><span data-stu-id="51308-155">There is an internal server error.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="51308-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="51308-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51308-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="51308-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="51308-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="51308-158">Schema Name</span></span>  <br/> |<span data-ttu-id="51308-159">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="51308-159">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="51308-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="51308-160">Validation File</span></span>  <br/> |<span data-ttu-id="51308-161">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="51308-161">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51308-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="51308-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="51308-163">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="51308-163">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51308-164">Também consulte</span><span class="sxs-lookup"><span data-stu-id="51308-164">See also</span></span>



[<span data-ttu-id="51308-165">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-165">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="51308-166">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-166">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="51308-167">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51308-167">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

