---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: O elemento DomainSettings representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.
ms.openlocfilehash: 961051399dc8babd8cba6eeaf43456071d0f40a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751934"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="341bd-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="341bd-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="341bd-104">O elemento **DomainSettings** representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="341bd-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="341bd-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="341bd-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="341bd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="341bd-106">Attributes and elements</span></span>

<span data-ttu-id="341bd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="341bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="341bd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="341bd-108">Attributes</span></span>

<span data-ttu-id="341bd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="341bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="341bd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="341bd-110">Child elements</span></span>

|<span data-ttu-id="341bd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="341bd-111">**Element**</span></span>|<span data-ttu-id="341bd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="341bd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="341bd-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="341bd-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="341bd-114">Contém configurações de domínio que são retornadas por uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="341bd-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="341bd-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="341bd-115">Parent elements</span></span>

|<span data-ttu-id="341bd-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="341bd-116">**Element**</span></span>|<span data-ttu-id="341bd-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="341bd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="341bd-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="341bd-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="341bd-119">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="341bd-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="341bd-120">Text value</span><span class="sxs-lookup"><span data-stu-id="341bd-120">Text value</span></span>

<span data-ttu-id="341bd-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="341bd-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="341bd-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="341bd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="341bd-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="341bd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="341bd-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="341bd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="341bd-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="341bd-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="341bd-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="341bd-126">Validation File</span></span>  <br/> |<span data-ttu-id="341bd-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="341bd-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="341bd-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="341bd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="341bd-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="341bd-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="341bd-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="341bd-130">See also</span></span>

- [<span data-ttu-id="341bd-131">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="341bd-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

