---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: O elemento BodyContentAttributedValue especifica o conteúdo do corpo de um item.
ms.openlocfilehash: 3550d9307e9bd652afc217f72610379a0a5b2f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527394"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="68615-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="68615-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="68615-104">O elemento **BodyContentAttributedValue** especifica o conteúdo do corpo de um item.</span><span class="sxs-lookup"><span data-stu-id="68615-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="68615-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="68615-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68615-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="68615-106">Attributes and elements</span></span>

<span data-ttu-id="68615-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="68615-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68615-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="68615-108">Attributes</span></span>

<span data-ttu-id="68615-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68615-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68615-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="68615-110">Child elements</span></span>

|<span data-ttu-id="68615-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68615-111">**Element**</span></span>|<span data-ttu-id="68615-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68615-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68615-113">Valor (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="68615-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="68615-114">Especifica o valor de um elemento **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="68615-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="68615-115">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="68615-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="68615-116">Especifica uma matriz de informações de atribuição para um ou mais dos contatos ou destinatários do Active Directory agregados no persona associado.</span><span class="sxs-lookup"><span data-stu-id="68615-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68615-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="68615-117">Parent elements</span></span>

|<span data-ttu-id="68615-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68615-118">**Element**</span></span>|<span data-ttu-id="68615-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68615-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68615-120">Agências</span><span class="sxs-lookup"><span data-stu-id="68615-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="68615-121">Especifica uma matriz de elementos **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="68615-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="68615-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="68615-122">Remarks</span></span>

<span data-ttu-id="68615-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="68615-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="68615-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="68615-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68615-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="68615-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68615-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="68615-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="68615-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="68615-127">Schema Name</span></span>  <br/> |<span data-ttu-id="68615-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="68615-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="68615-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="68615-129">Validation File</span></span>  <br/> |<span data-ttu-id="68615-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="68615-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="68615-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="68615-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="68615-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="68615-132">See also</span></span>



- [<span data-ttu-id="68615-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="68615-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

