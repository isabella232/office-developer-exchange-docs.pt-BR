---
title: Assistentes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4e69022d-1cef-4744-877c-848a0b5c4f40
description: O elemento Assistantnames especifica uma matriz de nomes de assistentes e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: cb3722e07da97ed472f9ae50180d61ed761413c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461538"
---
# <a name="assistantnames"></a><span data-ttu-id="d1574-103">Assistentes</span><span class="sxs-lookup"><span data-stu-id="d1574-103">AssistantNames</span></span>

<span data-ttu-id="d1574-104">O elemento **assistantnames** especifica uma matriz de nomes de assistentes e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="d1574-104">The **AssistantNames** element specifies an array of assistant names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantNames>
    <StringAttributedValue></StringAttributedValue>
</AssistantNames>
```

 <span data-ttu-id="d1574-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="d1574-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1574-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d1574-106">Attributes and elements</span></span>

<span data-ttu-id="d1574-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1574-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1574-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1574-108">Attributes</span></span>

<span data-ttu-id="d1574-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1574-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1574-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1574-110">Child elements</span></span>

|<span data-ttu-id="d1574-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1574-111">**Element**</span></span>|<span data-ttu-id="d1574-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1574-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1574-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d1574-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="d1574-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="d1574-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1574-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1574-115">Parent elements</span></span>

|<span data-ttu-id="d1574-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1574-116">**Element**</span></span>|<span data-ttu-id="d1574-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1574-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1574-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="d1574-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="d1574-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="d1574-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1574-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1574-120">Remarks</span></span>

<span data-ttu-id="d1574-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1574-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1574-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1574-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1574-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d1574-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1574-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1574-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1574-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1574-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d1574-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="d1574-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d1574-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1574-127">Validation File</span></span>  <br/> |<span data-ttu-id="d1574-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d1574-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1574-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d1574-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d1574-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d1574-130">See also</span></span>

- [<span data-ttu-id="d1574-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d1574-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

