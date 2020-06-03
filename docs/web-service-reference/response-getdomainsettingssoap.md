---
title: Resposta (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: O elemento Response representa a resposta a uma chamada GetDomainSettings para um domínio individual.
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455580"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="9432a-103">Resposta (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="9432a-104">O elemento **Response** representa a resposta a uma chamada **GetDomainSettings** para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="9432a-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="9432a-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="9432a-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9432a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9432a-106">Attributes and elements</span></span>

<span data-ttu-id="9432a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9432a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9432a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9432a-108">Attributes</span></span>

<span data-ttu-id="9432a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9432a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9432a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9432a-110">Child elements</span></span>

|<span data-ttu-id="9432a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9432a-111">**Element**</span></span>|<span data-ttu-id="9432a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9432a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9432a-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="9432a-114">Contém a resposta para cada domínio solicitado em uma solicitação **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="9432a-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="9432a-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="9432a-116">Contém o código de erro associado à resposta, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="9432a-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="9432a-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="9432a-118">Contém a mensagem de erro associada à resposta, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="9432a-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9432a-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9432a-119">Parent elements</span></span>

|<span data-ttu-id="9432a-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9432a-120">**Element**</span></span>|<span data-ttu-id="9432a-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9432a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9432a-122">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="9432a-123">Retorna ao chamador as definições de configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="9432a-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9432a-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9432a-124">Text value</span></span>

<span data-ttu-id="9432a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9432a-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9432a-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9432a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9432a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9432a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9432a-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9432a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9432a-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="9432a-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9432a-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9432a-130">Validation File</span></span>  <br/> |<span data-ttu-id="9432a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9432a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9432a-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9432a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9432a-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9432a-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9432a-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="9432a-134">See also</span></span>



[<span data-ttu-id="9432a-135">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9432a-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

