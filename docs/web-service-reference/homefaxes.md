---
title: HomeFaxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 459ddb1c-8cff-4125-b6fa-dc93c183dee8
description: O elemento HomeFaxes Especifica uma matriz de números de fax residencial e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: dd2cd8bba2c4cc7d08e88787d648e96ea996a251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823840"
---
# <a name="homefaxes"></a><span data-ttu-id="ddd64-103">HomeFaxes</span><span class="sxs-lookup"><span data-stu-id="ddd64-103">HomeFaxes</span></span>

<span data-ttu-id="ddd64-104">O elemento **HomeFaxes** Especifica uma matriz de números de fax residencial e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="ddd64-104">The **HomeFaxes** element specifies an array of home fax numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomeFaxes>
    <PhoneNumberAttributedValue/>
</HomeFaxes>
```

 <span data-ttu-id="ddd64-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="ddd64-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ddd64-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ddd64-106">Attributes and elements</span></span>

<span data-ttu-id="ddd64-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ddd64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddd64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ddd64-108">Attributes</span></span>

<span data-ttu-id="ddd64-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ddd64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddd64-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ddd64-110">Child elements</span></span>

|<span data-ttu-id="ddd64-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ddd64-111">**Element**</span></span>|<span data-ttu-id="ddd64-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ddd64-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddd64-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ddd64-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="ddd64-114">Contém um número de telefone atribuído único para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="ddd64-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ddd64-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ddd64-115">Parent elements</span></span>

|<span data-ttu-id="ddd64-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ddd64-116">**Element**</span></span>|<span data-ttu-id="ddd64-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ddd64-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddd64-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="ddd64-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ddd64-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ddd64-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ddd64-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ddd64-120">Remarks</span></span>

<span data-ttu-id="ddd64-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ddd64-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ddd64-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddd64-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ddd64-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ddd64-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ddd64-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ddd64-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ddd64-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ddd64-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ddd64-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="ddd64-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ddd64-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ddd64-127">Validation File</span></span>  <br/> |<span data-ttu-id="ddd64-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ddd64-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ddd64-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ddd64-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ddd64-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ddd64-130">See also</span></span>



- [<span data-ttu-id="ddd64-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ddd64-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

