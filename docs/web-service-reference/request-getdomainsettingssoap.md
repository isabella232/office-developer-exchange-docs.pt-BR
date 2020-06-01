---
title: Solicitação (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: O elemento Request contém uma solicitação para retornar as configurações de domínio.
ms.openlocfilehash: c5f666102be8aaeee001a23706732e9e6c44b560
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459585"
---
# <a name="request-getdomainsettings-soap"></a><span data-ttu-id="18a95-103">Solicitação (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18a95-103">Request (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="18a95-104">O elemento **Request** contém uma solicitação para retornar as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="18a95-104">The **Request** element contains a request to return domain settings.</span></span> 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 <span data-ttu-id="18a95-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="18a95-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18a95-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="18a95-106">Attributes and elements</span></span>

<span data-ttu-id="18a95-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="18a95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18a95-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="18a95-108">Attributes</span></span>

<span data-ttu-id="18a95-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a95-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18a95-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="18a95-110">Child elements</span></span>

|<span data-ttu-id="18a95-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18a95-111">**Element**</span></span>|<span data-ttu-id="18a95-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18a95-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18a95-113">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18a95-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="18a95-114">Representa os domínios em que as configurações para as quais são retornadas em uma [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou os domínios que a organização têm federado em uma [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="18a95-114">Represents the domains the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) or the domains the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
|[<span data-ttu-id="18a95-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18a95-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="18a95-116">Contém os nomes das definições de configuração solicitadas.</span><span class="sxs-lookup"><span data-stu-id="18a95-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18a95-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="18a95-117">Parent elements</span></span>

|<span data-ttu-id="18a95-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18a95-118">**Element**</span></span>|<span data-ttu-id="18a95-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18a95-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18a95-120">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18a95-120">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="18a95-121">Representa uma solicitação de [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="18a95-121">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md)request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18a95-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="18a95-122">Text value</span></span>

<span data-ttu-id="18a95-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18a95-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18a95-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="18a95-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18a95-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="18a95-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="18a95-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="18a95-126">Schema Name</span></span>  <br/> |<span data-ttu-id="18a95-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="18a95-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="18a95-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="18a95-128">Validation File</span></span>  <br/> |<span data-ttu-id="18a95-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="18a95-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18a95-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="18a95-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="18a95-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="18a95-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18a95-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="18a95-132">See also</span></span>



[<span data-ttu-id="18a95-133">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="18a95-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

