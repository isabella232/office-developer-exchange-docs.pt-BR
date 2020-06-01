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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462224"
---
# <a name="carphones"></a><span data-ttu-id="9dca5-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="9dca5-103">CarPhones</span></span>

<span data-ttu-id="9dca5-104">O elemento **CarPhone** especifica uma matriz de números de telefone de carros e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="9dca5-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="9dca5-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9dca5-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9dca5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9dca5-106">Attributes and elements</span></span>

<span data-ttu-id="9dca5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9dca5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9dca5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9dca5-108">Attributes</span></span>

<span data-ttu-id="9dca5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9dca5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9dca5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9dca5-110">Child elements</span></span>

|<span data-ttu-id="9dca5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9dca5-111">**Element**</span></span>|<span data-ttu-id="9dca5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9dca5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dca5-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="9dca5-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="9dca5-114">Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="9dca5-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="9dca5-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="9dca5-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="9dca5-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="9dca5-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9dca5-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9dca5-117">Parent elements</span></span>

|<span data-ttu-id="9dca5-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9dca5-118">**Element**</span></span>|<span data-ttu-id="9dca5-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9dca5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dca5-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="9dca5-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9dca5-121">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="9dca5-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9dca5-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9dca5-122">Remarks</span></span>

<span data-ttu-id="9dca5-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9dca5-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9dca5-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9dca5-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9dca5-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9dca5-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9dca5-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="9dca5-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9dca5-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9dca5-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9dca5-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="9dca5-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="9dca5-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9dca5-129">Validation File</span></span>  <br/> |<span data-ttu-id="9dca5-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9dca5-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9dca5-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9dca5-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9dca5-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9dca5-132">See also</span></span>



- [<span data-ttu-id="9dca5-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9dca5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

