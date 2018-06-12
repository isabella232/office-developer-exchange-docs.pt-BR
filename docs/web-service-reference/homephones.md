---
title: HomePhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: O elemento HomePhones Especifica uma matriz de números de telefone residencial e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 487d37e6a18bbd480a814de7570b0789f148096e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823844"
---
# <a name="homephones"></a><span data-ttu-id="f072e-103">HomePhones</span><span class="sxs-lookup"><span data-stu-id="f072e-103">HomePhones</span></span>

<span data-ttu-id="f072e-104">O elemento **HomePhones** Especifica uma matriz de números de telefone residencial e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="f072e-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="f072e-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="f072e-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f072e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f072e-106">Attributes and elements</span></span>

<span data-ttu-id="f072e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f072e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f072e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f072e-108">Attributes</span></span>

<span data-ttu-id="f072e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f072e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f072e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f072e-110">Child elements</span></span>

|<span data-ttu-id="f072e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f072e-111">**Element**</span></span>|<span data-ttu-id="f072e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f072e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f072e-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f072e-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="f072e-114">Contém um número de telefone atribuído único para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="f072e-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f072e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f072e-115">Parent elements</span></span>

|<span data-ttu-id="f072e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f072e-116">**Element**</span></span>|<span data-ttu-id="f072e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f072e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f072e-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="f072e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f072e-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="f072e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f072e-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f072e-120">Remarks</span></span>

<span data-ttu-id="f072e-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f072e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f072e-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f072e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f072e-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f072e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f072e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f072e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f072e-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f072e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f072e-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="f072e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f072e-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f072e-127">Validation File</span></span>  <br/> |<span data-ttu-id="f072e-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f072e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f072e-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f072e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f072e-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="f072e-130">See also</span></span>



- [<span data-ttu-id="f072e-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f072e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

