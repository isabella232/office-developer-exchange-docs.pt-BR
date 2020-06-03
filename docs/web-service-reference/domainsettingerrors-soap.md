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
description: O elemento DomainSettingsErrors contém informações de erro para configurações que não puderam ser retornadas.
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530702"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="6a54c-103">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a54c-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="6a54c-104">O elemento **DomainSettingsErrors** contém informações de erro para configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="6a54c-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="6a54c-105">**DomainSettingsErrors**</span><span class="sxs-lookup"><span data-stu-id="6a54c-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a54c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6a54c-106">Attributes and elements</span></span>

<span data-ttu-id="6a54c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6a54c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a54c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6a54c-108">Attributes</span></span>

<span data-ttu-id="6a54c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a54c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a54c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6a54c-110">Child elements</span></span>

|<span data-ttu-id="6a54c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a54c-111">**Element**</span></span>|<span data-ttu-id="6a54c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a54c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a54c-113">DomainSettingError (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a54c-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="6a54c-114">Representa um erro que ocorreu ao recuperar uma configuração de domínio.</span><span class="sxs-lookup"><span data-stu-id="6a54c-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="6a54c-115">Isso representa um erro de uma solicitação de operação de operação de [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="6a54c-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a54c-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6a54c-116">Parent elements</span></span>

|<span data-ttu-id="6a54c-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a54c-117">**Element**</span></span>|<span data-ttu-id="6a54c-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a54c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a54c-119">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a54c-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="6a54c-120">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="6a54c-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a54c-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6a54c-121">Text value</span></span>

<span data-ttu-id="6a54c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a54c-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a54c-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6a54c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a54c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a54c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6a54c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6a54c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6a54c-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="6a54c-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6a54c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6a54c-127">Validation File</span></span>  <br/> |<span data-ttu-id="6a54c-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6a54c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a54c-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6a54c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a54c-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6a54c-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a54c-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="6a54c-131">See also</span></span>

- [<span data-ttu-id="6a54c-132">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a54c-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

