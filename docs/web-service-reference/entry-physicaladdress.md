---
title: Entrada (PhysicalAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: 9e5b6515-453e-4f4c-b55e-6ffefe23c31b
description: O elemento ENTRY descreve um único endereço físico para um item de contato.
ms.openlocfilehash: 5e8343e9abebeeff8c2b81327b2e0f4ddcf45364
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459627"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="4fe60-103">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="4fe60-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="4fe60-104">O elemento **entry** descreve um único endereço físico para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="4fe60-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="4fe60-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fe60-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4fe60-106">Attributes and elements</span></span>

<span data-ttu-id="4fe60-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4fe60-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe60-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4fe60-108">Attributes</span></span>

|<span data-ttu-id="4fe60-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="4fe60-109">**Attribute**</span></span>|<span data-ttu-id="4fe60-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fe60-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fe60-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="4fe60-111">**Key**</span></span> <br/> | <span data-ttu-id="4fe60-112">Identifica um endereço físico.</span><span class="sxs-lookup"><span data-stu-id="4fe60-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="4fe60-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="4fe60-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="4fe60-114">-Business</span><span class="sxs-lookup"><span data-stu-id="4fe60-114">-  Business</span></span>  <br/><span data-ttu-id="4fe60-115">-Home</span><span class="sxs-lookup"><span data-stu-id="4fe60-115">-  Home</span></span>  <br/><span data-ttu-id="4fe60-116">-Outros</span><span class="sxs-lookup"><span data-stu-id="4fe60-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4fe60-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4fe60-117">Child elements</span></span>

|<span data-ttu-id="4fe60-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fe60-118">**Element**</span></span>|<span data-ttu-id="4fe60-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fe60-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe60-120">123</span><span class="sxs-lookup"><span data-stu-id="4fe60-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="4fe60-121">Representa um endereço de um item de contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="4fe60-122">Cidade</span><span class="sxs-lookup"><span data-stu-id="4fe60-122">City</span></span>](city.md) <br/> |<span data-ttu-id="4fe60-123">Representa o nome da cidade que está associado a um contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="4fe60-124">State</span><span class="sxs-lookup"><span data-stu-id="4fe60-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4fe60-125">Representa o estado de residência de um item de contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="4fe60-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="4fe60-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="4fe60-127">Representa o país ou a região de um determinado endereço físico.</span><span class="sxs-lookup"><span data-stu-id="4fe60-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="4fe60-128">PostalCode</span><span class="sxs-lookup"><span data-stu-id="4fe60-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="4fe60-129">Representa o código postal de um item de contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fe60-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4fe60-130">Parent elements</span></span>

|<span data-ttu-id="4fe60-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fe60-131">**Element**</span></span>|<span data-ttu-id="4fe60-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fe60-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe60-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="4fe60-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="4fe60-134">Contém uma coleção de endereços físicos associados a um contato.</span><span class="sxs-lookup"><span data-stu-id="4fe60-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fe60-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="4fe60-135">Remarks</span></span>

<span data-ttu-id="4fe60-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4fe60-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fe60-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4fe60-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe60-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fe60-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fe60-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4fe60-139">Schema Name</span></span>  <br/> |<span data-ttu-id="4fe60-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4fe60-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fe60-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4fe60-141">Validation File</span></span>  <br/> |<span data-ttu-id="4fe60-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4fe60-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fe60-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4fe60-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fe60-144">False</span><span class="sxs-lookup"><span data-stu-id="4fe60-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fe60-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="4fe60-145">See also</span></span>

- [<span data-ttu-id="4fe60-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe60-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="4fe60-147">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="4fe60-147">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="4fe60-148">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="4fe60-148">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="4fe60-149">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="4fe60-149">Deleting Contacts</span></span>](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

