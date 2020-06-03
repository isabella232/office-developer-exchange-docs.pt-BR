---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: O elemento DeliveryReportEnabled representa o sinalizador DeliveryReportEnabled (). O elemento DeliveryReportEnabled é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 2a163b3e6ceaa169cc8f76f395b7d501419a31ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458471"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="71c1e-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71c1e-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="71c1e-106">O elemento **DeliveryReportEnabled** representa o sinalizador **DeliveryReportEnabled ()** .</span><span class="sxs-lookup"><span data-stu-id="71c1e-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="71c1e-107">O elemento **DeliveryReportEnabled** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="71c1e-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="71c1e-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="71c1e-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="71c1e-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="71c1e-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71c1e-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="71c1e-110">Attributes and elements</span></span>

<span data-ttu-id="71c1e-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="71c1e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71c1e-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="71c1e-112">Attributes</span></span>

<span data-ttu-id="71c1e-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71c1e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71c1e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="71c1e-114">Child elements</span></span>

<span data-ttu-id="71c1e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="71c1e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71c1e-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="71c1e-116">Parent elements</span></span>

|<span data-ttu-id="71c1e-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="71c1e-117">**Element**</span></span>|<span data-ttu-id="71c1e-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="71c1e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71c1e-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71c1e-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="71c1e-120">Representa uma lista de relações de organização para uma única organização.</span><span class="sxs-lookup"><span data-stu-id="71c1e-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71c1e-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="71c1e-121">Text value</span></span>

<span data-ttu-id="71c1e-122">Um valor de texto true para o elemento DeliveryReportEnabled indica que os relatórios de entrega de usuários na organização podem ser usados.</span><span class="sxs-lookup"><span data-stu-id="71c1e-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="71c1e-123">Um valor false indica que os relatórios de entrega devem suprimir.</span><span class="sxs-lookup"><span data-stu-id="71c1e-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71c1e-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="71c1e-124">Remarks</span></span>

<span data-ttu-id="71c1e-125">Use este elemento para permitir ou suprimir os relatórios de entrega do servidor.</span><span class="sxs-lookup"><span data-stu-id="71c1e-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71c1e-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="71c1e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71c1e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="71c1e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="71c1e-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="71c1e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="71c1e-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="71c1e-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="71c1e-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="71c1e-130">Validation File</span></span>  <br/> |<span data-ttu-id="71c1e-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="71c1e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="71c1e-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="71c1e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="71c1e-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="71c1e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71c1e-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="71c1e-134">See also</span></span>

- [<span data-ttu-id="71c1e-135">Operação GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="71c1e-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

