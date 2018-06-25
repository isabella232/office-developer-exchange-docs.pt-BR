---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: O elemento NonIndexableItemDetail Especifica informações detalhadas sobre um item que não pode ser indexado.
ms.openlocfilehash: ef1bd072a44b42b501a3016c394b89fe6ab25bf0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824543"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="d1229-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="d1229-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="d1229-104">O elemento **NonIndexableItemDetail** Especifica informações detalhadas sobre um item que não pode ser indexado.</span><span class="sxs-lookup"><span data-stu-id="d1229-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
```XML
<NonIndexableItemDetail>
   <ItemId/>
   <ErrorCode/>
   <ErrorDescription/>
   <IsPartiallyIndexed/>
   <IsPermanentFailure/>
   <SortValue/>
   <AttemptCount/>
   <LastAttemptTime/>
   <AdditionalInfo/>
</NonIndexableItemDetail>
```

 <span data-ttu-id="d1229-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="d1229-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1229-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d1229-106">Attributes and elements</span></span>

<span data-ttu-id="d1229-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1229-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1229-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1229-108">Attributes</span></span>

<span data-ttu-id="d1229-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d1229-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1229-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1229-110">Child elements</span></span>

<span data-ttu-id="d1229-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount ](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="d1229-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1229-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1229-112">Parent elements</span></span>

[<span data-ttu-id="d1229-113">Itens (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="d1229-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="d1229-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1229-114">Remarks</span></span>

<span data-ttu-id="d1229-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1229-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1229-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1229-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1229-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d1229-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1229-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1229-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1229-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1229-119">Schema name</span></span>  <br/> |<span data-ttu-id="d1229-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d1229-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1229-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1229-121">Validation file</span></span>  <br/> |<span data-ttu-id="d1229-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1229-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1229-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d1229-123">Can be empty</span></span>  <br/> ||
   

