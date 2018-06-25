---
title: RequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestType
api_type:
- schema
ms.assetid: 4e657e57-528f-4250-a99c-f9850bbbcec5
description: O elemento RequestType identifica se uma solicitação de proxy é uma solicitação de entre florestas ou entre sites.
ms.openlocfilehash: 96a4d57432b15aa54fff2618df458fc75cb227f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825139"
---
# <a name="requesttype"></a><span data-ttu-id="2a6c6-103">RequestType</span><span class="sxs-lookup"><span data-stu-id="2a6c6-103">RequestType</span></span>

<span data-ttu-id="2a6c6-104">O elemento **RequestType** identifica se uma solicitação de proxy é uma solicitação de entre florestas ou entre sites.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-104">The **RequestType** element identifies whether a proxy request is a cross-site or a cross-forest request.</span></span> 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 <span data-ttu-id="2a6c6-105">**AvailabilityProxyRequestType**</span><span class="sxs-lookup"><span data-stu-id="2a6c6-105">**AvailabilityProxyRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a6c6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2a6c6-106">Attributes and elements</span></span>

<span data-ttu-id="2a6c6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a6c6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2a6c6-108">Attributes</span></span>

<span data-ttu-id="2a6c6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a6c6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2a6c6-110">Child elements</span></span>

<span data-ttu-id="2a6c6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a6c6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2a6c6-112">Parent elements</span></span>

<span data-ttu-id="2a6c6-113">Este elemento não tem um pai no esquema.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-113">This element does not have a parent in the schema.</span></span> <span data-ttu-id="2a6c6-114">Este elemento é usado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-114">This element is used in the SOAP header.</span></span> <span data-ttu-id="2a6c6-115">Para obter mais informações sobre como esse elemento é usado, consulte o arquivo WSDL.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-115">For more information about how this element is used, see the WSDL file.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2a6c6-116">Text value</span><span class="sxs-lookup"><span data-stu-id="2a6c6-116">Text value</span></span>

<span data-ttu-id="2a6c6-117">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="2a6c6-117">A text value is required for this element.</span></span> <span data-ttu-id="2a6c6-118">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="2a6c6-118">The following are the possible values:</span></span>
  
- <span data-ttu-id="2a6c6-119">CrossSite</span><span class="sxs-lookup"><span data-stu-id="2a6c6-119">CrossSite</span></span>
    
- <span data-ttu-id="2a6c6-120">Relação</span><span class="sxs-lookup"><span data-stu-id="2a6c6-120">CrossForest</span></span>
    
## <a name="element-information"></a><span data-ttu-id="2a6c6-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2a6c6-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a6c6-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a6c6-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a6c6-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2a6c6-123">Schema name</span></span>  <br/> |<span data-ttu-id="2a6c6-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2a6c6-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a6c6-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2a6c6-125">Validation file</span></span>  <br/> |<span data-ttu-id="2a6c6-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2a6c6-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a6c6-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2a6c6-127">Can be empty</span></span>  <br/> |<span data-ttu-id="2a6c6-128">False</span><span class="sxs-lookup"><span data-stu-id="2a6c6-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a6c6-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="2a6c6-129">See also</span></span>



- [<span data-ttu-id="2a6c6-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2a6c6-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

