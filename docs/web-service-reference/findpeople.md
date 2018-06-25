---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'O elemento FindPeople Especifica um conjunto de dados usados em uma solicitação de FindPeople. Os dados incluem zero ou mais dos seguintes elementos: uma forma de pessoa (opcional), um modo de exibição de item de página indexado, uma restrição (opcional), uma restrição de agregação de lista segura (opcional), uma ordem de classificação (opcional), uma Id da pasta pai e uma cadeia de caracteres de consulta (opcional).'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752299"
---
# <a name="findpeople"></a><span data-ttu-id="3a428-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="3a428-104">FindPeople</span></span>

<span data-ttu-id="3a428-105">O elemento **FindPeople** Especifica um conjunto de dados usados em uma solicitação de FindPeople.</span><span class="sxs-lookup"><span data-stu-id="3a428-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="3a428-106">Os dados incluem zero ou mais dos seguintes elementos: uma forma de pessoa (opcional), um modo de exibição de item de página indexado, uma restrição (opcional), uma restrição de agregação de lista segura (opcional), uma ordem de classificação (opcional), uma Id da pasta pai e uma cadeia de caracteres de consulta (opcional).</span><span class="sxs-lookup"><span data-stu-id="3a428-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 <span data-ttu-id="3a428-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="3a428-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a428-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3a428-108">Attributes and elements</span></span>

<span data-ttu-id="3a428-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3a428-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a428-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3a428-110">Attributes</span></span>

<span data-ttu-id="3a428-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a428-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a428-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3a428-112">Child elements</span></span>

<span data-ttu-id="3a428-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [restrição](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [ QueryString (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="3a428-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a428-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3a428-114">Parent elements</span></span>

<span data-ttu-id="3a428-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3a428-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a428-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="3a428-116">Remarks</span></span>

<span data-ttu-id="3a428-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3a428-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a428-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a428-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a428-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3a428-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a428-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="3a428-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a428-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3a428-121">Schema name</span></span>  <br/> |<span data-ttu-id="3a428-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3a428-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a428-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3a428-123">Validation file</span></span>  <br/> |<span data-ttu-id="3a428-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3a428-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a428-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3a428-125">Can be empty</span></span>  <br/> |<span data-ttu-id="3a428-126">false</span><span class="sxs-lookup"><span data-stu-id="3a428-126">false</span></span>  <br/> |
   

