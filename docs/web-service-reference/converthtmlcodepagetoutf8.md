---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: O elemento ConvertHtmlCodePageToUTF8 indica se o corpo de HTML do item é convertido em UTF8.
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457589"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="768e4-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="768e4-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="768e4-104">O elemento **ConvertHtmlCodePageToUTF8** indica se o corpo de HTML do item é convertido em UTF8.</span><span class="sxs-lookup"><span data-stu-id="768e4-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="768e4-105">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="768e4-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="768e4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="768e4-106">Attributes and elements</span></span>

<span data-ttu-id="768e4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="768e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="768e4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="768e4-108">Attributes</span></span>

<span data-ttu-id="768e4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="768e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="768e4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="768e4-110">Child elements</span></span>

<span data-ttu-id="768e4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="768e4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="768e4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="768e4-112">Parent elements</span></span>

|<span data-ttu-id="768e4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="768e4-113">**Element**</span></span>|<span data-ttu-id="768e4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="768e4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="768e4-115">Shape</span><span class="sxs-lookup"><span data-stu-id="768e4-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="768e4-116">Identifica um conjunto de propriedades a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="768e4-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="768e4-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="768e4-117">Text value</span></span>

<span data-ttu-id="768e4-118">Um valor de texto **true** para o elemento **ConvertHtmlCodePageToUTF8** indica que o corpo de HTML é convertido em UTF8.</span><span class="sxs-lookup"><span data-stu-id="768e4-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="768e4-119">Um valor **false** indica que o corpo HTML não é convertido em UTF8.</span><span class="sxs-lookup"><span data-stu-id="768e4-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="768e4-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="768e4-120">Remarks</span></span>

<span data-ttu-id="768e4-121">O valor padrão **true** é usado se o elemento **ConvertHtmlCodePageToUTF8** não for especificado em uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="768e4-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="768e4-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="768e4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="768e4-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="768e4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="768e4-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="768e4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="768e4-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="768e4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="768e4-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="768e4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="768e4-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="768e4-127">Validation File</span></span>  <br/> |<span data-ttu-id="768e4-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="768e4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="768e4-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="768e4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="768e4-130">False</span><span class="sxs-lookup"><span data-stu-id="768e4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="768e4-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="768e4-131">See also</span></span>



- [<span data-ttu-id="768e4-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="768e4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

