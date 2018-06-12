---
title: HomePhones2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba9bb159-362d-48e0-889d-823cb46ecebf
description: O elemento HomePhones2 Especifica uma matriz de valores de HomePhone2 e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 205f2f71421a0dfc7d0057412529bcefdb6636d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823842"
---
# <a name="homephones2"></a><span data-ttu-id="ee94c-103">HomePhones2</span><span class="sxs-lookup"><span data-stu-id="ee94c-103">HomePhones2</span></span>

<span data-ttu-id="ee94c-104">O elemento **HomePhones2** Especifica uma matriz de valores de **HomePhone2** e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="ee94c-104">The **HomePhones2** element specifies an array of **HomePhone2** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones2>
    <PhoneNumberAttributedValue/>
</HomePhones2>
```

 <span data-ttu-id="ee94c-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="ee94c-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee94c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ee94c-106">Attributes and elements</span></span>

<span data-ttu-id="ee94c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee94c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee94c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee94c-108">Attributes</span></span>

<span data-ttu-id="ee94c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee94c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee94c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee94c-110">Child elements</span></span>

|<span data-ttu-id="ee94c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee94c-111">**Element**</span></span>|<span data-ttu-id="ee94c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee94c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee94c-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ee94c-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="ee94c-114">Contém um número de telefone atribuído único para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="ee94c-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee94c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee94c-115">Parent elements</span></span>

|<span data-ttu-id="ee94c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee94c-116">**Element**</span></span>|<span data-ttu-id="ee94c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee94c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee94c-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="ee94c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ee94c-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ee94c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee94c-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ee94c-120">Remarks</span></span>

<span data-ttu-id="ee94c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ee94c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ee94c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee94c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee94c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ee94c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee94c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee94c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee94c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee94c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ee94c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="ee94c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ee94c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee94c-127">Validation File</span></span>  <br/> |<span data-ttu-id="ee94c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ee94c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee94c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ee94c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ee94c-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee94c-130">See also</span></span>



- [<span data-ttu-id="ee94c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ee94c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

