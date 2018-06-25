---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: O elemento GetNonIndexableItemDetails Especifica uma solicitação para recuperar os detalhes do item nonindexable.
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752560"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="6e709-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="6e709-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="6e709-104">O elemento **GetNonIndexableItemDetails** Especifica uma solicitação para recuperar os detalhes do item nonindexable.</span><span class="sxs-lookup"><span data-stu-id="6e709-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="6e709-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="6e709-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e709-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6e709-106">Attributes and elements</span></span>

<span data-ttu-id="6e709-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e709-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e709-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e709-108">Attributes</span></span>

<span data-ttu-id="6e709-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e709-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e709-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e709-110">Child elements</span></span>

|<span data-ttu-id="6e709-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e709-111">**Element**</span></span>|<span data-ttu-id="6e709-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e709-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e709-113">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="6e709-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="6e709-114">Especifica uma matriz de elementos de **caixa de correio** .</span><span class="sxs-lookup"><span data-stu-id="6e709-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="6e709-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="6e709-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="6e709-116">Contém o número de itens a serem retornados em uma única página para um resultado de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6e709-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="6e709-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="6e709-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="6e709-118">Especifica a referência para um item de página.</span><span class="sxs-lookup"><span data-stu-id="6e709-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="6e709-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="6e709-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="6e709-120">Contém a direção da paginação no resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6e709-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e709-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e709-121">Parent elements</span></span>

<span data-ttu-id="6e709-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e709-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e709-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e709-123">Remarks</span></span>

<span data-ttu-id="6e709-124">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6e709-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6e709-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e709-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e709-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6e709-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e709-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e709-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e709-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e709-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6e709-129">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="6e709-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="6e709-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e709-130">Validation File</span></span>  <br/> |<span data-ttu-id="6e709-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e709-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e709-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6e709-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6e709-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="6e709-133">See also</span></span>



- [<span data-ttu-id="6e709-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6e709-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

