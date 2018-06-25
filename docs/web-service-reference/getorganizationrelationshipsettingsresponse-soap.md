---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: O elemento GetOrganizationRelationshipSettingsResponse contém a resposta de operação (SOAP) GetOrganizationRelationshipSettings. O elemento GetOrganizationRelationshipSettingsResponse é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752576"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="6d0c9-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6d0c9-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="6d0c9-106">O elemento **GetOrganizationRelationshipSettingsResponse** contém a resposta de [operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="6d0c9-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="6d0c9-107">O elemento **GetOrganizationRelationshipSettingsResponse** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="6d0c9-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="6d0c9-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="6d0c9-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d0c9-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6d0c9-110">Attributes and elements</span></span>

<span data-ttu-id="6d0c9-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d0c9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d0c9-112">Attributes</span></span>

<span data-ttu-id="6d0c9-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d0c9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d0c9-114">Child elements</span></span>

|<span data-ttu-id="6d0c9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d0c9-115">**Element**</span></span>|<span data-ttu-id="6d0c9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d0c9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d0c9-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6d0c9-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="6d0c9-118">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="6d0c9-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6d0c9-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="6d0c9-120">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="6d0c9-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6d0c9-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="6d0c9-122">Representa uma coleção de relacionamentos da organização que correspondem à consulta.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d0c9-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d0c9-123">Parent elements</span></span>

<span data-ttu-id="6d0c9-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6d0c9-125">Text value</span><span class="sxs-lookup"><span data-stu-id="6d0c9-125">Text value</span></span>

<span data-ttu-id="6d0c9-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d0c9-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d0c9-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6d0c9-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d0c9-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d0c9-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6d0c9-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6d0c9-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6d0c9-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6d0c9-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6d0c9-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6d0c9-131">Validation File</span></span>  <br/> |<span data-ttu-id="6d0c9-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d0c9-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d0c9-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6d0c9-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d0c9-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6d0c9-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d0c9-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="6d0c9-135">See also</span></span>



[<span data-ttu-id="6d0c9-136">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6d0c9-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

