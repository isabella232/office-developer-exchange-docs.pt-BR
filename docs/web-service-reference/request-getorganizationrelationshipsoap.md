---
title: Solicitação (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 85dc155c-fad0-4756-b9a8-dedf5040a7c6
description: O elemento Request representa uma solicitação GetOrganizationRelationshipSettingsRequest (SOAP). O elemento request é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 90ccd3579c91c916ea645e6a3b466c9de4706421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459557"
---
# <a name="request-getorganizationrelationship-soap"></a><span data-ttu-id="5ddaf-105">Solicitação (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ddaf-105">Request (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="5ddaf-106">O elemento **Request** representa uma solicitação [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5ddaf-106">The **Request** element represents a [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) request.</span></span> <span data-ttu-id="5ddaf-107">O elemento **Request** é somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5ddaf-107">The **Request** element is for internal use only.</span></span> <span data-ttu-id="5ddaf-108">Esse elemento não é usado por clientes.</span><span class="sxs-lookup"><span data-stu-id="5ddaf-108">This element is not used by clients.</span></span> 
  
```XML
<Request>
   <Domains/>
</Request>
```

 <span data-ttu-id="5ddaf-109">**GetOrganizationRelationshipSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="5ddaf-109">**GetOrganizationRelationshipSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ddaf-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5ddaf-110">Attributes and elements</span></span>

<span data-ttu-id="5ddaf-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5ddaf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ddaf-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="5ddaf-112">Attributes</span></span>

<span data-ttu-id="5ddaf-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ddaf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ddaf-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5ddaf-114">Child elements</span></span>

|<span data-ttu-id="5ddaf-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5ddaf-115">**Element**</span></span>|<span data-ttu-id="5ddaf-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5ddaf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ddaf-117">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ddaf-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="5ddaf-118">Representa os domínios para os quais a descoberta automática deve ser executada e que devem ser usados em uma consulta.</span><span class="sxs-lookup"><span data-stu-id="5ddaf-118">Represents the domains for which Autodiscover is to be run and that are to be used in a query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ddaf-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5ddaf-119">Parent elements</span></span>

|<span data-ttu-id="5ddaf-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5ddaf-120">**Element**</span></span>|<span data-ttu-id="5ddaf-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5ddaf-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ddaf-122">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ddaf-122">GetOrganizationRelationshipSettingsRequestMessage (SOAP)</span></span>](getorganizationrelationshipsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="5ddaf-123">Representa uma solicitação de operação de [operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5ddaf-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ddaf-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5ddaf-124">Text value</span></span>

<span data-ttu-id="5ddaf-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ddaf-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ddaf-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5ddaf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ddaf-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="5ddaf-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5ddaf-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5ddaf-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5ddaf-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5ddaf-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5ddaf-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5ddaf-130">Validation File</span></span>  <br/> |<span data-ttu-id="5ddaf-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5ddaf-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ddaf-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5ddaf-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ddaf-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5ddaf-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ddaf-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="5ddaf-134">See also</span></span>



[<span data-ttu-id="5ddaf-135">GetOrganizationRelationshipSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5ddaf-135">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md)


[<span data-ttu-id="5ddaf-136">Trabalhando com a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="5ddaf-136">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

