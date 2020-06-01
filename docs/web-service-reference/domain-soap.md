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
description: O elemento Domain contém um domínio federado em uma resposta GetFederationInformation ou contém um domínio as definições de configuração para as quais são solicitadas em uma solicitação GetDomainSettings.
ms.openlocfilehash: f90c608ee1fc3356a227bca6411eaeff0c1e8b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456980"
---
# <a name="domain-soap"></a><span data-ttu-id="3dfb1-103">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3dfb1-103">Domain (SOAP)</span></span>

<span data-ttu-id="3dfb1-104">O elemento **Domain** contém um domínio federado em uma resposta **GetFederationInformation** ou contém um domínio as definições de configuração para as quais são solicitadas em uma solicitação **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="3dfb1-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="3dfb1-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="3dfb1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3dfb1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3dfb1-106">Attributes and elements</span></span>

<span data-ttu-id="3dfb1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3dfb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dfb1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3dfb1-108">Attributes</span></span>

<span data-ttu-id="3dfb1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dfb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dfb1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3dfb1-110">Child elements</span></span>

<span data-ttu-id="3dfb1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dfb1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3dfb1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3dfb1-112">Parent elements</span></span>

|<span data-ttu-id="3dfb1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3dfb1-113">**Element**</span></span>|<span data-ttu-id="3dfb1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3dfb1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dfb1-115">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3dfb1-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="3dfb1-116">Representa os domínios em que as definições de configuração para as quais são retornadas em uma operação **GetDomainSettings** ou os domínios que a organização federaram em uma operação **GetFederationInformation** .</span><span class="sxs-lookup"><span data-stu-id="3dfb1-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3dfb1-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3dfb1-117">Text value</span></span>

<span data-ttu-id="3dfb1-118">O valor de texto do elemento **Domain** representa um nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="3dfb1-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3dfb1-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3dfb1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dfb1-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dfb1-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3dfb1-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3dfb1-121">Schema Name</span></span>  <br/> |<span data-ttu-id="3dfb1-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="3dfb1-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3dfb1-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3dfb1-123">Validation File</span></span>  <br/> |<span data-ttu-id="3dfb1-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3dfb1-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3dfb1-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3dfb1-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dfb1-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3dfb1-126">True</span></span>  <br/> |
   

