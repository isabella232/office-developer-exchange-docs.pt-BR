---
title: ArrayOfDomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6dbd9221-e019-4981-bcdb-ea370331f407
description: O elemento ArrayOfDomainResponse contém uma matriz de respostas para as configurações do cada domínio solicitada.
ms.openlocfilehash: 7dec7f4e3df2fd0d7d1fcd4f08bc74a2b432af1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2018
ms.locfileid: "19751207"
---
# <a name="arrayofdomainresponse-soap"></a><span data-ttu-id="c55a4-103">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c55a4-103">ArrayOfDomainResponse (SOAP)</span></span>

<span data-ttu-id="c55a4-104">O elemento **ArrayOfDomainResponse** contém uma matriz de respostas para as configurações do cada domínio solicitada.</span><span class="sxs-lookup"><span data-stu-id="c55a4-104">The **ArrayOfDomainResponse** element contains an array of responses for each requested domain's settings.</span></span> 
  
```XML
<ArrayOfDomainResponse>
   <DomainResponse/>
</ArrayOfDomainResponse>
```

 <span data-ttu-id="c55a4-105">**ArrayOfDomainResponse**</span><span class="sxs-lookup"><span data-stu-id="c55a4-105">**ArrayOfDomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c55a4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c55a4-106">Attributes and elements</span></span>

<span data-ttu-id="c55a4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c55a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c55a4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c55a4-108">Attributes</span></span>

<span data-ttu-id="c55a4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c55a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c55a4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c55a4-110">Child elements</span></span>

|<span data-ttu-id="c55a4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c55a4-111">**Element**</span></span>|<span data-ttu-id="c55a4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c55a4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c55a4-113">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c55a4-113">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="c55a4-114">Contém as configurações solicitadas para o domínio especificado.</span><span class="sxs-lookup"><span data-stu-id="c55a4-114">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c55a4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c55a4-115">Parent elements</span></span>

<span data-ttu-id="c55a4-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c55a4-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c55a4-117">Text value</span><span class="sxs-lookup"><span data-stu-id="c55a4-117">Text value</span></span>

<span data-ttu-id="c55a4-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c55a4-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c55a4-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c55a4-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c55a4-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="c55a4-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c55a4-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c55a4-121">Schema Name</span></span>  <br/> |<span data-ttu-id="c55a4-122">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c55a4-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c55a4-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c55a4-123">Validation File</span></span>  <br/> |<span data-ttu-id="c55a4-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c55a4-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c55a4-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c55a4-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="c55a4-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c55a4-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c55a4-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="c55a4-127">See also</span></span>

- [<span data-ttu-id="c55a4-128">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c55a4-128">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

