---
title: DictionaryValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryValue
api_type:
- schema
ms.assetid: f4089381-826f-4f6a-8c6d-e51b910cbe6d
description: O elemento DictionaryValue Especifica o valor do dicionário para uma propriedade de dicionário.
ms.openlocfilehash: 78e4cd7e5d3d8f18276912da56bafb44cda76753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751812"
---
# <a name="dictionaryvalue"></a><span data-ttu-id="c11e6-103">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="c11e6-103">DictionaryValue</span></span>

<span data-ttu-id="c11e6-104">O elemento **DictionaryValue** Especifica o valor do dicionário para uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="c11e6-104">The **DictionaryValue** element specifies the dictionary value for a dictionary property.</span></span> 
  
```xml
<DictionaryValue>
   <Type/>
   <Value/>
</DictionaryValue>
```

 <span data-ttu-id="c11e6-105">**UserConfigurationDictionaryObjectType**</span><span class="sxs-lookup"><span data-stu-id="c11e6-105">**UserConfigurationDictionaryObjectType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c11e6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c11e6-106">Attributes and elements</span></span>

<span data-ttu-id="c11e6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c11e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c11e6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c11e6-108">Attributes</span></span>

<span data-ttu-id="c11e6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c11e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c11e6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c11e6-110">Child elements</span></span>

|<span data-ttu-id="c11e6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c11e6-111">**Element**</span></span>|<span data-ttu-id="c11e6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c11e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c11e6-113">Tipo (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="c11e6-113">Type (UserConfiguration)</span></span>](type-userconfiguration.md) <br/> |<span data-ttu-id="c11e6-114">Especifica o tipo de objeto do dicionário.</span><span class="sxs-lookup"><span data-stu-id="c11e6-114">Specifies the dictionary object type.</span></span>  <br/> |
|[<span data-ttu-id="c11e6-115">Valor (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="c11e6-115">Value (UserConfiguration)</span></span>](value-userconfiguration.md) <br/> |<span data-ttu-id="c11e6-116">Especifica o valor do objeto dictionary como uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="c11e6-116">Specifies the dictionary object value as a string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c11e6-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c11e6-117">Parent elements</span></span>

|<span data-ttu-id="c11e6-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c11e6-118">**Element**</span></span>|<span data-ttu-id="c11e6-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c11e6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c11e6-120">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="c11e6-120">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="c11e6-121">Especifica o conteúdo de uma propriedade de entrada do dicionário único.</span><span class="sxs-lookup"><span data-stu-id="c11e6-121">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c11e6-122">Text value</span><span class="sxs-lookup"><span data-stu-id="c11e6-122">Text value</span></span>

<span data-ttu-id="c11e6-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c11e6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c11e6-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c11e6-124">Remarks</span></span>

<span data-ttu-id="c11e6-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c11e6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c11e6-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c11e6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c11e6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c11e6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c11e6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c11e6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c11e6-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c11e6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c11e6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c11e6-130">Validation File</span></span>  <br/> |<span data-ttu-id="c11e6-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c11e6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c11e6-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c11e6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c11e6-133">False</span><span class="sxs-lookup"><span data-stu-id="c11e6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c11e6-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="c11e6-134">See also</span></span>

- [<span data-ttu-id="c11e6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c11e6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

