---
title: CarPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ad096246-113c-42ea-9e63-861b546003e8
description: O elemento de telefone do carro Especifica uma matriz de números de telefone de carro e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 694b3578e127a84dfd2fb844c6e81b28553b687c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751378"
---
# <a name="carphones"></a><span data-ttu-id="a39a9-103">CarPhones</span><span class="sxs-lookup"><span data-stu-id="a39a9-103">CarPhones</span></span>

<span data-ttu-id="a39a9-104">O elemento de **telefone do carro** Especifica uma matriz de números de telefone de carro e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="a39a9-104">The **CarPhone** element specifies an array of car phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CarPhones>
    <Value></Value>
    <Attributions></Attributions>
</CarPhones>
```

 <span data-ttu-id="a39a9-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="a39a9-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a39a9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a39a9-106">Attributes and elements</span></span>

<span data-ttu-id="a39a9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a39a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a39a9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a39a9-108">Attributes</span></span>

<span data-ttu-id="a39a9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a39a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a39a9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a39a9-110">Child elements</span></span>

|<span data-ttu-id="a39a9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a39a9-111">**Element**</span></span>|<span data-ttu-id="a39a9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a39a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a39a9-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="a39a9-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="a39a9-114">Especifica uma telefone número e digite as informações e é associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="a39a9-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="a39a9-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="a39a9-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="a39a9-116">Especifica uma matriz de atribuições para seu elemento **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="a39a9-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a39a9-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a39a9-117">Parent elements</span></span>

|<span data-ttu-id="a39a9-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a39a9-118">**Element**</span></span>|<span data-ttu-id="a39a9-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a39a9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a39a9-120">Pessoa</span><span class="sxs-lookup"><span data-stu-id="a39a9-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a39a9-121">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a39a9-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a39a9-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a39a9-122">Remarks</span></span>

<span data-ttu-id="a39a9-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a39a9-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a39a9-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a39a9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a39a9-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a39a9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a39a9-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a39a9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a39a9-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a39a9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a39a9-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="a39a9-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="a39a9-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a39a9-129">Validation File</span></span>  <br/> |<span data-ttu-id="a39a9-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a39a9-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a39a9-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a39a9-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a39a9-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="a39a9-132">See also</span></span>



- [<span data-ttu-id="a39a9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a39a9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

