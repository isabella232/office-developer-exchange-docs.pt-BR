---
title: Departamentos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0a6b0a4-f0dd-4945-af69-628da93f5452
description: O elemento de departamentos Especifica uma matriz de nomes de departamento e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 1f969c069cdbe4318c5692fc91615c184451af64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751777"
---
# <a name="departments"></a><span data-ttu-id="ade36-103">Departamentos</span><span class="sxs-lookup"><span data-stu-id="ade36-103">Departments</span></span>

<span data-ttu-id="ade36-104">O elemento de **departamentos** Especifica uma matriz de nomes de departamento e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="ade36-104">The **Departments** element specifies an array of department names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Departments>
    <StringAttributedValue></StringAttributedValue>
</Departments>
```

 <span data-ttu-id="ade36-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="ade36-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ade36-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ade36-106">Attributes and elements</span></span>

<span data-ttu-id="ade36-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ade36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ade36-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ade36-108">Attributes</span></span>

<span data-ttu-id="ade36-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ade36-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ade36-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ade36-110">Child elements</span></span>

|<span data-ttu-id="ade36-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ade36-111">**Element**</span></span>|<span data-ttu-id="ade36-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ade36-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ade36-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ade36-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="ade36-114">Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="ade36-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ade36-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ade36-115">Parent elements</span></span>

|<span data-ttu-id="ade36-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ade36-116">**Element**</span></span>|<span data-ttu-id="ade36-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ade36-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ade36-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="ade36-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="ade36-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="ade36-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ade36-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ade36-120">Remarks</span></span>

<span data-ttu-id="ade36-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ade36-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ade36-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ade36-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ade36-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ade36-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ade36-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ade36-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ade36-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ade36-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ade36-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="ade36-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ade36-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ade36-127">Validation File</span></span>  <br/> |<span data-ttu-id="ade36-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ade36-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ade36-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ade36-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ade36-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ade36-130">See also</span></span>

- [<span data-ttu-id="ade36-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ade36-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

