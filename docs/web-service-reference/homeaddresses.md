---
title: HomeAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: O elemento HomeAddresses especifica uma matriz de endereços residenciais e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: d6a1808bf000ac8bca1e2ce7865aa099037c5a5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460887"
---
# <a name="homeaddresses"></a><span data-ttu-id="9b5af-103">HomeAddresses</span><span class="sxs-lookup"><span data-stu-id="9b5af-103">HomeAddresses</span></span>

<span data-ttu-id="9b5af-104">O elemento **HomeAddresses** especifica uma matriz de endereços residenciais e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="9b5af-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="9b5af-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9b5af-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b5af-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9b5af-106">Attributes and elements</span></span>

<span data-ttu-id="9b5af-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9b5af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b5af-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9b5af-108">Attributes</span></span>

<span data-ttu-id="9b5af-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b5af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b5af-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9b5af-110">Child elements</span></span>

|<span data-ttu-id="9b5af-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b5af-111">**Element**</span></span>|<span data-ttu-id="9b5af-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b5af-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b5af-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9b5af-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="9b5af-114">Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="9b5af-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b5af-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9b5af-115">Parent elements</span></span>

|<span data-ttu-id="9b5af-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b5af-116">**Element**</span></span>|<span data-ttu-id="9b5af-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b5af-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b5af-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="9b5af-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9b5af-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="9b5af-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b5af-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b5af-120">Remarks</span></span>

<span data-ttu-id="9b5af-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9b5af-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9b5af-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b5af-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b5af-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9b5af-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b5af-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b5af-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b5af-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9b5af-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9b5af-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="9b5af-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9b5af-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9b5af-127">Validation File</span></span>  <br/> |<span data-ttu-id="9b5af-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b5af-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b5af-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9b5af-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9b5af-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9b5af-130">See also</span></span>



- [<span data-ttu-id="9b5af-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9b5af-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

