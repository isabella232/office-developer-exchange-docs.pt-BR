---
title: NonIndexableItemDetail
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a26d4c02-f1bd-40c4-9257-5db45e839f17
description: O elemento NonIndexableItemDetail especifica informações detalhadas sobre um item que não pode ser indexado.
ms.openlocfilehash: 4fc4324501570402d22aa303d6af2a60b50b3cc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466735"
---
# <a name="nonindexableitemdetail"></a><span data-ttu-id="8e34b-103">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="8e34b-103">NonIndexableItemDetail</span></span>

<span data-ttu-id="8e34b-104">O elemento **NonIndexableItemDetail** especifica informações detalhadas sobre um item que não pode ser indexado.</span><span class="sxs-lookup"><span data-stu-id="8e34b-104">The **NonIndexableItemDetail** element specifies detail information about an item that cannot be indexed.</span></span> 
  
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

 <span data-ttu-id="8e34b-105">**NonIndexableItemDetailType**</span><span class="sxs-lookup"><span data-stu-id="8e34b-105">**NonIndexableItemDetailType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8e34b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8e34b-106">Attributes and elements</span></span>

<span data-ttu-id="8e34b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8e34b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e34b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8e34b-108">Attributes</span></span>

<span data-ttu-id="8e34b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e34b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e34b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8e34b-110">Child elements</span></span>

<span data-ttu-id="8e34b-111">[ItemId](itemid.md)  |  [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)  |  [ErrorDescription](errordescription.md)  |  [IsPartiallyIndexed](ispartiallyindexed.md)  |  [IsPermanentFailure](ispermanentfailure.md)  |  [Sortvalue](sortvalue.md)  |  [AttemptCount](attemptcount.md)  |  [LastAttemptTime](lastattempttime.md)  |  [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8e34b-111">[ItemId](itemid.md) | [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md) | [ErrorDescription](errordescription.md) | [IsPartiallyIndexed](ispartiallyindexed.md) | [IsPermanentFailure](ispermanentfailure.md) | [SortValue](sortvalue.md) | [AttemptCount](attemptcount.md) | [LastAttemptTime](lastattempttime.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e34b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8e34b-112">Parent elements</span></span>

[<span data-ttu-id="8e34b-113">Itens (ArrayOfNonIndexableItemDetailsType)</span><span class="sxs-lookup"><span data-stu-id="8e34b-113">Items (ArrayOfNonIndexableItemDetailsType)</span></span>](items-arrayofnonindexableitemdetailstype.md)
  
## <a name="remarks"></a><span data-ttu-id="8e34b-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="8e34b-114">Remarks</span></span>

<span data-ttu-id="8e34b-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8e34b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8e34b-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e34b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e34b-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8e34b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e34b-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e34b-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e34b-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8e34b-119">Schema name</span></span>  <br/> |<span data-ttu-id="8e34b-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8e34b-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e34b-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8e34b-121">Validation file</span></span>  <br/> |<span data-ttu-id="8e34b-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8e34b-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e34b-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8e34b-123">Can be empty</span></span>  <br/> ||
   

