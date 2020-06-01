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
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467015"
---
# <a name="indexedfielduri"></a><span data-ttu-id="a0952-103">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="a0952-103">IndexedFieldURI</span></span>

<span data-ttu-id="a0952-104">O elemento **IndexedFieldURI** identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="a0952-104">The **IndexedFieldURI** element identifies individual members of a dictionary.</span></span> 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 <span data-ttu-id="a0952-105">**PathToIndexedFieldType**</span><span class="sxs-lookup"><span data-stu-id="a0952-105">**PathToIndexedFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0952-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a0952-106">Attributes and elements</span></span>

<span data-ttu-id="a0952-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0952-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0952-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0952-108">Attributes</span></span>

|<span data-ttu-id="a0952-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a0952-109">**Attribute**</span></span>|<span data-ttu-id="a0952-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0952-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0952-111">**FieldURI**</span><span class="sxs-lookup"><span data-stu-id="a0952-111">**FieldURI**</span></span> <br/> |<span data-ttu-id="a0952-112">Identifica o dicionário que contém o membro a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a0952-112">Identifies the dictionary that contains the member to return.</span></span> <span data-ttu-id="a0952-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="a0952-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="a0952-114">**FieldIndex**</span><span class="sxs-lookup"><span data-stu-id="a0952-114">**FieldIndex**</span></span> <br/> |<span data-ttu-id="a0952-115">Identifica o membro do dicionário a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a0952-115">Identifies the member of the dictionary to return.</span></span> <span data-ttu-id="a0952-116">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="a0952-116">This attribute is required.</span></span>  <br/> |
   
#### <a name="fielduri-attribute"></a><span data-ttu-id="a0952-117">Atributo FieldURI</span><span class="sxs-lookup"><span data-stu-id="a0952-117">FieldURI Attribute</span></span>

|<span data-ttu-id="a0952-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a0952-118">**Value**</span></span>|<span data-ttu-id="a0952-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0952-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0952-120">item: InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="a0952-120">item:InternetMessageHeader</span></span>  <br/> |<span data-ttu-id="a0952-121">Representa o cabeçalho da mensagem de um item.</span><span class="sxs-lookup"><span data-stu-id="a0952-121">Represents the message header of an item.</span></span>  <br/> |
|<span data-ttu-id="a0952-122">contatos: imendereço</span><span class="sxs-lookup"><span data-stu-id="a0952-122">contacts:ImAddress</span></span>  <br/> |<span data-ttu-id="a0952-123">Representa o endereço de mensagens instantâneas de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-123">Represents the instant messaging address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-124">contatos: PhysicalAddress: rua</span><span class="sxs-lookup"><span data-stu-id="a0952-124">contacts:PhysicalAddress:Street</span></span>  <br/> |<span data-ttu-id="a0952-125">Representa o endereço de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-125">Represents the street address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-126">contatos: PhysicalAddress: cidade</span><span class="sxs-lookup"><span data-stu-id="a0952-126">contacts:PhysicalAddress:City</span></span>  <br/> |<span data-ttu-id="a0952-127">Representa a cidade de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-127">Represents the city of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-128">contatos: PhysicalAddress: State</span><span class="sxs-lookup"><span data-stu-id="a0952-128">contacts:PhysicalAddress:State</span></span>  <br/> |<span data-ttu-id="a0952-129">Representa o estado de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-129">Represents the state of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-130">contatos: PhysicalAddress: país</span><span class="sxs-lookup"><span data-stu-id="a0952-130">contacts:PhysicalAddress:Country</span></span>  <br/> |<span data-ttu-id="a0952-131">Representa o país/região de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-131">Represents the country/region of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-132">contatos: PhysicalAddress: CEP</span><span class="sxs-lookup"><span data-stu-id="a0952-132">contacts:PhysicalAddress:PostalCode</span></span>  <br/> |<span data-ttu-id="a0952-133">Representa o código postal de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-133">Represents the postal code of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-134">contatos: PhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a0952-134">contacts:PhoneNumber</span></span>  <br/> |<span data-ttu-id="a0952-135">Representa o número de telefone de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-135">Represents the phone number of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-136">contatos: EmailAddress</span><span class="sxs-lookup"><span data-stu-id="a0952-136">contacts:EmailAddress</span></span>  <br/> |<span data-ttu-id="a0952-137">Representa o endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="a0952-137">Represents the e-mail address of a contact.</span></span>  <br/> |
|<span data-ttu-id="a0952-138">DistributionList: members: member</span><span class="sxs-lookup"><span data-stu-id="a0952-138">distributionlist:Members:Member</span></span>  <br/> |<span data-ttu-id="a0952-139">Representa um membro de uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="a0952-139">Represents a member of a distribution list.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0952-140">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0952-140">Child elements</span></span>

<span data-ttu-id="a0952-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0952-141">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0952-142">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0952-142">Parent elements</span></span>

|<span data-ttu-id="a0952-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0952-143">**Element**</span></span>|<span data-ttu-id="a0952-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0952-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0952-145">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="a0952-145">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="a0952-146">Identifica propriedades adicionais a serem obtidas, definidas ou criadas.</span><span class="sxs-lookup"><span data-stu-id="a0952-146">Identifies additional properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="a0952-147">Agregar</span><span class="sxs-lookup"><span data-stu-id="a0952-147">AggregateOn</span></span>](aggregateon.md) <br/> |<span data-ttu-id="a0952-148">Representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados de FindItem agrupado.</span><span class="sxs-lookup"><span data-stu-id="a0952-148">Represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span>  <br/> |
|[<span data-ttu-id="a0952-149">GroupBy</span><span class="sxs-lookup"><span data-stu-id="a0952-149">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="a0952-150">Especifica um agrupamento arbitrário para consultas do FindItem.</span><span class="sxs-lookup"><span data-stu-id="a0952-150">Specifies an arbitrary grouping for FindItem queries.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0952-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0952-151">Remarks</span></span>

<span data-ttu-id="a0952-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0952-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0952-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a0952-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0952-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0952-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0952-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0952-155">Schema Name</span></span>  <br/> |<span data-ttu-id="a0952-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a0952-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0952-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0952-157">Validation File</span></span>  <br/> |<span data-ttu-id="a0952-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a0952-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0952-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a0952-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0952-160">False</span><span class="sxs-lookup"><span data-stu-id="a0952-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0952-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="a0952-161">See also</span></span>



- [<span data-ttu-id="a0952-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a0952-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

