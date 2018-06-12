---
title: CompanyNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 615fa52d-86ff-4630-b188-5fdb9391eee2
description: O elemento CompanyNames contém uma matriz de nomes de empresa e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: b9024b08cb46d2ccbfcc7b07acb4645894cc5f4c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751402"
---
# <a name="companynames"></a><span data-ttu-id="4de1c-103">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="4de1c-103">CompanyNames</span></span>

<span data-ttu-id="4de1c-104">O elemento **CompanyNames** contém uma matriz de nomes de empresa e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="4de1c-104">The **CompanyNames** element contains an array of company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CompanyNames>
    <StringAttributedValue></StringAttributedValue>
</CompanyNames>
```

 <span data-ttu-id="4de1c-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4de1c-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4de1c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4de1c-106">Attributes and elements</span></span>

<span data-ttu-id="4de1c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4de1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4de1c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4de1c-108">Attributes</span></span>

<span data-ttu-id="4de1c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4de1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4de1c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4de1c-110">Child elements</span></span>

|<span data-ttu-id="4de1c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4de1c-111">**Element**</span></span>|<span data-ttu-id="4de1c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4de1c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4de1c-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4de1c-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4de1c-114">Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="4de1c-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4de1c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4de1c-115">Parent elements</span></span>

|<span data-ttu-id="4de1c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4de1c-116">**Element**</span></span>|<span data-ttu-id="4de1c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4de1c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4de1c-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="4de1c-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4de1c-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="4de1c-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4de1c-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4de1c-120">Remarks</span></span>

<span data-ttu-id="4de1c-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4de1c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4de1c-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4de1c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4de1c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4de1c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4de1c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4de1c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4de1c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4de1c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4de1c-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4de1c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4de1c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4de1c-127">Validation File</span></span>  <br/> |<span data-ttu-id="4de1c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4de1c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4de1c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4de1c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4de1c-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="4de1c-130">See also</span></span>



- [<span data-ttu-id="4de1c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4de1c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

