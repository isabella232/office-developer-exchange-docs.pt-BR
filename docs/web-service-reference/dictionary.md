---
title: Dictionary
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: O elemento Dictionary define um conjunto de entradas de propriedades de dicionário para um objeto de configuração de usuário.
ms.openlocfilehash: 8e5267717aab2317b2bc1581a775ead81025a08a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455664"
---
# <a name="dictionary"></a><span data-ttu-id="745ef-103">Dictionary</span><span class="sxs-lookup"><span data-stu-id="745ef-103">Dictionary</span></span>

<span data-ttu-id="745ef-104">O elemento **Dictionary** define um conjunto de entradas de propriedades de dicionário para um objeto de configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="745ef-104">The **Dictionary** element defines a set of dictionary property entries for a user configuration object.</span></span> 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 <span data-ttu-id="745ef-105">**UserConfigurationDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="745ef-105">**UserConfigurationDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="745ef-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="745ef-106">Attributes and elements</span></span>

<span data-ttu-id="745ef-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="745ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="745ef-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="745ef-108">Attributes</span></span>

<span data-ttu-id="745ef-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="745ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="745ef-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="745ef-110">Child elements</span></span>

|<span data-ttu-id="745ef-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="745ef-111">**Element**</span></span>|<span data-ttu-id="745ef-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="745ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="745ef-113">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="745ef-113">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="745ef-114">Especifica o conteúdo de uma única propriedade de entrada de dicionário.</span><span class="sxs-lookup"><span data-stu-id="745ef-114">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="745ef-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="745ef-115">Parent elements</span></span>

|<span data-ttu-id="745ef-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="745ef-116">**Element**</span></span>|<span data-ttu-id="745ef-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="745ef-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="745ef-118">Userconfiguration</span><span class="sxs-lookup"><span data-stu-id="745ef-118">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="745ef-119">Define um único objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="745ef-119">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="745ef-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="745ef-120">Text value</span></span>

<span data-ttu-id="745ef-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="745ef-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="745ef-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="745ef-122">Remarks</span></span>

<span data-ttu-id="745ef-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="745ef-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="745ef-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="745ef-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="745ef-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="745ef-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="745ef-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="745ef-126">Schema Name</span></span>  <br/> |<span data-ttu-id="745ef-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="745ef-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="745ef-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="745ef-128">Validation File</span></span>  <br/> |<span data-ttu-id="745ef-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="745ef-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="745ef-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="745ef-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="745ef-131">False</span><span class="sxs-lookup"><span data-stu-id="745ef-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="745ef-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="745ef-132">See also</span></span>

- [<span data-ttu-id="745ef-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="745ef-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

