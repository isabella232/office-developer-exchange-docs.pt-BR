---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: O elemento GetOrganizationRelationshipSettingsResponse contém a resposta de operação do GetOrganizationRelationshipSettings (SOAP). O elemento GetOrganizationRelationshipSettingsResponse é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 0f34fbc6577b379dd0ac379564c5e6bbd940d379
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457918"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="b7328-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7328-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="b7328-106">O elemento **GetOrganizationRelationshipSettingsResponse** contém a resposta de [operação do GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="b7328-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="b7328-107">O elemento **GetOrganizationRelationshipSettingsResponse** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="b7328-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="b7328-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="b7328-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="b7328-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="b7328-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7328-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b7328-110">Attributes and elements</span></span>

<span data-ttu-id="b7328-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b7328-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7328-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="b7328-112">Attributes</span></span>

<span data-ttu-id="b7328-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7328-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7328-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b7328-114">Child elements</span></span>

|<span data-ttu-id="b7328-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b7328-115">**Element**</span></span>|<span data-ttu-id="b7328-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b7328-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7328-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7328-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="b7328-118">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="b7328-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b7328-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7328-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="b7328-120">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="b7328-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="b7328-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7328-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="b7328-122">Representa uma coleção de relações de organização que correspondem à consulta.</span><span class="sxs-lookup"><span data-stu-id="b7328-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7328-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b7328-123">Parent elements</span></span>

<span data-ttu-id="b7328-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7328-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b7328-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b7328-125">Text value</span></span>

<span data-ttu-id="b7328-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7328-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7328-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b7328-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7328-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="b7328-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="b7328-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b7328-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b7328-130">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="b7328-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="b7328-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b7328-131">Validation File</span></span>  <br/> |<span data-ttu-id="b7328-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b7328-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7328-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b7328-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7328-134">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="b7328-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7328-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b7328-135">See also</span></span>



[<span data-ttu-id="b7328-136">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b7328-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

