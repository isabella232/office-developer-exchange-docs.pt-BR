---
title: CallbackPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: O elemento CallbackPhones Especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 3d7acb5f9d800ac7dfff5a43ca8f19e3d147c7a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751367"
---
# <a name="callbackphones"></a><span data-ttu-id="a36ff-103">CallbackPhones</span><span class="sxs-lookup"><span data-stu-id="a36ff-103">CallbackPhones</span></span>

<span data-ttu-id="a36ff-104">O elemento **CallbackPhones** Especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="a36ff-104">The **CallbackPhones** element specifies an array of call-back phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 <span data-ttu-id="a36ff-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="a36ff-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a36ff-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a36ff-106">Attributes and elements</span></span>

<span data-ttu-id="a36ff-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a36ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a36ff-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a36ff-108">Attributes</span></span>

<span data-ttu-id="a36ff-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a36ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a36ff-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a36ff-110">Child elements</span></span>

|<span data-ttu-id="a36ff-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a36ff-111">**Element**</span></span>|<span data-ttu-id="a36ff-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a36ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a36ff-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="a36ff-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="a36ff-114">Especifica uma telefone número e digite as informações e é associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="a36ff-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="a36ff-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="a36ff-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="a36ff-116">Especifica uma matriz de atribuições para seu elemento **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="a36ff-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a36ff-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a36ff-117">Parent elements</span></span>

|<span data-ttu-id="a36ff-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a36ff-118">**Element**</span></span>|<span data-ttu-id="a36ff-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a36ff-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a36ff-120">Pessoa</span><span class="sxs-lookup"><span data-stu-id="a36ff-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a36ff-121">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a36ff-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a36ff-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a36ff-122">Remarks</span></span>

<span data-ttu-id="a36ff-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a36ff-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a36ff-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a36ff-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a36ff-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a36ff-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a36ff-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a36ff-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a36ff-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a36ff-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a36ff-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="a36ff-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="a36ff-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a36ff-129">Validation File</span></span>  <br/> |<span data-ttu-id="a36ff-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a36ff-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a36ff-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a36ff-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a36ff-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="a36ff-132">See also</span></span>



- [<span data-ttu-id="a36ff-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a36ff-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

