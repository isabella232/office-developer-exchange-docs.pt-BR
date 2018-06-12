---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: O elemento DomainNames representa a coleção de nomes de domínio. O elemento DomainNames é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 45d256f3d5a57028a04572ad67d4be0786ca39e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751915"
---
# <a name="domainnames-soap"></a><span data-ttu-id="00071-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="00071-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="00071-106">O elemento **DomainNames** representa a coleção de nomes de domínio.</span><span class="sxs-lookup"><span data-stu-id="00071-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="00071-107">O elemento **DomainNames** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="00071-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="00071-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="00071-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="00071-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="00071-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00071-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="00071-110">Attributes and elements</span></span>

<span data-ttu-id="00071-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00071-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00071-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="00071-112">Attributes</span></span>

<span data-ttu-id="00071-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00071-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00071-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00071-114">Child elements</span></span>

|<span data-ttu-id="00071-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00071-115">**Element**</span></span>|<span data-ttu-id="00071-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00071-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00071-117">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="00071-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="00071-118">Representa uma coleção de domínios que são retornados da [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), [a operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)ou a [operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="00071-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00071-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00071-119">Parent elements</span></span>

|<span data-ttu-id="00071-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00071-120">**Element**</span></span>|<span data-ttu-id="00071-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00071-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00071-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="00071-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="00071-123">Representa uma lista de relacionamentos de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="00071-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00071-124">Text value</span><span class="sxs-lookup"><span data-stu-id="00071-124">Text value</span></span>

<span data-ttu-id="00071-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00071-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00071-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="00071-126">Remarks</span></span>

<span data-ttu-id="00071-127">Esse elemento representa os domínios SMTP das organizações externas.</span><span class="sxs-lookup"><span data-stu-id="00071-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00071-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="00071-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00071-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="00071-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="00071-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00071-130">Schema Name</span></span>  <br/> |<span data-ttu-id="00071-131">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="00071-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="00071-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00071-132">Validation File</span></span>  <br/> |<span data-ttu-id="00071-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00071-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00071-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="00071-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="00071-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="00071-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00071-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="00071-136">See also</span></span>

- [<span data-ttu-id="00071-137">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="00071-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

