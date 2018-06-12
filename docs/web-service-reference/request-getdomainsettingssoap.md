---
title: Solicitação (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: O elemento de solicitação contém uma solicitação para retornar as configurações de domínio.
ms.openlocfilehash: 71a6072d476fd665dad8b0c0fe388a40db56e059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825135"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="d3332-103">Solicitação (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3332-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="d3332-104">O elemento de **solicitação** contém uma solicitação para retornar as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="d3332-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="d3332-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="d3332-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3332-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d3332-106">Attributes and elements</span></span>

<span data-ttu-id="d3332-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d3332-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3332-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d3332-108">Attributes</span></span>

<span data-ttu-id="d3332-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3332-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3332-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d3332-110">Child elements</span></span>

|<span data-ttu-id="d3332-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d3332-111">**Element**</span></span>|<span data-ttu-id="d3332-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3332-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3332-113">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3332-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d3332-114">Representa os domínios que as configurações para o qual são retornadas em uma [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou os domínios que a organização tem federados em uma [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d3332-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="d3332-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3332-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="d3332-116">Contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="d3332-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3332-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d3332-117">Parent elements</span></span>

|<span data-ttu-id="d3332-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d3332-118">**Element**</span></span>|<span data-ttu-id="d3332-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d3332-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3332-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3332-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="d3332-121">Representa uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d3332-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3332-122">Text value</span><span class="sxs-lookup"><span data-stu-id="d3332-122">Text value</span></span>

<span data-ttu-id="d3332-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d3332-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3332-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d3332-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3332-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d3332-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d3332-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d3332-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d3332-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d3332-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d3332-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d3332-128">Validation File</span></span>  <br/> |<span data-ttu-id="d3332-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3332-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3332-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d3332-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3332-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d3332-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3332-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="d3332-132">See also</span></span>



[<span data-ttu-id="d3332-133">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3332-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

