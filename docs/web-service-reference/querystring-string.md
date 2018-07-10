---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: O elemento QueryString Especifica um conjunto de valores a serem retornadas que correspondam a cadeia de caracteres de consulta em uma solicitação de operação FindPeople. Uma pesquisa com nenhum QueryString especificado retorna todos os itens da pasta especificada.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824935"
---
# <a name="querystring-string"></a><span data-ttu-id="c31ac-104">QueryString (String)</span><span class="sxs-lookup"><span data-stu-id="c31ac-104">QueryString (String)</span></span>

<span data-ttu-id="c31ac-105">O elemento **QueryString** Especifica um conjunto de valores a serem retornadas que correspondam a cadeia de caracteres de consulta em uma solicitação de [operação FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c31ac-105">The **QueryString** element specifies a set of values to be returned that match the query string in a [FindPeople operation](findpeople-operation.md) request.</span></span> <span data-ttu-id="c31ac-106">Uma pesquisa com nenhum **QueryString** especificado retorna todos os itens da pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="c31ac-106">A search with no **QueryString** specified returns all items from the specified folder.</span></span> 
  
```XML
<QueryString/> 
```

 <span data-ttu-id="c31ac-107">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c31ac-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c31ac-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c31ac-108">Attributes and elements</span></span>

<span data-ttu-id="c31ac-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c31ac-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c31ac-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c31ac-110">Attributes</span></span>

<span data-ttu-id="c31ac-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c31ac-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c31ac-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c31ac-112">Child elements</span></span>

<span data-ttu-id="c31ac-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c31ac-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c31ac-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c31ac-114">Parent elements</span></span>

|<span data-ttu-id="c31ac-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c31ac-115">**Element**</span></span>|<span data-ttu-id="c31ac-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c31ac-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c31ac-117">FindPeople</span><span class="sxs-lookup"><span data-stu-id="c31ac-117">FindPeople</span></span>](findpeople.md) <br/> |<span data-ttu-id="c31ac-118">Contém os argumentos para uma pesquisa de [operação FindPeople](findpeople-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c31ac-118">Contains the arguments for a [FindPeople operation](findpeople-operation.md) search.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c31ac-119">Text value</span><span class="sxs-lookup"><span data-stu-id="c31ac-119">Text value</span></span>

<span data-ttu-id="c31ac-120">O valor de texto **QueryString** representa uma consulta de caixa de correio que foram feita por meio de um subconjunto da [Sintaxe de consulta avançada (AQS)](http://msdn.microsoft.com/pt-br/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c31ac-120">The **QueryString** text value represents a mailbox query made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/pt-br/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="c31ac-121">Para obter informações sobre a sintaxe para esse elemento, consulte [QueryString (QueryStringType)](querystring-querystringtype.md).</span><span class="sxs-lookup"><span data-stu-id="c31ac-121">For information about the syntax for this element, see [QueryString (QueryStringType)](querystring-querystringtype.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c31ac-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="c31ac-122">Remarks</span></span>

<span data-ttu-id="c31ac-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c31ac-123">This element was introduced in Exchange Server 2013.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c31ac-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c31ac-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c31ac-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c31ac-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c31ac-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c31ac-126">Schema name</span></span>  <br/> |<span data-ttu-id="c31ac-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c31ac-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c31ac-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c31ac-128">Validation file</span></span>  <br/> |<span data-ttu-id="c31ac-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c31ac-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c31ac-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c31ac-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c31ac-131">False</span><span class="sxs-lookup"><span data-stu-id="c31ac-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c31ac-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="c31ac-132">See also</span></span>



[<span data-ttu-id="c31ac-133">Operação FindPeople</span><span class="sxs-lookup"><span data-stu-id="c31ac-133">FindPeople operation</span></span>](findpeople-operation.md)


- [<span data-ttu-id="c31ac-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c31ac-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

