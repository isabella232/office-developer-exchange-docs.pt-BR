---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: O elemento SortBy contém uma propriedade de item usada para classificar o resultado da pesquisa.
ms.openlocfilehash: cf2b1e633bc66e526028078833afade363e4c5e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468394"
---
# <a name="sortby"></a><span data-ttu-id="94627-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="94627-103">SortBy</span></span>

<span data-ttu-id="94627-104">O elemento **sortBy** contém uma propriedade de item usada para classificar o resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="94627-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="94627-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="94627-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94627-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="94627-106">Attributes and elements</span></span>

<span data-ttu-id="94627-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94627-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94627-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="94627-108">Attributes</span></span>

|<span data-ttu-id="94627-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="94627-109">**Attribute**</span></span>|<span data-ttu-id="94627-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94627-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94627-111">Ordem</span><span class="sxs-lookup"><span data-stu-id="94627-111">Order</span></span>  <br/> |<span data-ttu-id="94627-112">O valor de texto do atributo **Order** é a ordem de classificação.</span><span class="sxs-lookup"><span data-stu-id="94627-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="94627-113">Um valor de texto **crescente** indica que os resultados estão em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="94627-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="94627-114">Um valor de texto **decrescente** indica que os resultados estão em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="94627-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="94627-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94627-115">Child elements</span></span>

<span data-ttu-id="94627-116">[FieldURI](fielduri.md)  |  [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="94627-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94627-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94627-117">Parent elements</span></span>

[<span data-ttu-id="94627-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="94627-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="94627-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="94627-119">Remarks</span></span>

<span data-ttu-id="94627-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="94627-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="94627-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="94627-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94627-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="94627-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94627-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="94627-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94627-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94627-124">Schema name</span></span>  <br/> |<span data-ttu-id="94627-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="94627-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94627-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94627-126">Validation file</span></span>  <br/> |<span data-ttu-id="94627-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="94627-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94627-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="94627-128">Can be empty</span></span>  <br/> ||
   

