---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: O elemento FreeBusyAccessEnabled representa o sinalizador FreeBusyAccessEnabled (). O elemento FreeBusyAccessEnabled é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461293"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="c7495-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c7495-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="c7495-106">O elemento **FreeBusyAccessEnabled** representa o sinalizador **FreeBusyAccessEnabled ()** .</span><span class="sxs-lookup"><span data-stu-id="c7495-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="c7495-107">O elemento **FreeBusyAccessEnabled** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="c7495-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="c7495-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="c7495-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="c7495-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c7495-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7495-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c7495-110">Attributes and elements</span></span>

<span data-ttu-id="c7495-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c7495-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7495-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="c7495-112">Attributes</span></span>

<span data-ttu-id="c7495-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7495-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7495-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c7495-114">Child elements</span></span>

<span data-ttu-id="c7495-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c7495-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c7495-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c7495-116">Parent elements</span></span>

|<span data-ttu-id="c7495-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7495-117">**Element**</span></span>|<span data-ttu-id="c7495-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7495-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7495-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c7495-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="c7495-120">Representa uma lista de relações de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="c7495-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c7495-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c7495-121">Text value</span></span>

<span data-ttu-id="c7495-122">Um valor de texto **true** para o elemento **FreeBusyAccessEnabled** indica que a relação de compartilhamento deve ser usada para recuperar informações de disponibilidade de usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="c7495-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="c7495-123">Um valor **false** indica que a relação de compartilhamento deve ser suprimida.</span><span class="sxs-lookup"><span data-stu-id="c7495-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c7495-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c7495-124">Remarks</span></span>

<span data-ttu-id="c7495-125">Use este elemento para permitir ou suprimir informações de disponibilidade do servidor.</span><span class="sxs-lookup"><span data-stu-id="c7495-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c7495-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c7495-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7495-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7495-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c7495-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c7495-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c7495-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c7495-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c7495-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c7495-130">Validation File</span></span>  <br/> |<span data-ttu-id="c7495-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c7495-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7495-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c7495-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7495-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c7495-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7495-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="c7495-134">See also</span></span>



[<span data-ttu-id="c7495-135">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c7495-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

