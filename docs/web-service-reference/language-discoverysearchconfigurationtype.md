---
title: Language (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: O elemento Language (DiscoverySearchConfigurationType) identifica a cultura a ser usada para o formato específico de cultura de intervalos de datas. Também especifica o idioma usado em uma consulta de pesquisa.
ms.openlocfilehash: 3cf85525147bec5d6dfc6fe2b2af5916d42c44be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463283"
---
# <a name="language-discoverysearchconfigurationtype"></a><span data-ttu-id="a80ea-104">Language (DiscoverySearchConfigurationType)</span><span class="sxs-lookup"><span data-stu-id="a80ea-104">Language (DiscoverySearchConfigurationType)</span></span>

<span data-ttu-id="a80ea-105">O elemento **Language (DiscoverySearchConfigurationType)** identifica a cultura a ser usada para o formato específico de cultura de intervalos de datas.</span><span class="sxs-lookup"><span data-stu-id="a80ea-105">The **Language (DiscoverySearchConfigurationType)** element identifies the culture to be used for the culture-specific format of date ranges.</span></span> <span data-ttu-id="a80ea-106">Também especifica o idioma usado em uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a80ea-106">It also specifies the language used in a search query.</span></span> 
  
```XML
<Language />
```

 <span data-ttu-id="a80ea-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="a80ea-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a80ea-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a80ea-108">Attributes and elements</span></span>

<span data-ttu-id="a80ea-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a80ea-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a80ea-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a80ea-110">Attributes</span></span>

<span data-ttu-id="a80ea-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a80ea-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a80ea-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a80ea-112">Child elements</span></span>

<span data-ttu-id="a80ea-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a80ea-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a80ea-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a80ea-114">Parent elements</span></span>

[<span data-ttu-id="a80ea-115">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a80ea-115">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="a80ea-116">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a80ea-116">Text value</span></span>

<span data-ttu-id="a80ea-117">O valor de texto do elemento **Language (DiscoverySearchConfigurationType)** é uma cultura ou idioma.</span><span class="sxs-lookup"><span data-stu-id="a80ea-117">The text value of the **Language (DiscoverySearchConfigurationType)** element is a culture or language.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a80ea-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="a80ea-118">Remarks</span></span>

<span data-ttu-id="a80ea-119">Este elemento Especifica o formato dos intervalos de datas especificados na [operação SearchMailboxes](searchmailboxes-operation.md) ou na [operação SetHoldOnMailboxes](setholdonmailboxes-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a80ea-119">This element specifies the format of date ranges specified in the [SearchMailboxes operation](searchmailboxes-operation.md) or the [SetHoldOnMailboxes operation](setholdonmailboxes-operation.md).</span></span>
  
<span data-ttu-id="a80ea-120">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a80ea-120">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a80ea-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a80ea-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a80ea-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a80ea-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a80ea-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a80ea-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a80ea-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a80ea-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a80ea-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a80ea-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a80ea-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a80ea-126">Validation File</span></span>  <br/> |<span data-ttu-id="a80ea-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a80ea-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a80ea-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a80ea-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a80ea-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a80ea-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a80ea-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a80ea-130">See also</span></span>



[<span data-ttu-id="a80ea-131">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a80ea-131">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)


- [<span data-ttu-id="a80ea-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a80ea-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

