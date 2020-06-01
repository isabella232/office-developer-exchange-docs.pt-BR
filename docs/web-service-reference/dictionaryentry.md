---
title: DictionaryEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryEntry
api_type:
- schema
ms.assetid: 531ea96a-d411-43e6-9fec-11fa2c959a30
description: O elemento DictionaryEntry especifica o conteúdo de uma única propriedade de entrada de dicionário.
ms.openlocfilehash: 4c5d4c037f0c97b26d518d2f1386f71b31fa2d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455657"
---
# <a name="dictionaryentry"></a><span data-ttu-id="302d6-103">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="302d6-103">DictionaryEntry</span></span>

<span data-ttu-id="302d6-104">O elemento **DictionaryEntry** especifica o conteúdo de uma única propriedade de entrada de dicionário.</span><span class="sxs-lookup"><span data-stu-id="302d6-104">The **DictionaryEntry** element specifies the contents of a single dictionary entry property.</span></span> 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 <span data-ttu-id="302d6-105">**UserConfigurationDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="302d6-105">**UserConfigurationDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="302d6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="302d6-106">Attributes and elements</span></span>

<span data-ttu-id="302d6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="302d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="302d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="302d6-108">Attributes</span></span>

<span data-ttu-id="302d6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="302d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="302d6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="302d6-110">Child elements</span></span>

|<span data-ttu-id="302d6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="302d6-111">**Element**</span></span>|<span data-ttu-id="302d6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="302d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="302d6-113">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="302d6-113">DictionaryKey</span></span>](dictionarykey.md) <br/> |<span data-ttu-id="302d6-114">Especifica a chave de dicionário para uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="302d6-114">Specifies the dictionary key for a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="302d6-115">Dictionaryvalue</span><span class="sxs-lookup"><span data-stu-id="302d6-115">DictionaryValue</span></span>](dictionaryvalue.md) <br/> |<span data-ttu-id="302d6-116">Especifica o valor do dicionário para uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="302d6-116">Specifies the dictionary value for a dictionary property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="302d6-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="302d6-117">Parent elements</span></span>

|<span data-ttu-id="302d6-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="302d6-118">**Element**</span></span>|<span data-ttu-id="302d6-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="302d6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="302d6-120">Dictionary</span><span class="sxs-lookup"><span data-stu-id="302d6-120">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="302d6-121">Define um conjunto de entradas de propriedades de dicionário para um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="302d6-121">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="302d6-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="302d6-122">Text value</span></span>

<span data-ttu-id="302d6-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="302d6-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="302d6-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="302d6-124">Remarks</span></span>

<span data-ttu-id="302d6-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="302d6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="302d6-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="302d6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="302d6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="302d6-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="302d6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="302d6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="302d6-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="302d6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="302d6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="302d6-130">Validation File</span></span>  <br/> |<span data-ttu-id="302d6-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="302d6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="302d6-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="302d6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="302d6-133">False</span><span class="sxs-lookup"><span data-stu-id="302d6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="302d6-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="302d6-134">See also</span></span>

- [<span data-ttu-id="302d6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="302d6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

