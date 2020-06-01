---
title: CompanyNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 615fa52d-86ff-4630-b188-5fdb9391eee2
description: O elemento companyNames contém uma matriz de nomes de empresa e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 25daa43873fe00837004217e3f814a7201638450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463255"
---
# <a name="companynames"></a><span data-ttu-id="5d2b9-103">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="5d2b9-103">CompanyNames</span></span>

<span data-ttu-id="5d2b9-104">O elemento **companyNames** contém uma matriz de nomes de empresa e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="5d2b9-104">The **CompanyNames** element contains an array of company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<CompanyNames>
    <StringAttributedValue></StringAttributedValue>
</CompanyNames>
```

 <span data-ttu-id="5d2b9-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="5d2b9-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d2b9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5d2b9-106">Attributes and elements</span></span>

<span data-ttu-id="5d2b9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d2b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d2b9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d2b9-108">Attributes</span></span>

<span data-ttu-id="5d2b9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d2b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d2b9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d2b9-110">Child elements</span></span>

|<span data-ttu-id="5d2b9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d2b9-111">**Element**</span></span>|<span data-ttu-id="5d2b9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d2b9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d2b9-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="5d2b9-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="5d2b9-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="5d2b9-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d2b9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d2b9-115">Parent elements</span></span>

|<span data-ttu-id="5d2b9-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d2b9-116">**Element**</span></span>|<span data-ttu-id="5d2b9-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d2b9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d2b9-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="5d2b9-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="5d2b9-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="5d2b9-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d2b9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d2b9-120">Remarks</span></span>

<span data-ttu-id="5d2b9-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5d2b9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5d2b9-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d2b9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d2b9-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5d2b9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d2b9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d2b9-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d2b9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d2b9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5d2b9-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="5d2b9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="5d2b9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d2b9-127">Validation File</span></span>  <br/> |<span data-ttu-id="5d2b9-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5d2b9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d2b9-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5d2b9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5d2b9-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="5d2b9-130">See also</span></span>



- [<span data-ttu-id="5d2b9-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5d2b9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

