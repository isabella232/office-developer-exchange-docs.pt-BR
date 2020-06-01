---
title: Gerações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 637560b5-2b08-4787-a5d8-e0467f83acca
description: O elemento Generations especifica uma matriz de valores de geração e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: a3ef0e2c73e2ebd7c121f817b8ea97c5e4d4d333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463010"
---
# <a name="generations"></a><span data-ttu-id="b8c1e-103">Gerações</span><span class="sxs-lookup"><span data-stu-id="b8c1e-103">Generations</span></span>

<span data-ttu-id="b8c1e-104">O elemento **Generations** especifica uma matriz de valores de geração e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-104">The **Generations** element specifies an array of generation values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Generations>
    <StringAttributedValue/>
</Generations>
```

 <span data-ttu-id="b8c1e-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b8c1e-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8c1e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b8c1e-106">Attributes and elements</span></span>

<span data-ttu-id="b8c1e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8c1e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8c1e-108">Attributes</span></span>

<span data-ttu-id="b8c1e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8c1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8c1e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8c1e-110">Child elements</span></span>

|<span data-ttu-id="b8c1e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8c1e-111">**Element**</span></span>|<span data-ttu-id="b8c1e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8c1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8c1e-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b8c1e-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="b8c1e-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8c1e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8c1e-115">Parent elements</span></span>

|<span data-ttu-id="b8c1e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8c1e-116">**Element**</span></span>|<span data-ttu-id="b8c1e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8c1e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8c1e-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="b8c1e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b8c1e-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="b8c1e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8c1e-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8c1e-120">Remarks</span></span>

<span data-ttu-id="b8c1e-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b8c1e-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8c1e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8c1e-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b8c1e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8c1e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8c1e-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8c1e-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8c1e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b8c1e-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b8c1e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b8c1e-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8c1e-127">Validation File</span></span>  <br/> |<span data-ttu-id="b8c1e-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b8c1e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8c1e-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b8c1e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b8c1e-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b8c1e-130">See also</span></span>



- [<span data-ttu-id="b8c1e-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b8c1e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

