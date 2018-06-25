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
description: O elemento de entrada descreve um único endereço físico para um item de contato.
ms.openlocfilehash: 4551e6117e5f91d901fe160f37e8f67cb1bc5ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752079"
---
# <a name="entry-physicaladdress"></a><span data-ttu-id="b557f-103">Entrada (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="b557f-103">Entry (PhysicalAddress)</span></span>

<span data-ttu-id="b557f-104">O elemento de **entrada** descreve um único endereço físico para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-104">The **Entry** element describes a single physical address for a contact item.</span></span> 
  
```xml
<Entry Key="">
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
</Entry>
```

 <span data-ttu-id="b557f-105">**PhysicalAddressDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="b557f-105">**PhysicalAddressDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b557f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b557f-106">Attributes and elements</span></span>

<span data-ttu-id="b557f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b557f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b557f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b557f-108">Attributes</span></span>

|<span data-ttu-id="b557f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="b557f-109">**Attribute**</span></span>|<span data-ttu-id="b557f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b557f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b557f-111">**Key**</span><span class="sxs-lookup"><span data-stu-id="b557f-111">**Key**</span></span> <br/> | <span data-ttu-id="b557f-112">Identifica um endereço físico.</span><span class="sxs-lookup"><span data-stu-id="b557f-112">Identifies a physical address.</span></span><br/><br/> <span data-ttu-id="b557f-113">Estes são os valores possíveis para este atributo:</span><span class="sxs-lookup"><span data-stu-id="b557f-113">The following are the possible values for this attribute:</span></span><br/>  <br/><span data-ttu-id="b557f-114">-Business</span><span class="sxs-lookup"><span data-stu-id="b557f-114">-  Business</span></span>  <br/><span data-ttu-id="b557f-115">-Home</span><span class="sxs-lookup"><span data-stu-id="b557f-115">-  Home</span></span>  <br/><span data-ttu-id="b557f-116">-Outros</span><span class="sxs-lookup"><span data-stu-id="b557f-116">-  Other</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b557f-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b557f-117">Child elements</span></span>

|<span data-ttu-id="b557f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b557f-118">**Element**</span></span>|<span data-ttu-id="b557f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b557f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b557f-120">Rua</span><span class="sxs-lookup"><span data-stu-id="b557f-120">Street</span></span>](street.md) <br/> |<span data-ttu-id="b557f-121">Representa um endereço para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-121">Represents a street address for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="b557f-122">Cidade</span><span class="sxs-lookup"><span data-stu-id="b557f-122">City</span></span>](city.md) <br/> |<span data-ttu-id="b557f-123">Representa o nome da cidade que está associado um contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-123">Represents the city name that is associated with a contact.</span></span>  <br/> |
|[<span data-ttu-id="b557f-124">Estado</span><span class="sxs-lookup"><span data-stu-id="b557f-124">State</span></span>](state-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b557f-125">Representa o estado de residência para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-125">Represents the state of residence for a contact item.</span></span>  <br/> |
|[<span data-ttu-id="b557f-126">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b557f-126">CountryOrRegion</span></span>](countryorregion.md) <br/> |<span data-ttu-id="b557f-127">Representa o país ou região para um determinado endereço físico.</span><span class="sxs-lookup"><span data-stu-id="b557f-127">Represents the country or region for a given physical address.</span></span>  <br/> |
|[<span data-ttu-id="b557f-128">PostalCode</span><span class="sxs-lookup"><span data-stu-id="b557f-128">PostalCode</span></span>](postalcode.md) <br/> |<span data-ttu-id="b557f-129">Representa o código postal para um item de contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-129">Represents the postal code for a contact item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b557f-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b557f-130">Parent elements</span></span>

|<span data-ttu-id="b557f-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b557f-131">**Element**</span></span>|<span data-ttu-id="b557f-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b557f-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b557f-133">PhysicalAddresses</span><span class="sxs-lookup"><span data-stu-id="b557f-133">PhysicalAddresses</span></span>](physicaladdresses.md) <br/> |<span data-ttu-id="b557f-134">Contém uma coleção de endereços físicos que estão associados um contato.</span><span class="sxs-lookup"><span data-stu-id="b557f-134">Contains a collection of physical addresses that are associated with a contact.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b557f-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="b557f-135">Remarks</span></span>

<span data-ttu-id="b557f-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b557f-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b557f-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b557f-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b557f-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="b557f-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b557f-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b557f-139">Schema Name</span></span>  <br/> |<span data-ttu-id="b557f-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b557f-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="b557f-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b557f-141">Validation File</span></span>  <br/> |<span data-ttu-id="b557f-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b557f-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b557f-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b557f-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="b557f-144">False</span><span class="sxs-lookup"><span data-stu-id="b557f-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b557f-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="b557f-145">See also</span></span>

- [<span data-ttu-id="b557f-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b557f-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="b557f-147">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="b557f-147">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="b557f-148">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="b557f-148">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [<span data-ttu-id="b557f-149">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="b557f-149">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

