---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: O elemento CarPhone especifica uma matriz de números de telefone de carros e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 41d0cc264da69ab17b8ebf109759139c4249719e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462224"
---
# <a name="carphones"></a><span data-ttu-id="95097-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="95097-103">CarPhones</span></span>

<span data-ttu-id="95097-104">O elemento **CarPhone** especifica uma matriz de números de telefone de carros e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="95097-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="95097-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="95097-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95097-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="95097-106">Attributes and elements</span></span>

<span data-ttu-id="95097-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95097-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95097-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="95097-108">Attributes</span></span>

<span data-ttu-id="95097-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95097-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95097-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95097-110">Child elements</span></span>

|<span data-ttu-id="95097-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95097-111">**Element**</span></span>|<span data-ttu-id="95097-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95097-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95097-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="95097-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="95097-114">Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="95097-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="95097-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="95097-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="95097-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="95097-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95097-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95097-117">Parent elements</span></span>

|<span data-ttu-id="95097-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95097-118">**Element**</span></span>|<span data-ttu-id="95097-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95097-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95097-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="95097-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="95097-121">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="95097-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95097-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="95097-122">Remarks</span></span>

<span data-ttu-id="95097-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="95097-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="95097-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95097-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95097-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="95097-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95097-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="95097-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95097-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95097-127">Schema Name</span></span>  <br/> |<span data-ttu-id="95097-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="95097-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="95097-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95097-129">Validation File</span></span>  <br/> |<span data-ttu-id="95097-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95097-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="95097-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="95097-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="95097-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="95097-132">See also</span></span>



- [<span data-ttu-id="95097-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95097-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

