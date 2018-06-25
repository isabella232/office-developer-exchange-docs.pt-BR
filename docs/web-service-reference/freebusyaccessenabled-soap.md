---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: O elemento FreeBusyAccessEnabled representa o sinalizador FreeBusyAccessEnabled(). O elemento FreeBusyAccessEnabled é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752367"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="864b7-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="864b7-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="864b7-106">O elemento **FreeBusyAccessEnabled** representa o sinalizador **FreeBusyAccessEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="864b7-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="864b7-107">O elemento **FreeBusyAccessEnabled** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="864b7-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="864b7-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="864b7-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="864b7-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="864b7-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="864b7-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="864b7-110">Attributes and elements</span></span>

<span data-ttu-id="864b7-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="864b7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="864b7-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="864b7-112">Attributes</span></span>

<span data-ttu-id="864b7-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="864b7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="864b7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="864b7-114">Child elements</span></span>

<span data-ttu-id="864b7-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="864b7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="864b7-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="864b7-116">Parent elements</span></span>

|<span data-ttu-id="864b7-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="864b7-117">**Element**</span></span>|<span data-ttu-id="864b7-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="864b7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="864b7-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="864b7-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="864b7-120">Representa uma lista de relacionamentos de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="864b7-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="864b7-121">Text value</span><span class="sxs-lookup"><span data-stu-id="864b7-121">Text value</span></span>

<span data-ttu-id="864b7-122">Um valor de texto de **true** para o elemento **FreeBusyAccessEnabled** indica que a relação de compartilhamento deve ser usada para recuperar informações de disponibilidade dos usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="864b7-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="864b7-123">Um valor **false** indica que a relação de compartilhamento deve ser suprimida.</span><span class="sxs-lookup"><span data-stu-id="864b7-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="864b7-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="864b7-124">Remarks</span></span>

<span data-ttu-id="864b7-125">Use esse elemento para permitir ou impedir que informações de disponibilidade do servidor.</span><span class="sxs-lookup"><span data-stu-id="864b7-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="864b7-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="864b7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="864b7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="864b7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="864b7-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="864b7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="864b7-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="864b7-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="864b7-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="864b7-130">Validation File</span></span>  <br/> |<span data-ttu-id="864b7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="864b7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="864b7-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="864b7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="864b7-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="864b7-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="864b7-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="864b7-134">See also</span></span>



[<span data-ttu-id="864b7-135">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="864b7-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

