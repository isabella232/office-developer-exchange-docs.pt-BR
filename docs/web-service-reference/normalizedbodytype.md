---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: O elemento NormalizedBodyType Especifica se o corpo normalizado é retornado no formato HTML ou texto.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824554"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="5e8d3-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="5e8d3-103">NormalizedBodyType</span></span>

<span data-ttu-id="5e8d3-104">O elemento **NormalizedBodyType** Especifica se o corpo normalizado é retornado no formato HTML ou texto.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="5e8d3-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="5e8d3-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e8d3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5e8d3-106">Attributes and elements</span></span>

<span data-ttu-id="5e8d3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e8d3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5e8d3-108">Attributes</span></span>

<span data-ttu-id="5e8d3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e8d3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5e8d3-110">Child elements</span></span>

<span data-ttu-id="5e8d3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e8d3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5e8d3-112">Parent elements</span></span>

[<span data-ttu-id="5e8d3-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5e8d3-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="5e8d3-114">Text value</span><span class="sxs-lookup"><span data-stu-id="5e8d3-114">Text value</span></span>

<span data-ttu-id="5e8d3-115">O valor de texto do elemento **NormalizedBodyType** indica o formato do corpo normalizado é retornado em tempo.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="5e8d3-116">A tabela a seguir lista os valores possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="5e8d3-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5e8d3-117">**Value**</span></span>|<span data-ttu-id="5e8d3-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e8d3-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e8d3-119">Melhor</span><span class="sxs-lookup"><span data-stu-id="5e8d3-119">Best</span></span>  <br/> |<span data-ttu-id="5e8d3-120">A resposta retornará o conteúdo disponível mais sofisticado de corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="5e8d3-121">Isso é útil se for desconhecido se o conteúdo é o texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="5e8d3-122">O corpo retornado será o texto se o corpo armazenado for texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="5e8d3-123">Caso contrário, a resposta retornará HTML, se o corpo armazenado está no formato HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="5e8d3-124">Este é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="5e8d3-125">HTML</span><span class="sxs-lookup"><span data-stu-id="5e8d3-125">HTML</span></span>  <br/> |<span data-ttu-id="5e8d3-126">A resposta retornará um corpo normalizado como HTML.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="5e8d3-127">Texto</span><span class="sxs-lookup"><span data-stu-id="5e8d3-127">Text</span></span>  <br/> |<span data-ttu-id="5e8d3-128">A resposta retornará um corpo normalizado como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e8d3-129">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="5e8d3-129">Remarks</span></span>

<span data-ttu-id="5e8d3-130">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5e8d3-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="5e8d3-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e8d3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e8d3-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5e8d3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e8d3-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e8d3-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e8d3-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5e8d3-134">Schema Name</span></span>  <br/> |<span data-ttu-id="5e8d3-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5e8d3-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e8d3-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5e8d3-136">Validation File</span></span>  <br/> |<span data-ttu-id="5e8d3-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e8d3-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e8d3-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5e8d3-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e8d3-139">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="5e8d3-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e8d3-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="5e8d3-140">See also</span></span>



[<span data-ttu-id="5e8d3-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5e8d3-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="5e8d3-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5e8d3-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

