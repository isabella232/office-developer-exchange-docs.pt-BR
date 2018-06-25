---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: O elemento de TargetApplicationUri define o URI do aplicativo de destino. O elemento TargetApplicationUri é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: fa401d4c1e8c1460804f116d840fe21129957852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837693"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="6aaa5-105">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6aaa5-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="6aaa5-106">O elemento de **TargetApplicationUri** define o URI do aplicativo de destino.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="6aaa5-107">O elemento **TargetApplicationUri** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="6aaa5-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="6aaa5-109">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="6aaa5-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6aaa5-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6aaa5-110">Attributes and elements</span></span>

<span data-ttu-id="6aaa5-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6aaa5-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6aaa5-112">Attributes</span></span>

<span data-ttu-id="6aaa5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6aaa5-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6aaa5-114">Child elements</span></span>

<span data-ttu-id="6aaa5-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6aaa5-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6aaa5-116">Parent elements</span></span>

|<span data-ttu-id="6aaa5-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6aaa5-117">**Element**</span></span>|<span data-ttu-id="6aaa5-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6aaa5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6aaa5-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6aaa5-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="6aaa5-120">Representa uma lista de relacionamentos de organização para uma única organização</span><span class="sxs-lookup"><span data-stu-id="6aaa5-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6aaa5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="6aaa5-121">Remarks</span></span>

<span data-ttu-id="6aaa5-122">Este elemento define o URI da organização externa de destino.</span><span class="sxs-lookup"><span data-stu-id="6aaa5-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6aaa5-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6aaa5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6aaa5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6aaa5-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6aaa5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6aaa5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6aaa5-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6aaa5-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6aaa5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6aaa5-127">Validation File</span></span>  <br/> |<span data-ttu-id="6aaa5-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6aaa5-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6aaa5-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6aaa5-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6aaa5-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6aaa5-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6aaa5-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="6aaa5-131">See also</span></span>



[<span data-ttu-id="6aaa5-132">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6aaa5-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

