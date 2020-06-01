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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459437"
---
# <a name="uniquebodytype"></a><span data-ttu-id="99458-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="99458-103">UniqueBodyType</span></span>

<span data-ttu-id="99458-104">O elemento **UniqueBodyType** especifica se o corpo exclusivo é retornado no formato de texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="99458-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="99458-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="99458-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99458-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="99458-106">Attributes and elements</span></span>

<span data-ttu-id="99458-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99458-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99458-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99458-108">Attributes</span></span>

<span data-ttu-id="99458-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99458-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99458-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99458-110">Child elements</span></span>

<span data-ttu-id="99458-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99458-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99458-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99458-112">Parent elements</span></span>

[<span data-ttu-id="99458-113">Shape</span><span class="sxs-lookup"><span data-stu-id="99458-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="99458-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="99458-114">Text value</span></span>

<span data-ttu-id="99458-115">O valor de texto do elemento **UniqueBodyType** indica o formato em que o corpo exclusivo é retornado.</span><span class="sxs-lookup"><span data-stu-id="99458-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="99458-116">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="99458-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="99458-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="99458-117">**Value**</span></span>|<span data-ttu-id="99458-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99458-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99458-119">Melhor</span><span class="sxs-lookup"><span data-stu-id="99458-119">Best</span></span>  <br/> |<span data-ttu-id="99458-120">A resposta retornará o conteúdo mais avançado disponível do corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="99458-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="99458-121">Isso é útil se for desconhecido se o conteúdo for texto ou HTML.</span><span class="sxs-lookup"><span data-stu-id="99458-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="99458-122">O corpo retornado será texto se o corpo armazenado for texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="99458-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="99458-123">Caso contrário, a resposta retornará HTML se o corpo armazenado estiver em formato HTML ou RTF.</span><span class="sxs-lookup"><span data-stu-id="99458-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="99458-124">Esse é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="99458-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="99458-125">HTML</span><span class="sxs-lookup"><span data-stu-id="99458-125">HTML</span></span>  <br/> |<span data-ttu-id="99458-126">A resposta retornará um corpo exclusivo como HTML.</span><span class="sxs-lookup"><span data-stu-id="99458-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="99458-127">Texto</span><span class="sxs-lookup"><span data-stu-id="99458-127">Text</span></span>  <br/> |<span data-ttu-id="99458-128">A resposta retornará um corpo exclusivo como texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="99458-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="99458-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="99458-129">Remarks</span></span>

<span data-ttu-id="99458-130">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="99458-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="99458-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99458-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99458-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="99458-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99458-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="99458-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99458-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99458-134">Schema Name</span></span>  <br/> |<span data-ttu-id="99458-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="99458-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="99458-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99458-136">Validation File</span></span>  <br/> |<span data-ttu-id="99458-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99458-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99458-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="99458-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="99458-139">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="99458-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99458-140">Também consulte</span><span class="sxs-lookup"><span data-stu-id="99458-140">See also</span></span>



[<span data-ttu-id="99458-141">Shape</span><span class="sxs-lookup"><span data-stu-id="99458-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="99458-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="99458-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

