---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: O elemento DomainSetting contém configurações de domínio que são retornadas pela solicitação de operação GetDomainSettings operação (SOAP).
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751929"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="88a60-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88a60-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="88a60-104">O elemento **DomainSetting** contém configurações de domínio que são retornadas pela solicitação de operação [GetDomainSettings operação (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="88a60-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="88a60-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="88a60-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88a60-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="88a60-106">Attributes and elements</span></span>

<span data-ttu-id="88a60-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88a60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88a60-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="88a60-108">Attributes</span></span>

<span data-ttu-id="88a60-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88a60-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88a60-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88a60-110">Child elements</span></span>

|<span data-ttu-id="88a60-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88a60-111">**Element**</span></span>|<span data-ttu-id="88a60-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88a60-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88a60-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88a60-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="88a60-114">Representa o nome de uma configuração.</span><span class="sxs-lookup"><span data-stu-id="88a60-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88a60-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88a60-115">Parent elements</span></span>

|<span data-ttu-id="88a60-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88a60-116">**Element**</span></span>|<span data-ttu-id="88a60-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88a60-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88a60-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88a60-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="88a60-119">Representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="88a60-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88a60-120">Text value</span><span class="sxs-lookup"><span data-stu-id="88a60-120">Text value</span></span>

<span data-ttu-id="88a60-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88a60-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88a60-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="88a60-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88a60-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="88a60-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="88a60-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88a60-124">Schema Name</span></span>  <br/> |<span data-ttu-id="88a60-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="88a60-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="88a60-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88a60-126">Validation File</span></span>  <br/> |<span data-ttu-id="88a60-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88a60-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88a60-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="88a60-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="88a60-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="88a60-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88a60-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="88a60-130">See also</span></span>

- [<span data-ttu-id="88a60-131">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88a60-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

