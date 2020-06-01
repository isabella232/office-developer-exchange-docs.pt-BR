---
title: GetOrganizationRelationshipSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4e8aa3b3-4bfc-40c3-b96b-9f7062b09309
description: O elemento GetOrganizationRelationshipSettingsRequest representa os parâmetros de uma chamada para a operação de operação do GetOrganizationRelationshipSettings (SOAP). O elemento GetOrganizationRelationshipSettingsRequest é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 053bbb8cbe2ccdcf6d544ab1fc92bb81765997e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452731"
---
# <a name="getorganizationrelationshipsettingsrequest-soap"></a><span data-ttu-id="920c4-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="920c4-105">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>

<span data-ttu-id="920c4-106">O elemento **GetOrganizationRelationshipSettingsRequest** representa os parâmetros de uma chamada para a operação de [operação do GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="920c4-106">The **GetOrganizationRelationshipSettingsRequest** element represents the parameters of a call to the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation.</span></span> <span data-ttu-id="920c4-107">O elemento **GetOrganizationRelationshipSettingsRequest** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="920c4-107">The **GetOrganizationRelationshipSettingsRequest** element is for internal use only.</span></span> <span data-ttu-id="920c4-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="920c4-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsRequest>
   <Domains/>
</GetOrganizationRelationshipSettingsRequest>
```

 <span data-ttu-id="920c4-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="920c4-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="920c4-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="920c4-110">Attributes and elements</span></span>

<span data-ttu-id="920c4-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="920c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="920c4-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="920c4-112">Attributes</span></span>

<span data-ttu-id="920c4-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="920c4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="920c4-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="920c4-114">Child elements</span></span>

|<span data-ttu-id="920c4-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="920c4-115">**Element**</span></span>|<span data-ttu-id="920c4-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="920c4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="920c4-117">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="920c4-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="920c4-118">Representa uma coleção de identificadores de domínio.</span><span class="sxs-lookup"><span data-stu-id="920c4-118">Represents a collection of domain identifiers.</span></span>  <br/> |
|||
   
### <a name="parent-elements"></a><span data-ttu-id="920c4-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="920c4-119">Parent elements</span></span>

<span data-ttu-id="920c4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="920c4-120">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="920c4-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="920c4-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="920c4-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="920c4-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="920c4-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="920c4-123">Schema Name</span></span>  <br/> |<span data-ttu-id="920c4-124">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="920c4-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="920c4-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="920c4-125">Validation File</span></span>  <br/> |<span data-ttu-id="920c4-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="920c4-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="920c4-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="920c4-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="920c4-128">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="920c4-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="920c4-129">Também consulte</span><span class="sxs-lookup"><span data-stu-id="920c4-129">See also</span></span>



[<span data-ttu-id="920c4-130">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="920c4-130">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

