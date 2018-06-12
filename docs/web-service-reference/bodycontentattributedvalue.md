---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: O elemento BodyContentAttributedValue Especifica o conteúdo do corpo de um item.
ms.openlocfilehash: f5b8f0a19b77ce550b1d7f1c415cc8ee4340863a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751308"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="00c1c-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="00c1c-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="00c1c-104">O elemento **BodyContentAttributedValue** Especifica o conteúdo do corpo de um item.</span><span class="sxs-lookup"><span data-stu-id="00c1c-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="00c1c-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="00c1c-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00c1c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="00c1c-106">Attributes and elements</span></span>

<span data-ttu-id="00c1c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00c1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00c1c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="00c1c-108">Attributes</span></span>

<span data-ttu-id="00c1c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00c1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00c1c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00c1c-110">Child elements</span></span>

|<span data-ttu-id="00c1c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00c1c-111">**Element**</span></span>|<span data-ttu-id="00c1c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00c1c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00c1c-113">Valor (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="00c1c-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="00c1c-114">Especifica o valor de um elemento **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="00c1c-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="00c1c-115">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="00c1c-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="00c1c-116">Especifica uma matriz das informações de atribuição para uma ou mais contatos ou destinatários do active directory agregados em que a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="00c1c-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00c1c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00c1c-117">Parent elements</span></span>

|<span data-ttu-id="00c1c-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00c1c-118">**Element**</span></span>|<span data-ttu-id="00c1c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00c1c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00c1c-120">Corpos</span><span class="sxs-lookup"><span data-stu-id="00c1c-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="00c1c-121">Especifica uma matriz de elementos de **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="00c1c-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00c1c-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="00c1c-122">Remarks</span></span>

<span data-ttu-id="00c1c-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00c1c-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00c1c-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="00c1c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00c1c-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="00c1c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00c1c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="00c1c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00c1c-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00c1c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="00c1c-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="00c1c-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="00c1c-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00c1c-129">Validation File</span></span>  <br/> |<span data-ttu-id="00c1c-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00c1c-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="00c1c-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="00c1c-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="00c1c-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="00c1c-132">See also</span></span>



- [<span data-ttu-id="00c1c-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="00c1c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

