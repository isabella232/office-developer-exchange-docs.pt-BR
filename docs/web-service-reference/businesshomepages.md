---
title: BusinessHomePages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9961c0c2-7cac-4af1-84ac-0eafdce0a6ab
description: O elemento BusinessHomePages especifica uma matriz de home pages comerciais e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: f0e85e0b3c857e44d94bd42c6d3ea757d015eb25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465909"
---
# <a name="businesshomepages"></a><span data-ttu-id="4bdd5-103">BusinessHomePages</span><span class="sxs-lookup"><span data-stu-id="4bdd5-103">BusinessHomePages</span></span>

<span data-ttu-id="4bdd5-104">O elemento **BusinessHomePages** especifica uma matriz de home pages comerciais e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="4bdd5-104">The **BusinessHomePages** element specifies an array of business home pages and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessHomePages>
    <StringAttributedValue></StringAttributedValue>
</BusinessHomePages>
```

 <span data-ttu-id="4bdd5-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4bdd5-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bdd5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4bdd5-106">Attributes and elements</span></span>

<span data-ttu-id="4bdd5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4bdd5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bdd5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4bdd5-108">Attributes</span></span>

<span data-ttu-id="4bdd5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bdd5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bdd5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4bdd5-110">Child elements</span></span>

|<span data-ttu-id="4bdd5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4bdd5-111">**Element**</span></span>|<span data-ttu-id="4bdd5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4bdd5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bdd5-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4bdd5-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4bdd5-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="4bdd5-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4bdd5-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4bdd5-115">Parent elements</span></span>

|<span data-ttu-id="4bdd5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4bdd5-116">**Element**</span></span>|<span data-ttu-id="4bdd5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4bdd5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bdd5-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="4bdd5-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4bdd5-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="4bdd5-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bdd5-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4bdd5-120">Remarks</span></span>

<span data-ttu-id="4bdd5-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4bdd5-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4bdd5-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4bdd5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bdd5-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4bdd5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bdd5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bdd5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4bdd5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4bdd5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4bdd5-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4bdd5-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4bdd5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4bdd5-127">Validation File</span></span>  <br/> |<span data-ttu-id="4bdd5-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4bdd5-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4bdd5-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4bdd5-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4bdd5-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="4bdd5-130">See also</span></span>



- [<span data-ttu-id="4bdd5-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4bdd5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

