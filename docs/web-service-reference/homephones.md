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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823844"
---
# <a name="homephones"></a><span data-ttu-id="a3e12-103">HomePhones</span><span class="sxs-lookup"><span data-stu-id="a3e12-103">HomePhones</span></span>

<span data-ttu-id="a3e12-104">O elemento **HomePhones** Especifica uma matriz de números de telefone residencial e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="a3e12-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="a3e12-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="a3e12-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3e12-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a3e12-106">Attributes and elements</span></span>

<span data-ttu-id="a3e12-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3e12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3e12-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3e12-108">Attributes</span></span>

<span data-ttu-id="a3e12-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3e12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3e12-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3e12-110">Child elements</span></span>

|<span data-ttu-id="a3e12-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3e12-111">**Element**</span></span>|<span data-ttu-id="a3e12-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3e12-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3e12-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="a3e12-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="a3e12-114">Contém um número de telefone atribuído único para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="a3e12-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3e12-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3e12-115">Parent elements</span></span>

|<span data-ttu-id="a3e12-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3e12-116">**Element**</span></span>|<span data-ttu-id="a3e12-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3e12-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3e12-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="a3e12-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a3e12-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="a3e12-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3e12-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3e12-120">Remarks</span></span>

<span data-ttu-id="a3e12-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a3e12-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a3e12-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a3e12-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3e12-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a3e12-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3e12-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3e12-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3e12-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3e12-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a3e12-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="a3e12-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a3e12-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3e12-127">Validation File</span></span>  <br/> |<span data-ttu-id="a3e12-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3e12-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3e12-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a3e12-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a3e12-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="a3e12-130">See also</span></span>



- [<span data-ttu-id="a3e12-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a3e12-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

