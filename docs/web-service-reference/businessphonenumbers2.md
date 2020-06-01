---
title: BusinessPhoneNumbers2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f335ea74-9b5b-4224-9475-40ef33fe76bd
description: O elemento BusinessPhoneNumbers2 especifica uma matriz de elementos BusinessPhoneNumber2 e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: c8879e3f7ab996d7e761a72b7ce5f332a9006aed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461601"
---
# <a name="businessphonenumbers2"></a><span data-ttu-id="5bb44-103">BusinessPhoneNumbers2</span><span class="sxs-lookup"><span data-stu-id="5bb44-103">BusinessPhoneNumbers2</span></span>

<span data-ttu-id="5bb44-104">O elemento **BusinessPhoneNumbers2** especifica uma matriz de elementos **BusinessPhoneNumber2** e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="5bb44-104">The **BusinessPhoneNumbers2** element specifies an array of **BusinessPhoneNumber2** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessPhoneNumbers2>
    <Value></Value>
    <Attributions></Attributions>
</BusinessPhoneNumbers2>
```

 <span data-ttu-id="5bb44-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="5bb44-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5bb44-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5bb44-106">Attributes and elements</span></span>

<span data-ttu-id="5bb44-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5bb44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bb44-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5bb44-108">Attributes</span></span>

<span data-ttu-id="5bb44-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5bb44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bb44-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5bb44-110">Child elements</span></span>

|<span data-ttu-id="5bb44-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5bb44-111">**Element**</span></span>|<span data-ttu-id="5bb44-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bb44-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bb44-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="5bb44-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="5bb44-114">Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="5bb44-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="5bb44-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="5bb44-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="5bb44-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="5bb44-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5bb44-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5bb44-117">Parent elements</span></span>

|<span data-ttu-id="5bb44-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5bb44-118">**Element**</span></span>|<span data-ttu-id="5bb44-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bb44-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bb44-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="5bb44-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="5bb44-121">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="5bb44-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bb44-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="5bb44-122">Remarks</span></span>

<span data-ttu-id="5bb44-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5bb44-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5bb44-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5bb44-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bb44-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5bb44-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bb44-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="5bb44-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bb44-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5bb44-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5bb44-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="5bb44-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="5bb44-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5bb44-129">Validation File</span></span>  <br/> |<span data-ttu-id="5bb44-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5bb44-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bb44-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5bb44-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5bb44-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="5bb44-132">See also</span></span>



- [<span data-ttu-id="5bb44-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5bb44-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

