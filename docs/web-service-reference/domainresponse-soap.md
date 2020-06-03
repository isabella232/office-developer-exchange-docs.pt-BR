---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: O elemento DomainResponse contém as configurações solicitadas para o domínio especificado.
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456959"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="deb5e-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="deb5e-104">O elemento **DomainResponse** contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="deb5e-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="deb5e-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="deb5e-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="deb5e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="deb5e-106">Attributes and elements</span></span>

<span data-ttu-id="deb5e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="deb5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="deb5e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="deb5e-108">Attributes</span></span>

<span data-ttu-id="deb5e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="deb5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="deb5e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="deb5e-110">Child elements</span></span>

|<span data-ttu-id="deb5e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="deb5e-111">**Element**</span></span>|<span data-ttu-id="deb5e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="deb5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="deb5e-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="deb5e-114">Contém informações de erro sobre as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="deb5e-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="deb5e-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="deb5e-116">Representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="deb5e-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="deb5e-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="deb5e-118">Identifica o destino do redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="deb5e-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="deb5e-119">O destino pode ser uma URL ou um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="deb5e-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="deb5e-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="deb5e-121">Especifica o código de erro associado à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="deb5e-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="deb5e-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="deb5e-123">Especifica a mensagem de erro associada à solicitação específica.</span><span class="sxs-lookup"><span data-stu-id="deb5e-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="deb5e-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="deb5e-124">Parent elements</span></span>

|<span data-ttu-id="deb5e-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="deb5e-125">**Element**</span></span>|<span data-ttu-id="deb5e-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="deb5e-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="deb5e-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="deb5e-128">Contém uma matriz de elementos **DomainResponse** .</span><span class="sxs-lookup"><span data-stu-id="deb5e-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="deb5e-129">Cada elemento **DomainResponse** contém as configurações solicitadas para o usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="deb5e-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="deb5e-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="deb5e-131">Contém as respostas de cada domínio.</span><span class="sxs-lookup"><span data-stu-id="deb5e-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="deb5e-132">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="deb5e-132">Text value</span></span>

<span data-ttu-id="deb5e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="deb5e-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="deb5e-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="deb5e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="deb5e-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="deb5e-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="deb5e-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="deb5e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="deb5e-137">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="deb5e-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="deb5e-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="deb5e-138">Validation File</span></span>  <br/> |<span data-ttu-id="deb5e-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="deb5e-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="deb5e-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="deb5e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="deb5e-141">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="deb5e-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="deb5e-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="deb5e-142">See also</span></span>

- [<span data-ttu-id="deb5e-143">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="deb5e-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

