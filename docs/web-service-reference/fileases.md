---
title: FileAses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81efc37-bb70-4d52-a614-cec87d1b0f04
description: O elemento FileAses especifica uma matriz de elementos StringAttributedValue e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 9d97c2c7210e9ae20326d7327c9de4159d5df5a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461076"
---
# <a name="fileases"></a><span data-ttu-id="5fc26-103">FileAses</span><span class="sxs-lookup"><span data-stu-id="5fc26-103">FileAses</span></span>

<span data-ttu-id="5fc26-104">O elemento **FileAses** especifica uma matriz de elementos **StringAttributedValue** e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="5fc26-104">The **FileAses** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAses>
    <StringAttributedValue/>
</FileAses>
```

 <span data-ttu-id="5fc26-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="5fc26-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fc26-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5fc26-106">Attributes and elements</span></span>

<span data-ttu-id="5fc26-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5fc26-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fc26-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5fc26-108">Attributes</span></span>

<span data-ttu-id="5fc26-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fc26-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fc26-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5fc26-110">Child elements</span></span>

|<span data-ttu-id="5fc26-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5fc26-111">**Element**</span></span>|<span data-ttu-id="5fc26-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5fc26-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fc26-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="5fc26-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="5fc26-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="5fc26-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fc26-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5fc26-115">Parent elements</span></span>

|<span data-ttu-id="5fc26-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5fc26-116">**Element**</span></span>|<span data-ttu-id="5fc26-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5fc26-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fc26-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="5fc26-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="5fc26-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="5fc26-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5fc26-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="5fc26-120">Remarks</span></span>

<span data-ttu-id="5fc26-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5fc26-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5fc26-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fc26-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fc26-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5fc26-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fc26-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5fc26-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5fc26-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5fc26-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5fc26-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="5fc26-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="5fc26-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5fc26-127">Validation File</span></span>  <br/> |<span data-ttu-id="5fc26-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5fc26-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5fc26-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5fc26-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5fc26-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="5fc26-130">See also</span></span>



- [<span data-ttu-id="5fc26-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5fc26-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

