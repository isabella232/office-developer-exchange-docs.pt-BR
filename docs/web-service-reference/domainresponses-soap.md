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
description: O elemento DomainResponses contém uma matriz de respostas para cada configuração de domínio solicitada.
ms.openlocfilehash: 2c76b9691fe88657a65130ef6829e5af64380d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526316"
---
# <a name="domainresponses-soap"></a><span data-ttu-id="71b04-103">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71b04-103">DomainResponses (SOAP)</span></span>

<span data-ttu-id="71b04-104">O elemento **DomainResponses** contém uma matriz de respostas para cada configuração de domínio solicitada.</span><span class="sxs-lookup"><span data-stu-id="71b04-104">The **DomainResponses** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 <span data-ttu-id="71b04-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="71b04-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71b04-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="71b04-106">Attributes and elements</span></span>

<span data-ttu-id="71b04-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="71b04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71b04-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="71b04-108">Attributes</span></span>

<span data-ttu-id="71b04-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71b04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71b04-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="71b04-110">Child elements</span></span>

|<span data-ttu-id="71b04-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71b04-111">**Element**</span></span>|<span data-ttu-id="71b04-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71b04-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71b04-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71b04-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="71b04-114">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="71b04-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71b04-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="71b04-115">Parent elements</span></span>

|<span data-ttu-id="71b04-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71b04-116">**Element**</span></span>|<span data-ttu-id="71b04-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71b04-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71b04-118">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71b04-118">GetDomainSettingsResponse (SOAP)</span></span>](getdomainsettingsresponse-soap.md) <br/> |<span data-ttu-id="71b04-119">Representa a resposta a uma solicitação de [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio e retorna as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="71b04-119">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request for a domain, and returns the domain settings.</span></span>  <br/> |
|[<span data-ttu-id="71b04-120">Resposta (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71b04-120">Response (GetDomainSettings) (SOAP)</span></span>](response-getdomainsettingssoap.md) <br/> |<span data-ttu-id="71b04-121">Representa a resposta a uma chamada de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) para um domínio individual.</span><span class="sxs-lookup"><span data-stu-id="71b04-121">Represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) call for an individual domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71b04-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="71b04-122">Text value</span></span>

<span data-ttu-id="71b04-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71b04-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71b04-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="71b04-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71b04-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="71b04-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="71b04-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="71b04-126">Schema Name</span></span>  <br/> |<span data-ttu-id="71b04-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="71b04-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="71b04-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="71b04-128">Validation File</span></span>  <br/> |<span data-ttu-id="71b04-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="71b04-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71b04-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="71b04-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="71b04-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="71b04-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71b04-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="71b04-132">See also</span></span>

- [<span data-ttu-id="71b04-133">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71b04-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

