---
title: Resposta (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: O elemento Response contém as informações de resposta da operação GetOrganizationRelationshipSettings (SOAP). O elemento Response é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 55f8cd549f40b780b2e7438634a851a2c3854f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467939"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="64c96-105">Resposta (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="64c96-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="64c96-106">O elemento **Response** contém as informações de resposta da [operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="64c96-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="64c96-107">O elemento **Response** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="64c96-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="64c96-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="64c96-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="64c96-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="64c96-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64c96-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="64c96-110">Attributes and elements</span></span>

<span data-ttu-id="64c96-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="64c96-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64c96-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="64c96-112">Attributes</span></span>

<span data-ttu-id="64c96-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64c96-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64c96-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="64c96-114">Child elements</span></span>

|<span data-ttu-id="64c96-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64c96-115">**Element**</span></span>|<span data-ttu-id="64c96-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c96-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64c96-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="64c96-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="64c96-118">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="64c96-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="64c96-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="64c96-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="64c96-120">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="64c96-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="64c96-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="64c96-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="64c96-122">Representa uma lista de relações de organização que correspondem à consulta.</span><span class="sxs-lookup"><span data-stu-id="64c96-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64c96-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="64c96-123">Parent elements</span></span>

<span data-ttu-id="64c96-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64c96-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="64c96-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="64c96-125">Text value</span></span>

<span data-ttu-id="64c96-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64c96-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64c96-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="64c96-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64c96-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="64c96-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="64c96-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="64c96-129">Schema Name</span></span>  <br/> |<span data-ttu-id="64c96-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="64c96-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="64c96-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="64c96-131">Validation File</span></span>  <br/> |<span data-ttu-id="64c96-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="64c96-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="64c96-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="64c96-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="64c96-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="64c96-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64c96-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="64c96-135">See also</span></span>



[<span data-ttu-id="64c96-136">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="64c96-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

