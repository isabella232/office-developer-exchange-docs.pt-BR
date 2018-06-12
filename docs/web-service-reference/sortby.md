---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: O elemento de SortBy contém uma propriedade de item usada para classificar os resultados de pesquisa.
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825518"
---
# <a name="sortby"></a><span data-ttu-id="41a55-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="41a55-103">SortBy</span></span>

<span data-ttu-id="41a55-104">O elemento de **SortBy** contém uma propriedade de item usada para classificar os resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="41a55-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="41a55-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="41a55-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41a55-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="41a55-106">Attributes and elements</span></span>

<span data-ttu-id="41a55-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41a55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41a55-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41a55-108">Attributes</span></span>

|<span data-ttu-id="41a55-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="41a55-109">**Attribute**</span></span>|<span data-ttu-id="41a55-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41a55-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41a55-111">Ordem</span><span class="sxs-lookup"><span data-stu-id="41a55-111">Order</span></span>  <br/> |<span data-ttu-id="41a55-112">O valor de texto do atributo **ordem** é a ordem de classificação.</span><span class="sxs-lookup"><span data-stu-id="41a55-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="41a55-113">Um valor de texto de **crescente** indica que os resultados são em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="41a55-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="41a55-114">Um valor de texto de **Decrescente** indica que os resultados em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="41a55-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="41a55-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41a55-115">Child elements</span></span>

<span data-ttu-id="41a55-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="41a55-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41a55-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41a55-117">Parent elements</span></span>

[<span data-ttu-id="41a55-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="41a55-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="41a55-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="41a55-119">Remarks</span></span>

<span data-ttu-id="41a55-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="41a55-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="41a55-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="41a55-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41a55-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="41a55-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41a55-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="41a55-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="41a55-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41a55-124">Schema name</span></span>  <br/> |<span data-ttu-id="41a55-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="41a55-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="41a55-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41a55-126">Validation file</span></span>  <br/> |<span data-ttu-id="41a55-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="41a55-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41a55-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="41a55-128">Can be empty</span></span>  <br/> ||
   

