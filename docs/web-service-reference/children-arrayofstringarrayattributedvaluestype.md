---
title: Filhos (ArrayOfStringArrayAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d37b3fd5-63f1-4003-a6ec-54adfce23d52
description: O elemento filho Especifica uma matriz de nomes de filho e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 7c98e7cb96cecad0d1b5122236b6cd0947c6b3d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751389"
---
# <a name="children-arrayofstringarrayattributedvaluestype"></a><span data-ttu-id="b74cb-103">Filhos (ArrayOfStringArrayAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="b74cb-103">Children (ArrayOfStringArrayAttributedValuesType)</span></span>

<span data-ttu-id="b74cb-104">O elemento **filho** Especifica uma matriz de nomes de filho e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="b74cb-104">The **Children** element specifies an array of child names and identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Children>
    <StringAttributedValue></StringAttributedValue>
</Children>
```

 <span data-ttu-id="b74cb-105">**ArrayOfStringArrayAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b74cb-105">**ArrayOfStringArrayAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b74cb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b74cb-106">Attributes and elements</span></span>

<span data-ttu-id="b74cb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b74cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b74cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b74cb-108">Attributes</span></span>

<span data-ttu-id="b74cb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b74cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b74cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b74cb-110">Child elements</span></span>

|<span data-ttu-id="b74cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b74cb-111">**Element**</span></span>|<span data-ttu-id="b74cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b74cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b74cb-113">StringArrayAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b74cb-113">StringArrayAttributedValue</span></span>](stringarrayattributedvalue.md) <br/> |<span data-ttu-id="b74cb-114">Especifica uma instância de uma matriz de dados de cadeia de caracteres de um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="b74cb-114">Specifies an instance of an array of string data for a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b74cb-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b74cb-115">Parent elements</span></span>

|<span data-ttu-id="b74cb-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b74cb-116">**Element**</span></span>|<span data-ttu-id="b74cb-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b74cb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b74cb-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="b74cb-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b74cb-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b74cb-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b74cb-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="b74cb-120">Remarks</span></span>

<span data-ttu-id="b74cb-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b74cb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b74cb-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b74cb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b74cb-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b74cb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b74cb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b74cb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b74cb-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b74cb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b74cb-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b74cb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b74cb-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b74cb-127">Validation File</span></span>  <br/> |<span data-ttu-id="b74cb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b74cb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b74cb-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b74cb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b74cb-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b74cb-130">See also</span></span>



- [<span data-ttu-id="b74cb-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b74cb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

