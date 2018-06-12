---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: O elemento DomainSettingsErrors contém informações de erro para as configurações que não puderam ser retornadas.
ms.openlocfilehash: 6ecd23bc556ca32d724581a28cc7c117c6853207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751933"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="332d3-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="332d3-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="332d3-104">O elemento **DomainSettingsErrors** contém informações de erro para as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="332d3-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="332d3-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="332d3-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="332d3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="332d3-106">Attributes and elements</span></span>

<span data-ttu-id="332d3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="332d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="332d3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="332d3-108">Attributes</span></span>

<span data-ttu-id="332d3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="332d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="332d3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="332d3-110">Child elements</span></span>

|<span data-ttu-id="332d3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="332d3-111">**Element**</span></span>|<span data-ttu-id="332d3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="332d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="332d3-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="332d3-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="332d3-114">Representa um erro que ocorreu durante a recuperação de uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="332d3-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="332d3-115">Isso representa um erro de uma solicitação de operação [GetDomainSettings operação (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="332d3-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="332d3-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="332d3-116">Parent elements</span></span>

|<span data-ttu-id="332d3-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="332d3-117">**Element**</span></span>|<span data-ttu-id="332d3-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="332d3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="332d3-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="332d3-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="332d3-120">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="332d3-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="332d3-121">Text value</span><span class="sxs-lookup"><span data-stu-id="332d3-121">Text value</span></span>

<span data-ttu-id="332d3-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="332d3-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="332d3-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="332d3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="332d3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="332d3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="332d3-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="332d3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="332d3-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="332d3-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="332d3-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="332d3-127">Validation File</span></span>  <br/> |<span data-ttu-id="332d3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="332d3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="332d3-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="332d3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="332d3-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="332d3-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="332d3-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="332d3-131">See also</span></span>

- [<span data-ttu-id="332d3-132">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="332d3-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

