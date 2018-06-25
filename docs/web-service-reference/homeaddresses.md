---
title: HomeAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57fb1b9d-2ba8-4359-ae79-35c0d56a2d0f
description: O elemento HomeAddresses Especifica uma matriz de endereços residenciais e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: a9d4ceafcac9cf0809668871b4df932b31525ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823817"
---
# <a name="homeaddresses"></a><span data-ttu-id="65c71-103">HomeAddresses</span><span class="sxs-lookup"><span data-stu-id="65c71-103">HomeAddresses</span></span>

<span data-ttu-id="65c71-104">O elemento **HomeAddresses** Especifica uma matriz de endereços residenciais e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="65c71-104">The **HomeAddresses** element specifies an array of home addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeAddresses>
    <PostalAddressAttributedValue/>
</HomeAddresses>
```

 <span data-ttu-id="65c71-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="65c71-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65c71-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="65c71-106">Attributes and elements</span></span>

<span data-ttu-id="65c71-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="65c71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65c71-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="65c71-108">Attributes</span></span>

<span data-ttu-id="65c71-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="65c71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65c71-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="65c71-110">Child elements</span></span>

|<span data-ttu-id="65c71-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="65c71-111">**Element**</span></span>|<span data-ttu-id="65c71-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65c71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65c71-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="65c71-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="65c71-114">Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="65c71-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65c71-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="65c71-115">Parent elements</span></span>

|<span data-ttu-id="65c71-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="65c71-116">**Element**</span></span>|<span data-ttu-id="65c71-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65c71-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65c71-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="65c71-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="65c71-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="65c71-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65c71-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="65c71-120">Remarks</span></span>

<span data-ttu-id="65c71-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="65c71-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="65c71-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="65c71-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65c71-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="65c71-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65c71-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="65c71-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65c71-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="65c71-125">Schema Name</span></span>  <br/> |<span data-ttu-id="65c71-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="65c71-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="65c71-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="65c71-127">Validation File</span></span>  <br/> |<span data-ttu-id="65c71-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65c71-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="65c71-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="65c71-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="65c71-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="65c71-130">See also</span></span>



- [<span data-ttu-id="65c71-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="65c71-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

