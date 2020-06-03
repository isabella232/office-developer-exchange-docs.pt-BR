---
title: BusinessPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ecbe4f1c-1c9e-44e0-a8f7-08c160a0fddb
description: O elemento BusinessPhoneNumbers especifica uma matriz de números de telefone comercial e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 8713af3ad302a2940cab247ff7188e55e8021ca0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461615"
---
# <a name="businessphonenumbers"></a><span data-ttu-id="2182a-103">BusinessPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="2182a-103">BusinessPhoneNumbers</span></span>

<span data-ttu-id="2182a-104">O elemento **BusinessPhoneNumbers** especifica uma matriz de números de telefone comercial e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="2182a-104">The **BusinessPhoneNumbers** element specifies an array of business phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers>
```

 <span data-ttu-id="2182a-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2182a-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2182a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2182a-106">Attributes and elements</span></span>

<span data-ttu-id="2182a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2182a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2182a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2182a-108">Attributes</span></span>

<span data-ttu-id="2182a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2182a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2182a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2182a-110">Child elements</span></span>

|<span data-ttu-id="2182a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2182a-111">**Element**</span></span>|<span data-ttu-id="2182a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2182a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2182a-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="2182a-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="2182a-114">Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="2182a-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="2182a-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="2182a-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="2182a-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="2182a-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2182a-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2182a-117">Parent elements</span></span>

|<span data-ttu-id="2182a-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2182a-118">**Element**</span></span>|<span data-ttu-id="2182a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2182a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2182a-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="2182a-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2182a-121">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="2182a-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2182a-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="2182a-122">Remarks</span></span>

<span data-ttu-id="2182a-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2182a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2182a-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2182a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2182a-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2182a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2182a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="2182a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2182a-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2182a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2182a-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2182a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="2182a-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2182a-129">Validation File</span></span>  <br/> |<span data-ttu-id="2182a-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2182a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2182a-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2182a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2182a-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="2182a-132">See also</span></span>



- [<span data-ttu-id="2182a-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2182a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

