---
title: GetOrganizationRelationshipSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: O elemento GetOrganizationRelationshipSettingsRequest representa os parâmetros de uma chamada para a operação de operação (SOAP) GetOrganizationRelationshipSettings. O elemento GetOrganizationRelationshipSettingsRequest é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 451506d53212ddca416f5b797624688f511988d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752573"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="d2f0d-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2f0d-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="d2f0d-106">O elemento **GetOrganizationRelationshipSettingsRequest** representa os parâmetros de uma chamada para a operação [GetOrganizationRelationshipSettings operação (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f0d-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="d2f0d-107">O elemento **GetOrganizationRelationshipSettingsRequest** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="d2f0d-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="d2f0d-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="d2f0d-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2f0d-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d2f0d-110">Attributes and elements</span></span>

<span data-ttu-id="d2f0d-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2f0d-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2f0d-112">Attributes</span></span>

<span data-ttu-id="d2f0d-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2f0d-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2f0d-114">Child elements</span></span>

|<span data-ttu-id="d2f0d-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2f0d-115">**Element**</span></span>|<span data-ttu-id="d2f0d-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2f0d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2f0d-117">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2f0d-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d2f0d-118">Representa uma coleção dos identificadores de domínio.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="d2f0d-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2f0d-119">Parent elements</span></span>

<span data-ttu-id="d2f0d-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2f0d-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2f0d-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d2f0d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2f0d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2f0d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d2f0d-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2f0d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="d2f0d-124">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d2f0d-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d2f0d-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2f0d-125">Validation File</span></span>  <br/> |<span data-ttu-id="d2f0d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2f0d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2f0d-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d2f0d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2f0d-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d2f0d-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2f0d-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="d2f0d-129">See also</span></span>



[<span data-ttu-id="d2f0d-130">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d2f0d-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

