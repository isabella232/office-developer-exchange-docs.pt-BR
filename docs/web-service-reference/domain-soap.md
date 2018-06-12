---
title: Domínio (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: O elemento de domínio contém um domínio federado em uma resposta GetFederationInformation ou contém um domínio em que as definições de configuração para o qual são solicitadas em uma solicitação de GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751913"
---
# <a name="domain-soap"></a><span data-ttu-id="85e9a-103">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="85e9a-103">Domain (SOAP)</span></span>

<span data-ttu-id="85e9a-104">O elemento de **domínio** contém um domínio federado em uma resposta **GetFederationInformation** ou contém um domínio em que as definições de configuração para o qual são solicitadas em uma solicitação de **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="85e9a-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="85e9a-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="85e9a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85e9a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="85e9a-106">Attributes and elements</span></span>

<span data-ttu-id="85e9a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="85e9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85e9a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="85e9a-108">Attributes</span></span>

<span data-ttu-id="85e9a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85e9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85e9a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="85e9a-110">Child elements</span></span>

<span data-ttu-id="85e9a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85e9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85e9a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="85e9a-112">Parent elements</span></span>

|<span data-ttu-id="85e9a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="85e9a-113">**Element**</span></span>|<span data-ttu-id="85e9a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="85e9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85e9a-115">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="85e9a-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="85e9a-116">Representa os domínios que as definições de configuração para o qual são retornadas em uma operação de **GetDomainSettings** ou os domínios que a organização tem federados em uma operação de **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="85e9a-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85e9a-117">Text value</span><span class="sxs-lookup"><span data-stu-id="85e9a-117">Text value</span></span>

<span data-ttu-id="85e9a-118">O valor de texto do elemento **domínio** representa um nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="85e9a-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="85e9a-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="85e9a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85e9a-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="85e9a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="85e9a-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="85e9a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="85e9a-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="85e9a-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="85e9a-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="85e9a-123">Validation File</span></span>  <br/> |<span data-ttu-id="85e9a-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="85e9a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="85e9a-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="85e9a-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="85e9a-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="85e9a-126">True</span></span>  <br/> |
   

