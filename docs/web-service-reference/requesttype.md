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
description: O elemento RequestType identifica se uma solicitação de proxy é uma solicitação de intersite ou entre florestas.
ms.openlocfilehash: 278a65a1f2ce4cb433ae8099703d70d0a2cafa3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455965"
---
# <a name="requesttype"></a><span data-ttu-id="f3cf2-103">RequestType</span><span class="sxs-lookup"><span data-stu-id="f3cf2-103">RequestType</span></span>

<span data-ttu-id="f3cf2-104">O elemento **RequestType** identifica se uma solicitação de proxy é uma solicitação de intersite ou entre florestas.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-104">The **RequestType** element identifies whether a proxy request is a cross-site or a cross-forest request.</span></span> 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 <span data-ttu-id="f3cf2-105">**AvailabilityProxyRequestType**</span><span class="sxs-lookup"><span data-stu-id="f3cf2-105">**AvailabilityProxyRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3cf2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f3cf2-106">Attributes and elements</span></span>

<span data-ttu-id="f3cf2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3cf2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f3cf2-108">Attributes</span></span>

<span data-ttu-id="f3cf2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3cf2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3cf2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f3cf2-110">Child elements</span></span>

<span data-ttu-id="f3cf2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3cf2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f3cf2-112">Parent elements</span></span>

<span data-ttu-id="f3cf2-113">Este elemento não tem um pai no esquema.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-113">This element does not have a parent in the schema.</span></span> <span data-ttu-id="f3cf2-114">Este elemento é usado no cabeçalho SOAP.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-114">This element is used in the SOAP header.</span></span> <span data-ttu-id="f3cf2-115">Para obter mais informações sobre como esse elemento é usado, consulte o arquivo WSDL.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-115">For more information about how this element is used, see the WSDL file.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f3cf2-116">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f3cf2-116">Text value</span></span>

<span data-ttu-id="f3cf2-117">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="f3cf2-117">A text value is required for this element.</span></span> <span data-ttu-id="f3cf2-118">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="f3cf2-118">The following are the possible values:</span></span>
  
- <span data-ttu-id="f3cf2-119">CrossSite</span><span class="sxs-lookup"><span data-stu-id="f3cf2-119">CrossSite</span></span>
    
- <span data-ttu-id="f3cf2-120">CrossForest</span><span class="sxs-lookup"><span data-stu-id="f3cf2-120">CrossForest</span></span>
    
## <a name="element-information"></a><span data-ttu-id="f3cf2-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f3cf2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3cf2-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="f3cf2-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3cf2-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f3cf2-123">Schema name</span></span>  <br/> |<span data-ttu-id="f3cf2-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f3cf2-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3cf2-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f3cf2-125">Validation file</span></span>  <br/> |<span data-ttu-id="f3cf2-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f3cf2-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3cf2-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f3cf2-127">Can be empty</span></span>  <br/> |<span data-ttu-id="f3cf2-128">False</span><span class="sxs-lookup"><span data-stu-id="f3cf2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3cf2-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="f3cf2-129">See also</span></span>



- [<span data-ttu-id="f3cf2-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f3cf2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

