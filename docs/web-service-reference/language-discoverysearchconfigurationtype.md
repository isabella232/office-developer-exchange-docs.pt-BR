---
title: Idioma (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: O elemento de idioma (DiscoverySearchConfigurationType) identifica a cultura a ser usado para o formato de específico da cultura dos intervalos de data. Ela também especifica o idioma usado em uma consulta de pesquisa.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824197"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="ac2ae-104">Idioma (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="ac2ae-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="ac2ae-105">O elemento de **idioma (DiscoverySearchConfigurationType)** identifica a cultura a ser usado para o formato de específico da cultura dos intervalos de data.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="ac2ae-106">Ela também especifica o idioma usado em uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="ac2ae-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="ac2ae-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac2ae-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ac2ae-108">Attributes and elements</span></span>

<span data-ttu-id="ac2ae-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac2ae-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac2ae-110">Attributes</span></span>

<span data-ttu-id="ac2ae-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac2ae-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac2ae-112">Child elements</span></span>

<span data-ttu-id="ac2ae-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac2ae-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac2ae-114">Parent elements</span></span>

[<span data-ttu-id="ac2ae-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac2ae-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="ac2ae-116">Text value</span><span class="sxs-lookup"><span data-stu-id="ac2ae-116">Text value</span></span>

<span data-ttu-id="ac2ae-117">O valor de texto do elemento de **idioma (DiscoverySearchConfigurationType)** é um idioma ou cultura.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac2ae-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ac2ae-118">Remarks</span></span>

<span data-ttu-id="ac2ae-119">Este elemento Especifica o formato de intervalos de data especificado na [operação SearchMailboxes](searchmailboxes-operation.md) ou a [operação SetHoldOnMailboxes](setholdonmailboxes-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ac2ae-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="ac2ae-120">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ac2ae-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ac2ae-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac2ae-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac2ae-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ac2ae-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac2ae-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac2ae-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac2ae-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ac2ae-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ac2ae-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ac2ae-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac2ae-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ac2ae-126">Validation File</span></span>  <br/> |<span data-ttu-id="ac2ae-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ac2ae-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac2ae-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ac2ae-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac2ae-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ac2ae-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac2ae-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="ac2ae-130">See also</span></span>



[<span data-ttu-id="ac2ae-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac2ae-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="ac2ae-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ac2ae-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

