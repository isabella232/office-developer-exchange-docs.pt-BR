---
title: BusinessPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: O elemento BusinessPhoneNumbers Especifica uma matriz de números de telefone comercial e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 692c38a00241da9f753c431612f4a8fcf26cc7ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751337"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="87859-103">BusinessPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="87859-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="87859-104">O elemento **BusinessPhoneNumbers** Especifica uma matriz de números de telefone comercial e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="87859-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="87859-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="87859-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87859-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="87859-106">Attributes and elements</span></span>

<span data-ttu-id="87859-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="87859-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87859-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="87859-108">Attributes</span></span>

<span data-ttu-id="87859-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87859-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87859-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="87859-110">Child elements</span></span>

|<span data-ttu-id="87859-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87859-111">**Element**</span></span>|<span data-ttu-id="87859-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87859-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87859-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="87859-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="87859-114">Especifica uma telefone número e digite as informações e é associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="87859-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="87859-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="87859-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="87859-116">Especifica uma matriz de atribuições para seu elemento **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="87859-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87859-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="87859-117">Parent elements</span></span>

|<span data-ttu-id="87859-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87859-118">**Element**</span></span>|<span data-ttu-id="87859-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87859-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87859-120">Pessoa</span><span class="sxs-lookup"><span data-stu-id="87859-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="87859-121">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="87859-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87859-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="87859-122">Remarks</span></span>

<span data-ttu-id="87859-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="87859-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="87859-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="87859-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87859-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="87859-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87859-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="87859-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87859-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="87859-127">Schema Name</span></span>  <br/> |<span data-ttu-id="87859-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="87859-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="87859-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="87859-129">Validation File</span></span>  <br/> |<span data-ttu-id="87859-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="87859-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="87859-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="87859-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="87859-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="87859-132">See also</span></span>



- [<span data-ttu-id="87859-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87859-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

