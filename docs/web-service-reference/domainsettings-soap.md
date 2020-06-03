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
ms.openlocfilehash: 67e3753b0cf5c7c653664ff087f697ce7ae2b7a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530695"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="97eaa-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="97eaa-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="97eaa-104">O elemento **DomainSettings** representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="97eaa-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="97eaa-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="97eaa-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97eaa-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="97eaa-106">Attributes and elements</span></span>

<span data-ttu-id="97eaa-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97eaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97eaa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97eaa-108">Attributes</span></span>

<span data-ttu-id="97eaa-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97eaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97eaa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97eaa-110">Child elements</span></span>

|<span data-ttu-id="97eaa-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97eaa-111">**Element**</span></span>|<span data-ttu-id="97eaa-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97eaa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97eaa-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="97eaa-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="97eaa-114">Contém as configurações de domínio retornadas por uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="97eaa-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97eaa-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97eaa-115">Parent elements</span></span>

|<span data-ttu-id="97eaa-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97eaa-116">**Element**</span></span>|<span data-ttu-id="97eaa-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97eaa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97eaa-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="97eaa-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="97eaa-119">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="97eaa-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97eaa-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="97eaa-120">Text value</span></span>

<span data-ttu-id="97eaa-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97eaa-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97eaa-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="97eaa-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97eaa-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="97eaa-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="97eaa-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97eaa-124">Schema Name</span></span>  <br/> |<span data-ttu-id="97eaa-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="97eaa-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="97eaa-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97eaa-126">Validation File</span></span>  <br/> |<span data-ttu-id="97eaa-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="97eaa-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97eaa-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="97eaa-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="97eaa-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="97eaa-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97eaa-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="97eaa-130">See also</span></span>

- [<span data-ttu-id="97eaa-131">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="97eaa-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

