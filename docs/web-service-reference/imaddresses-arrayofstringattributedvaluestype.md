---
title: ImAddresses (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: O elemento imaddresss especifica uma matriz de endereços de mensagens instantâneas e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 6714af5d88e50047f48da2f10dbb33d2e2feb724
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460439"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="2ca04-103">ImAddresses (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="2ca04-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="2ca04-104">O elemento **Imaddresss** especifica uma matriz de endereços de mensagens instantâneas e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="2ca04-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="2ca04-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2ca04-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ca04-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2ca04-106">Attributes and elements</span></span>

<span data-ttu-id="2ca04-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2ca04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ca04-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2ca04-108">Attributes</span></span>

<span data-ttu-id="2ca04-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ca04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ca04-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2ca04-110">Child elements</span></span>

|<span data-ttu-id="2ca04-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2ca04-111">**Element**</span></span>|<span data-ttu-id="2ca04-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2ca04-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ca04-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2ca04-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="2ca04-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="2ca04-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ca04-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2ca04-115">Parent elements</span></span>

|<span data-ttu-id="2ca04-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2ca04-116">**Element**</span></span>|<span data-ttu-id="2ca04-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2ca04-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ca04-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="2ca04-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2ca04-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="2ca04-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2ca04-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2ca04-120">Remarks</span></span>

<span data-ttu-id="2ca04-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2ca04-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ca04-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ca04-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ca04-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2ca04-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ca04-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2ca04-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ca04-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2ca04-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2ca04-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2ca04-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2ca04-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2ca04-127">Validation File</span></span>  <br/> |<span data-ttu-id="2ca04-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2ca04-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ca04-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2ca04-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2ca04-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="2ca04-130">See also</span></span>



- [<span data-ttu-id="2ca04-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2ca04-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

