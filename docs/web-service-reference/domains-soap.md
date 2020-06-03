---
title: Domínios (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: O elemento Domains representa o conjunto de domínios que é retornado em uma operação GetDomainSettings (SOAP), os domínios que a organização tem federado em uma operação do GetFederationInformation (SOAP) ou os domínios com um relacionamento de organização, conforme retornado pela operação de GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526302"
---
# <a name="domains-soap"></a><span data-ttu-id="83a2c-103">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-103">Domains (SOAP)</span></span>

<span data-ttu-id="83a2c-104">O elemento **Domains** representa o conjunto de domínios que é retornado em uma [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), os domínios que a organização tem federado em uma [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou os domínios com um relacionamento de organização, conforme RETORNADO pela operação de [GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="83a2c-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="83a2c-105">**Domínios**</span><span class="sxs-lookup"><span data-stu-id="83a2c-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83a2c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="83a2c-106">Attributes and elements</span></span>

<span data-ttu-id="83a2c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="83a2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83a2c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="83a2c-108">Attributes</span></span>

<span data-ttu-id="83a2c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83a2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83a2c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="83a2c-110">Child elements</span></span>

|<span data-ttu-id="83a2c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83a2c-111">**Element**</span></span>|<span data-ttu-id="83a2c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83a2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83a2c-113">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="83a2c-114">Representa um único domínio.</span><span class="sxs-lookup"><span data-stu-id="83a2c-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83a2c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="83a2c-115">Parent elements</span></span>

|<span data-ttu-id="83a2c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83a2c-116">**Element**</span></span>|<span data-ttu-id="83a2c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83a2c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83a2c-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="83a2c-119">Representa uma solicitação de [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="83a2c-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="83a2c-120">Resposta (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="83a2c-121">Contém as informações de resposta da [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="83a2c-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="83a2c-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="83a2c-123">Representa uma solicitação de [operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="83a2c-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83a2c-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="83a2c-124">Text value</span></span>

<span data-ttu-id="83a2c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83a2c-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83a2c-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="83a2c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83a2c-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="83a2c-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="83a2c-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="83a2c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="83a2c-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="83a2c-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="83a2c-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="83a2c-130">Validation File</span></span>  <br/> |<span data-ttu-id="83a2c-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83a2c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83a2c-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="83a2c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="83a2c-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="83a2c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83a2c-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="83a2c-134">See also</span></span>

- [<span data-ttu-id="83a2c-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="83a2c-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83a2c-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)

