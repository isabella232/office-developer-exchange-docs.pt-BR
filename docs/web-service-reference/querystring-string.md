---
title: QueryString (cadeia de caracteres)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: O elemento QueryString especifica um conjunto de valores a serem retornados que correspondam à cadeia de caracteres de consulta em uma solicitação de operação FindPeople. Uma pesquisa sem QueryString especificado retorna todos os itens da pasta especificada.
ms.openlocfilehash: ec025f86d3e6fb74810e9c539eba102d05adbb93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465321"
---
# <a name="querystring-string"></a><span data-ttu-id="63bb6-104">QueryString (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="63bb6-104">QueryString (String)</span></span>

<span data-ttu-id="63bb6-105">O elemento **QueryString** especifica um conjunto de valores a serem retornados que correspondam à cadeia de caracteres de consulta em uma solicitação de [operação FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="63bb6-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="63bb6-106">Uma pesquisa sem **QueryString** especificado retorna todos os itens da pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="63bb6-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="63bb6-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="63bb6-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63bb6-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="63bb6-108">Attributes and elements</span></span>

<span data-ttu-id="63bb6-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="63bb6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63bb6-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="63bb6-110">Attributes</span></span>

<span data-ttu-id="63bb6-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63bb6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63bb6-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="63bb6-112">Child elements</span></span>

<span data-ttu-id="63bb6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63bb6-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63bb6-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="63bb6-114">Parent elements</span></span>

|<span data-ttu-id="63bb6-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="63bb6-115">**Element**</span></span>|<span data-ttu-id="63bb6-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63bb6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63bb6-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="63bb6-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="63bb6-118">Contém os argumentos para uma pesquisa de [operação do FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="63bb6-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63bb6-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="63bb6-119">Text value</span></span>

<span data-ttu-id="63bb6-120">O valor de texto **QueryString** representa uma consulta de caixa de correio feita usando um subconjunto de [sintaxe de consulta avançada (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="63bb6-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="63bb6-121">Para obter informações sobre a sintaxe desse elemento, confira [QueryString (querystringtype)](querystring-querystringtype.md).</span><span class="sxs-lookup"><span data-stu-id="63bb6-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63bb6-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="63bb6-122">Remarks</span></span>

<span data-ttu-id="63bb6-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="63bb6-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63bb6-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="63bb6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63bb6-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="63bb6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63bb6-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="63bb6-126">Schema name</span></span>  <br/> |<span data-ttu-id="63bb6-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="63bb6-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63bb6-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="63bb6-128">Validation file</span></span>  <br/> |<span data-ttu-id="63bb6-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="63bb6-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63bb6-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="63bb6-130">Can be empty</span></span>  <br/> |<span data-ttu-id="63bb6-131">False</span><span class="sxs-lookup"><span data-stu-id="63bb6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63bb6-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="63bb6-132">See also</span></span>



[<span data-ttu-id="63bb6-133">Operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="63bb6-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="63bb6-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="63bb6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

