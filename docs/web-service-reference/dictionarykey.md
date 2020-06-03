---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: O elemento DictionaryKey especifica a chave de dicionário para uma propriedade Dictionary.
ms.openlocfilehash: 8d9d897c86eb5048068936433c6c0d77917ff777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462147"
---
# <a name="dictionarykey"></a><span data-ttu-id="461ae-103">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="461ae-103">DictionaryKey</span></span>

<span data-ttu-id="461ae-104">O elemento **DictionaryKey** especifica a chave de dicionário para uma propriedade Dictionary.</span><span class="sxs-lookup"><span data-stu-id="461ae-104">The **DictionaryKey** element specifies the dictionary key for a dictionary property.</span></span> 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 <span data-ttu-id="461ae-105">**UserConfigurationDictionaryObjectType**</span><span class="sxs-lookup"><span data-stu-id="461ae-105">**UserConfigurationDictionaryObjectType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="461ae-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="461ae-106">Attributes and elements</span></span>

<span data-ttu-id="461ae-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="461ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="461ae-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="461ae-108">Attributes</span></span>

<span data-ttu-id="461ae-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="461ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="461ae-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="461ae-110">Child elements</span></span>

|<span data-ttu-id="461ae-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="461ae-111">**Element**</span></span>|<span data-ttu-id="461ae-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="461ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="461ae-113">Tipo (userconfiguration)</span><span class="sxs-lookup"><span data-stu-id="461ae-113">Type (UserConfiguration)</span></span>](type-userconfiguration.md) <br/> | <span data-ttu-id="461ae-114">Especifica um tipo de objeto Dictionary.</span><span class="sxs-lookup"><span data-stu-id="461ae-114">Specifies a dictionary object type.</span></span><br/><br/><span data-ttu-id="461ae-115">O tipo pode ser um dos seguintes valores de cadeia de caracteres:</span><span class="sxs-lookup"><span data-stu-id="461ae-115">The type can be one of the following string values:</span></span><br/><br/><span data-ttu-id="461ae-116">-DateTime</span><span class="sxs-lookup"><span data-stu-id="461ae-116">-  DateTime</span></span>  <br/><span data-ttu-id="461ae-117">-Boolean</span><span class="sxs-lookup"><span data-stu-id="461ae-117">-  Boolean</span></span>  <br/><span data-ttu-id="461ae-118">-Byte</span><span class="sxs-lookup"><span data-stu-id="461ae-118">-  Byte</span></span>  <br/><span data-ttu-id="461ae-119">-String</span><span class="sxs-lookup"><span data-stu-id="461ae-119">-  String</span></span>  <br/><span data-ttu-id="461ae-120">- Integer32</span><span class="sxs-lookup"><span data-stu-id="461ae-120">-  Integer32</span></span>  <br/><span data-ttu-id="461ae-121">- UnsignedInteger32</span><span class="sxs-lookup"><span data-stu-id="461ae-121">-  UnsignedInteger32</span></span>  <br/><span data-ttu-id="461ae-122">- Integer64</span><span class="sxs-lookup"><span data-stu-id="461ae-122">-  Integer64</span></span>  <br/><span data-ttu-id="461ae-123">- UnsignedInteger64</span><span class="sxs-lookup"><span data-stu-id="461ae-123">-  UnsignedInteger64</span></span>  <br/><span data-ttu-id="461ae-124">- StringArray</span><span class="sxs-lookup"><span data-stu-id="461ae-124">-  StringArray</span></span>  <br/><span data-ttu-id="461ae-125">-ByteArray</span><span class="sxs-lookup"><span data-stu-id="461ae-125">-  ByteArray</span></span>  <br/> |
|[<span data-ttu-id="461ae-126">Valor (userconfiguration)</span><span class="sxs-lookup"><span data-stu-id="461ae-126">Value (UserConfiguration)</span></span>](value-userconfiguration.md) <br/> |<span data-ttu-id="461ae-127">Especifica o valor do objeto Dictionary como uma cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="461ae-127">Specifies the dictionary object value as a string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="461ae-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="461ae-128">Parent elements</span></span>

|<span data-ttu-id="461ae-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="461ae-129">**Element**</span></span>|<span data-ttu-id="461ae-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="461ae-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="461ae-131">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="461ae-131">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="461ae-132">Especifica o conteúdo de uma única propriedade de entrada de dicionário.</span><span class="sxs-lookup"><span data-stu-id="461ae-132">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="461ae-133">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="461ae-133">Text value</span></span>

<span data-ttu-id="461ae-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="461ae-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="461ae-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="461ae-135">Remarks</span></span>

<span data-ttu-id="461ae-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="461ae-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="461ae-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="461ae-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="461ae-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="461ae-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="461ae-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="461ae-139">Schema Name</span></span>  <br/> |<span data-ttu-id="461ae-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="461ae-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="461ae-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="461ae-141">Validation File</span></span>  <br/> |<span data-ttu-id="461ae-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="461ae-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="461ae-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="461ae-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="461ae-144">False</span><span class="sxs-lookup"><span data-stu-id="461ae-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="461ae-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="461ae-145">See also</span></span>

- [<span data-ttu-id="461ae-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="461ae-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

