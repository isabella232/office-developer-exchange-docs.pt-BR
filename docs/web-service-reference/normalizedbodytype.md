---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: O elemento NormalizedBodyType especifica se o corpo normalizado é retornado no formato de texto ou HTML.
ms.openlocfilehash: e5d968673403eba24a68c67175e3ebcbb35eca39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462658"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="a7d57-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="a7d57-103">NormalizedBodyType</span></span>

<span data-ttu-id="a7d57-104">O elemento **NormalizedBodyType** especifica se o corpo normalizado é retornado no formato de texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="a7d57-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="a7d57-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="a7d57-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7d57-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a7d57-106">Attributes and elements</span></span>

<span data-ttu-id="a7d57-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7d57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7d57-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7d57-108">Attributes</span></span>

<span data-ttu-id="a7d57-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7d57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7d57-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7d57-110">Child elements</span></span>

<span data-ttu-id="a7d57-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7d57-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7d57-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7d57-112">Parent elements</span></span>

[<span data-ttu-id="a7d57-113">Shape</span><span class="sxs-lookup"><span data-stu-id="a7d57-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="a7d57-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a7d57-114">Text value</span></span>

<span data-ttu-id="a7d57-115">O valor de texto do elemento **NormalizedBodyType** indica o formato em que o corpo normalizado é retornado.</span><span class="sxs-lookup"><span data-stu-id="a7d57-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="a7d57-116">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="a7d57-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="a7d57-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a7d57-117">**Value**</span></span>|<span data-ttu-id="a7d57-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7d57-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7d57-119">Melhor</span><span class="sxs-lookup"><span data-stu-id="a7d57-119">Best</span></span>  <br/> |<span data-ttu-id="a7d57-120">A resposta retornará o conteúdo mais avançado disponível do corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="a7d57-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="a7d57-121">Isso é útil se for desconhecido se o conteúdo for texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="a7d57-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="a7d57-122">O corpo retornado será texto se o corpo armazenado for texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="a7d57-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="a7d57-123">Caso contrário, a resposta retornará HTML se o corpo armazenado estiver em formato HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="a7d57-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="a7d57-124">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="a7d57-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="a7d57-125">HTML</span><span class="sxs-lookup"><span data-stu-id="a7d57-125">HTML</span></span>  <br/> |<span data-ttu-id="a7d57-126">A resposta retornará um corpo normalizado como HTML.</span><span class="sxs-lookup"><span data-stu-id="a7d57-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="a7d57-127">Texto</span><span class="sxs-lookup"><span data-stu-id="a7d57-127">Text</span></span>  <br/> |<span data-ttu-id="a7d57-128">A resposta retornará um corpo normalizado como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="a7d57-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7d57-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="a7d57-129">Remarks</span></span>

<span data-ttu-id="a7d57-130">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a7d57-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a7d57-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7d57-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7d57-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a7d57-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7d57-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7d57-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7d57-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7d57-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a7d57-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a7d57-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7d57-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7d57-136">Validation File</span></span>  <br/> |<span data-ttu-id="a7d57-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a7d57-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7d57-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7d57-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7d57-139">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="a7d57-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7d57-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="a7d57-140">See also</span></span>



[<span data-ttu-id="a7d57-141">Shape</span><span class="sxs-lookup"><span data-stu-id="a7d57-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="a7d57-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a7d57-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

