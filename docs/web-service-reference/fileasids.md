---
title: FileAsIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 71cae100-b68e-454b-b9b6-ddbcb4d78f3f
description: O elemento FileAsIds especifica uma matriz de elementos StringAttributedValue e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: ecdf30fac345834600439227709504b0d56b988b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461041"
---
# <a name="fileasids"></a><span data-ttu-id="eb624-103">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="eb624-103">FileAsIds</span></span>

<span data-ttu-id="eb624-104">O elemento **FileAsIds** especifica uma matriz de elementos **StringAttributedValue** e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="eb624-104">The **FileAsIds** element specifies an array of **StringAttributedValue** elements and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<FileAsIds>
    <StringAttributedValue/>
<FileAsIds>
```

 <span data-ttu-id="eb624-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="eb624-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb624-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eb624-106">Attributes and elements</span></span>

<span data-ttu-id="eb624-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb624-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb624-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb624-108">Attributes</span></span>

<span data-ttu-id="eb624-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb624-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb624-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb624-110">Child elements</span></span>

|<span data-ttu-id="eb624-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb624-111">**Element**</span></span>|<span data-ttu-id="eb624-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb624-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb624-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="eb624-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="eb624-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="eb624-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb624-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb624-115">Parent elements</span></span>

|<span data-ttu-id="eb624-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb624-116">**Element**</span></span>|<span data-ttu-id="eb624-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb624-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb624-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="eb624-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="eb624-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="eb624-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb624-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb624-120">Remarks</span></span>

<span data-ttu-id="eb624-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="eb624-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eb624-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb624-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb624-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eb624-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb624-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb624-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb624-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb624-125">Schema Name</span></span>  <br/> |<span data-ttu-id="eb624-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="eb624-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="eb624-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb624-127">Validation File</span></span>  <br/> |<span data-ttu-id="eb624-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eb624-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb624-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="eb624-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="eb624-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="eb624-130">See also</span></span>



- [<span data-ttu-id="eb624-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="eb624-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

