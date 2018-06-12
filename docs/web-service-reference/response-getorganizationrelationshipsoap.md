---
title: Resposta (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: O elemento de resposta contém as informações de resposta GetOrganizationRelationshipSettings operação (SOAP). O elemento de resposta é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 97bef9ab9f0b860e62646703c35d539b7922a65a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825174"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="a017c-105">Resposta (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a017c-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="a017c-106">O elemento de **resposta** contém as informações de resposta [GetOrganizationRelationshipSettings operação (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="a017c-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="a017c-107">O elemento de **resposta** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="a017c-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="a017c-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="a017c-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="a017c-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="a017c-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a017c-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a017c-110">Attributes and elements</span></span>

<span data-ttu-id="a017c-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a017c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a017c-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a017c-112">Attributes</span></span>

<span data-ttu-id="a017c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a017c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a017c-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a017c-114">Child elements</span></span>

|<span data-ttu-id="a017c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a017c-115">**Element**</span></span>|<span data-ttu-id="a017c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a017c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a017c-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a017c-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="a017c-118">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="a017c-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a017c-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a017c-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="a017c-120">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="a017c-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="a017c-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a017c-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="a017c-122">Representa uma lista de relacionamentos da organização que correspondem à consulta.</span><span class="sxs-lookup"><span data-stu-id="a017c-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a017c-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a017c-123">Parent elements</span></span>

<span data-ttu-id="a017c-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a017c-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a017c-125">Text value</span><span class="sxs-lookup"><span data-stu-id="a017c-125">Text value</span></span>

<span data-ttu-id="a017c-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a017c-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a017c-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a017c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a017c-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="a017c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a017c-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a017c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="a017c-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="a017c-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a017c-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a017c-131">Validation File</span></span>  <br/> |<span data-ttu-id="a017c-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a017c-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a017c-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a017c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="a017c-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a017c-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a017c-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="a017c-135">See also</span></span>



[<span data-ttu-id="a017c-136">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a017c-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

