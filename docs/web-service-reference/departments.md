---
title: Exiba
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a0a6b0a4-f0dd-4945-af69-628da93f5452
description: O elemento departamentos especifica uma matriz de nomes de departamento e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 17590793e00a914cb53b479994bcc89e37bb0e31
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467932"
---
# <a name="departments"></a><span data-ttu-id="9d17f-103">Exiba</span><span class="sxs-lookup"><span data-stu-id="9d17f-103">Departments</span></span>

<span data-ttu-id="9d17f-104">O elemento **departamentos** especifica uma matriz de nomes de departamento e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="9d17f-104">The **Departments** element specifies an array of department names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Departments>
    <StringAttributedValue></StringAttributedValue>
</Departments>
```

 <span data-ttu-id="9d17f-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="9d17f-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d17f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9d17f-106">Attributes and elements</span></span>

<span data-ttu-id="9d17f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d17f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d17f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d17f-108">Attributes</span></span>

<span data-ttu-id="9d17f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d17f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d17f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d17f-110">Child elements</span></span>

|<span data-ttu-id="9d17f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d17f-111">**Element**</span></span>|<span data-ttu-id="9d17f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d17f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d17f-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9d17f-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="9d17f-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="9d17f-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d17f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d17f-115">Parent elements</span></span>

|<span data-ttu-id="9d17f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d17f-116">**Element**</span></span>|<span data-ttu-id="9d17f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d17f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d17f-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="9d17f-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9d17f-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="9d17f-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d17f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d17f-120">Remarks</span></span>

<span data-ttu-id="9d17f-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9d17f-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d17f-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d17f-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d17f-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9d17f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d17f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d17f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d17f-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d17f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9d17f-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="9d17f-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9d17f-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d17f-127">Validation File</span></span>  <br/> |<span data-ttu-id="9d17f-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9d17f-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d17f-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9d17f-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9d17f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="9d17f-130">See also</span></span>

- [<span data-ttu-id="9d17f-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9d17f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

