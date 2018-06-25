---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: O elemento DeliveryReportEnabled representa o sinalizador DeliveryReportEnabled(). O elemento DeliveryReportEnabled é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751775"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="3f7d0-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3f7d0-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="3f7d0-106">O elemento **DeliveryReportEnabled** representa o sinalizador **DeliveryReportEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="3f7d0-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="3f7d0-107">O elemento **DeliveryReportEnabled** é apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="3f7d0-108">Este elemento não é usado pelos clientes.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="3f7d0-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3f7d0-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f7d0-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3f7d0-110">Attributes and elements</span></span>

<span data-ttu-id="3f7d0-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f7d0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f7d0-112">Attributes</span></span>

<span data-ttu-id="3f7d0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f7d0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f7d0-114">Child elements</span></span>

<span data-ttu-id="3f7d0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f7d0-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f7d0-116">Parent elements</span></span>

|<span data-ttu-id="3f7d0-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3f7d0-117">**Element**</span></span>|<span data-ttu-id="3f7d0-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f7d0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f7d0-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3f7d0-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="3f7d0-120">Representa uma lista de relacionamentos de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f7d0-121">Text value</span><span class="sxs-lookup"><span data-stu-id="3f7d0-121">Text value</span></span>

<span data-ttu-id="3f7d0-122">Um valor de texto, True para o elemento DeliveryReportEnabled indica que os relatórios de entrega de usuários na organização podem ser usados.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="3f7d0-123">Um valor false indica que os relatórios de entrega deve ser suprimida.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f7d0-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="3f7d0-124">Remarks</span></span>

<span data-ttu-id="3f7d0-125">Use esse elemento para permitir ou suprimir notificações de entrega do servidor.</span><span class="sxs-lookup"><span data-stu-id="3f7d0-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f7d0-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3f7d0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f7d0-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f7d0-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3f7d0-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f7d0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3f7d0-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="3f7d0-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3f7d0-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f7d0-130">Validation File</span></span>  <br/> |<span data-ttu-id="3f7d0-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3f7d0-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f7d0-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3f7d0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f7d0-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3f7d0-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f7d0-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="3f7d0-134">See also</span></span>

- [<span data-ttu-id="3f7d0-135">Operação de GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3f7d0-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

