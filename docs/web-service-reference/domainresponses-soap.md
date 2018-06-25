---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: O elemento DomainResponses contém uma matriz de respostas para as configurações do cada domínio solicitada.
ms.openlocfilehash: 77a3efc1605337ab436f6aea2b61a67f22e4f8ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751923"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="bb607-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb607-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="bb607-104">O elemento **DomainResponses** contém uma matriz de respostas para as configurações do cada domínio solicitada.</span><span class="sxs-lookup"><span data-stu-id="bb607-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="bb607-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="bb607-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb607-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="bb607-106">Attributes and elements</span></span>

<span data-ttu-id="bb607-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bb607-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb607-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bb607-108">Attributes</span></span>

<span data-ttu-id="bb607-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb607-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb607-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bb607-110">Child elements</span></span>

|<span data-ttu-id="bb607-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb607-111">**Element**</span></span>|<span data-ttu-id="bb607-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb607-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb607-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb607-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="bb607-114">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="bb607-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb607-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bb607-115">Parent elements</span></span>

|<span data-ttu-id="bb607-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bb607-116">**Element**</span></span>|<span data-ttu-id="bb607-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bb607-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb607-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb607-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="bb607-119">Representa a resposta a uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio e retorna as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="bb607-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="bb607-120">Resposta (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb607-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="bb607-121">Representa a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="bb607-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb607-122">Text value</span><span class="sxs-lookup"><span data-stu-id="bb607-122">Text value</span></span>

<span data-ttu-id="bb607-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bb607-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb607-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="bb607-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb607-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb607-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bb607-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bb607-126">Schema Name</span></span>  <br/> |<span data-ttu-id="bb607-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="bb607-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bb607-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bb607-128">Validation File</span></span>  <br/> |<span data-ttu-id="bb607-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bb607-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb607-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bb607-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb607-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="bb607-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb607-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="bb607-132">See also</span></span>

- [<span data-ttu-id="bb607-133">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bb607-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

