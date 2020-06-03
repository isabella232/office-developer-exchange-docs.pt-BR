---
title: CallbackPhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a7c1377-aac3-42c5-820f-d01cd8e9cf5c
description: O elemento CallbackPhones especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 79d74beffb8de8981e042b0c80e1aa5505a1048c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529459"
---
# <a name="callbackphones"></a><span data-ttu-id="0a8db-103">CallbackPhones</span><span class="sxs-lookup"><span data-stu-id="0a8db-103">CallbackPhones</span></span>

<span data-ttu-id="0a8db-104">O elemento **CallbackPhones** especifica uma matriz de números de telefone de retorno de chamada e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="0a8db-104">The **CallbackPhones** element specifies an array of call-back phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CallbackPhones>
    <Value></Value>
    <Attributions></Attributions>
</CallbackPhones>
```

 <span data-ttu-id="0a8db-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="0a8db-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a8db-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0a8db-106">Attributes and elements</span></span>

<span data-ttu-id="0a8db-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0a8db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a8db-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0a8db-108">Attributes</span></span>

<span data-ttu-id="0a8db-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a8db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a8db-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0a8db-110">Child elements</span></span>

|<span data-ttu-id="0a8db-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a8db-111">**Element**</span></span>|<span data-ttu-id="0a8db-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a8db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a8db-113">Valor (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="0a8db-113">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md) <br/> |<span data-ttu-id="0a8db-114">Especifica um número de telefone e informações de tipo e está associado a um conjunto de atribuições.</span><span class="sxs-lookup"><span data-stu-id="0a8db-114">Specifies a phone number and type information and is associated with a set of attributions.</span></span>  <br/> |
|[<span data-ttu-id="0a8db-115">Atribuições (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0a8db-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="0a8db-116">Especifica uma matriz de atribuições para o elemento de **valor** associado.</span><span class="sxs-lookup"><span data-stu-id="0a8db-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a8db-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0a8db-117">Parent elements</span></span>

|<span data-ttu-id="0a8db-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a8db-118">**Element**</span></span>|<span data-ttu-id="0a8db-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a8db-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a8db-120">Pessoal</span><span class="sxs-lookup"><span data-stu-id="0a8db-120">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0a8db-121">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="0a8db-121">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a8db-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="0a8db-122">Remarks</span></span>

<span data-ttu-id="0a8db-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0a8db-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0a8db-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a8db-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a8db-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0a8db-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a8db-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a8db-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a8db-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0a8db-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0a8db-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="0a8db-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="0a8db-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0a8db-129">Validation File</span></span>  <br/> |<span data-ttu-id="0a8db-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0a8db-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a8db-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0a8db-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0a8db-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="0a8db-132">See also</span></span>



- [<span data-ttu-id="0a8db-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0a8db-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

