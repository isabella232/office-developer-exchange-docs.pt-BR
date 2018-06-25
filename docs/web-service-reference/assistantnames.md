---
title: AssistantNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: O elemento AssistantNames Especifica uma matriz de nomes de assistente e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 7414caa74dc8221d0b1b471c3d5ed09552f7e200
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751213"
---
# <a name="assistantnames"></a><span data-ttu-id="01f8b-103">AssistantNames</span><span class="sxs-lookup"><span data-stu-id="01f8b-103">AssistantNames</span></span>

<span data-ttu-id="01f8b-104">O elemento **AssistantNames** Especifica uma matriz de nomes de assistente e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="01f8b-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="01f8b-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="01f8b-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01f8b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="01f8b-106">Attributes and elements</span></span>

<span data-ttu-id="01f8b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01f8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01f8b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01f8b-108">Attributes</span></span>

<span data-ttu-id="01f8b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01f8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01f8b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01f8b-110">Child elements</span></span>

|<span data-ttu-id="01f8b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01f8b-111">**Element**</span></span>|<span data-ttu-id="01f8b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01f8b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01f8b-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="01f8b-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="01f8b-114">Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="01f8b-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01f8b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01f8b-115">Parent elements</span></span>

|<span data-ttu-id="01f8b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01f8b-116">**Element**</span></span>|<span data-ttu-id="01f8b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01f8b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01f8b-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="01f8b-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="01f8b-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="01f8b-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="01f8b-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="01f8b-120">Remarks</span></span>

<span data-ttu-id="01f8b-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="01f8b-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="01f8b-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01f8b-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01f8b-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="01f8b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01f8b-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="01f8b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01f8b-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01f8b-125">Schema Name</span></span>  <br/> |<span data-ttu-id="01f8b-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="01f8b-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="01f8b-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01f8b-127">Validation File</span></span>  <br/> |<span data-ttu-id="01f8b-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01f8b-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="01f8b-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="01f8b-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="01f8b-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="01f8b-130">See also</span></span>

- [<span data-ttu-id="01f8b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01f8b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

