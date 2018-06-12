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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752560"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="9169c-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9169c-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="9169c-104">O elemento **GetNonIndexableItemDetails** Especifica uma solicitação para recuperar os detalhes do item nonindexable.</span><span class="sxs-lookup"><span data-stu-id="9169c-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="9169c-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="9169c-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9169c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9169c-106">Attributes and elements</span></span>

<span data-ttu-id="9169c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9169c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9169c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9169c-108">Attributes</span></span>

<span data-ttu-id="9169c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9169c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9169c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9169c-110">Child elements</span></span>

|<span data-ttu-id="9169c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9169c-111">**Element**</span></span>|<span data-ttu-id="9169c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9169c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9169c-113">Caixas de correio (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="9169c-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="9169c-114">Especifica uma matriz de elementos de **caixa de correio** .</span><span class="sxs-lookup"><span data-stu-id="9169c-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="9169c-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="9169c-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="9169c-116">Contém o número de itens a serem retornados em uma única página para um resultado de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9169c-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="9169c-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="9169c-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="9169c-118">Especifica a referência para um item de página.</span><span class="sxs-lookup"><span data-stu-id="9169c-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="9169c-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="9169c-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="9169c-120">Contém a direção da paginação no resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9169c-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9169c-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9169c-121">Parent elements</span></span>

<span data-ttu-id="9169c-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9169c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9169c-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="9169c-123">Remarks</span></span>

<span data-ttu-id="9169c-124">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9169c-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9169c-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9169c-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9169c-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9169c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9169c-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9169c-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9169c-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9169c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9169c-129">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="9169c-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="9169c-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9169c-130">Validation File</span></span>  <br/> |<span data-ttu-id="9169c-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9169c-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9169c-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9169c-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9169c-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="9169c-133">See also</span></span>



- [<span data-ttu-id="9169c-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9169c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

