---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: O elemento IndexedFieldURI identifica membros individuais de um dicionário.
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823909"
---
# <a name="indexedfielduri"></a><span data-ttu-id="26ab1-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="26ab1-103">IndexedFieldURI</span></span>

<span data-ttu-id="26ab1-104">O elemento **IndexedFieldURI** identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="26ab1-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="26ab1-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="26ab1-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26ab1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="26ab1-106">Attributes and elements</span></span>

<span data-ttu-id="26ab1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26ab1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26ab1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="26ab1-108">Attributes</span></span>

|<span data-ttu-id="26ab1-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="26ab1-109">**Attribute**</span></span>|<span data-ttu-id="26ab1-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26ab1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="26ab1-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="26ab1-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="26ab1-112">Identifica o dicionário que contém o membro para retornar.</span><span class="sxs-lookup"><span data-stu-id="26ab1-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="26ab1-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="26ab1-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="26ab1-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="26ab1-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="26ab1-115">Identifica o membro do dicionário para retornar.</span><span class="sxs-lookup"><span data-stu-id="26ab1-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="26ab1-116">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="26ab1-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="26ab1-117">Atributo FieldURI</span><span class="sxs-lookup"><span data-stu-id="26ab1-117">FieldURI Attribute</span></span>

|<span data-ttu-id="26ab1-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="26ab1-118">**Value**</span></span>|<span data-ttu-id="26ab1-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26ab1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="26ab1-120">item: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="26ab1-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="26ab1-121">Representa o cabeçalho da mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="26ab1-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="26ab1-122">Contatos: ImAddress</span><span class="sxs-lookup"><span data-stu-id="26ab1-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="26ab1-123">Representa o endereço de um contato de mensagens instantâneas.</span><span class="sxs-lookup"><span data-stu-id="26ab1-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-124">Contatos: PhysicalAddress:Street</span><span class="sxs-lookup"><span data-stu-id="26ab1-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="26ab1-125">Representa o endereço de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-126">Contatos: PhysicalAddress:City</span><span class="sxs-lookup"><span data-stu-id="26ab1-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="26ab1-127">Representa a cidade de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-128">Contatos: PhysicalAddress:State</span><span class="sxs-lookup"><span data-stu-id="26ab1-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="26ab1-129">Representa o estado de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-130">Contatos: PhysicalAddress:Country</span><span class="sxs-lookup"><span data-stu-id="26ab1-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="26ab1-131">Representa o país/região de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-132">Contatos: PhysicalAddress:PostalCode</span><span class="sxs-lookup"><span data-stu-id="26ab1-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="26ab1-133">Representa o código postal de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-134">Contatos: PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="26ab1-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="26ab1-135">Representa o número de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-136">Contatos: EmailAddress</span><span class="sxs-lookup"><span data-stu-id="26ab1-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="26ab1-137">Representa o endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="26ab1-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="26ab1-138">DistributionList:Members:Member</span><span class="sxs-lookup"><span data-stu-id="26ab1-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="26ab1-139">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="26ab1-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="26ab1-140">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26ab1-140">Child elements</span></span>

<span data-ttu-id="26ab1-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26ab1-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26ab1-142">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26ab1-142">Parent elements</span></span>

|<span data-ttu-id="26ab1-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26ab1-143">**Element**</span></span>|<span data-ttu-id="26ab1-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26ab1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26ab1-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="26ab1-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="26ab1-146">Identifica as propriedades adicionais para obter, definir ou criar.</span><span class="sxs-lookup"><span data-stu-id="26ab1-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="26ab1-147">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="26ab1-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="26ab1-148">Representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupada.</span><span class="sxs-lookup"><span data-stu-id="26ab1-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="26ab1-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="26ab1-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="26ab1-150">Especifica um agrupamento arbitrário para consultas FindItem.</span><span class="sxs-lookup"><span data-stu-id="26ab1-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26ab1-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="26ab1-151">Remarks</span></span>

<span data-ttu-id="26ab1-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26ab1-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26ab1-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="26ab1-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26ab1-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="26ab1-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26ab1-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26ab1-155">Schema Name</span></span>  <br/> |<span data-ttu-id="26ab1-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="26ab1-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="26ab1-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26ab1-157">Validation File</span></span>  <br/> |<span data-ttu-id="26ab1-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26ab1-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26ab1-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="26ab1-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="26ab1-160">False</span><span class="sxs-lookup"><span data-stu-id="26ab1-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26ab1-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="26ab1-161">See also</span></span>



- [<span data-ttu-id="26ab1-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26ab1-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

