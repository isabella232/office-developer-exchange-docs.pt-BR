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
description: O elemento de domínios representa a coleção de domínio que é retornada em uma operação de GetDomainSettings (SOAP), os domínios que a organização tem federados em uma operação de GetFederationInformation (SOAP) ou os domínios com um relacionamento de organização como retornado por operação GetOrganizationRelationshipSettings (SOAP).
ms.openlocfilehash: 7a21a3a09516de2d1c38021ca3ccd2161d9cdd1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751924"
---
# <a name="domains-soap"></a><span data-ttu-id="eb63a-103">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-103">Domains (SOAP)</span></span>

<span data-ttu-id="eb63a-104">O elemento de **domínios** representa a coleção de domínio que é retornada em uma [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), os domínios que a organização tem federados em uma [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou os domínios com uma relacionamento de organização conforme retornado pela [operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="eb63a-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="eb63a-105">**Domínios**</span><span class="sxs-lookup"><span data-stu-id="eb63a-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb63a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eb63a-106">Attributes and elements</span></span>

<span data-ttu-id="eb63a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb63a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb63a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb63a-108">Attributes</span></span>

<span data-ttu-id="eb63a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb63a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb63a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb63a-110">Child elements</span></span>

|<span data-ttu-id="eb63a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb63a-111">**Element**</span></span>|<span data-ttu-id="eb63a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb63a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb63a-113">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="eb63a-114">Representa um único domínio.</span><span class="sxs-lookup"><span data-stu-id="eb63a-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb63a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb63a-115">Parent elements</span></span>

|<span data-ttu-id="eb63a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb63a-116">**Element**</span></span>|<span data-ttu-id="eb63a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb63a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb63a-118">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="eb63a-119">Representa uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="eb63a-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="eb63a-120">Resposta (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="eb63a-121">Contém as informações de resposta [GetFederationInformation operação (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="eb63a-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="eb63a-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="eb63a-123">Representa uma solicitação de [operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="eb63a-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb63a-124">Text value</span><span class="sxs-lookup"><span data-stu-id="eb63a-124">Text value</span></span>

<span data-ttu-id="eb63a-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb63a-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb63a-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eb63a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb63a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb63a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="eb63a-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb63a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="eb63a-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="eb63a-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="eb63a-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb63a-130">Validation File</span></span>  <br/> |<span data-ttu-id="eb63a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eb63a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb63a-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eb63a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb63a-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="eb63a-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb63a-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="eb63a-134">See also</span></span>

- [<span data-ttu-id="eb63a-135">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="eb63a-136">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eb63a-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)

