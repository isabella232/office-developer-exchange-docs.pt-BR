---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: O elemento UniqueBodyType especifica se o corpo exclusivo é retornado no formato de texto ou HTML.
ms.openlocfilehash: 7e6c4631ef589555ce4d5da747c200ffe956f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459437"
---
# <a name="uniquebodytype"></a><span data-ttu-id="d70bc-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="d70bc-103">UniqueBodyType</span></span>

<span data-ttu-id="d70bc-104">O elemento **UniqueBodyType** especifica se o corpo exclusivo é retornado no formato de texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="d70bc-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="d70bc-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="d70bc-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d70bc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d70bc-106">Attributes and elements</span></span>

<span data-ttu-id="d70bc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d70bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d70bc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d70bc-108">Attributes</span></span>

<span data-ttu-id="d70bc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d70bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d70bc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d70bc-110">Child elements</span></span>

<span data-ttu-id="d70bc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d70bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d70bc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d70bc-112">Parent elements</span></span>

[<span data-ttu-id="d70bc-113">Shape</span><span class="sxs-lookup"><span data-stu-id="d70bc-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="d70bc-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d70bc-114">Text value</span></span>

<span data-ttu-id="d70bc-115">O valor de texto do elemento **UniqueBodyType** indica o formato em que o corpo exclusivo é retornado.</span><span class="sxs-lookup"><span data-stu-id="d70bc-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="d70bc-116">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="d70bc-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="d70bc-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d70bc-117">**Value**</span></span>|<span data-ttu-id="d70bc-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d70bc-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d70bc-119">Melhor</span><span class="sxs-lookup"><span data-stu-id="d70bc-119">Best</span></span>  <br/> |<span data-ttu-id="d70bc-120">A resposta retornará o conteúdo mais avançado disponível do corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="d70bc-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="d70bc-121">Isso é útil se for desconhecido se o conteúdo for texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="d70bc-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="d70bc-122">O corpo retornado será texto se o corpo armazenado for texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="d70bc-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="d70bc-123">Caso contrário, a resposta retornará HTML se o corpo armazenado estiver em formato HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="d70bc-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="d70bc-124">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="d70bc-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="d70bc-125">HTML</span><span class="sxs-lookup"><span data-stu-id="d70bc-125">HTML</span></span>  <br/> |<span data-ttu-id="d70bc-126">A resposta retornará um corpo exclusivo como HTML.</span><span class="sxs-lookup"><span data-stu-id="d70bc-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="d70bc-127">Texto</span><span class="sxs-lookup"><span data-stu-id="d70bc-127">Text</span></span>  <br/> |<span data-ttu-id="d70bc-128">A resposta retornará um corpo exclusivo como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="d70bc-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d70bc-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="d70bc-129">Remarks</span></span>

<span data-ttu-id="d70bc-130">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d70bc-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="d70bc-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d70bc-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d70bc-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d70bc-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d70bc-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="d70bc-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d70bc-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d70bc-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d70bc-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d70bc-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d70bc-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d70bc-136">Validation File</span></span>  <br/> |<span data-ttu-id="d70bc-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d70bc-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d70bc-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d70bc-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d70bc-139">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d70bc-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d70bc-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="d70bc-140">See also</span></span>



[<span data-ttu-id="d70bc-141">Shape</span><span class="sxs-lookup"><span data-stu-id="d70bc-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="d70bc-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d70bc-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

