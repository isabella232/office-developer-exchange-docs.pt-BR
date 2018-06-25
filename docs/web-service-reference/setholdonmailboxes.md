---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: O elemento SetHoldOnMailboxes contém uma solicitação de SetHoldOnMailboxes.
ms.openlocfilehash: 7d226de908c4d5a474129e3e1f2344ec1318f538
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825413"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="390d5-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="390d5-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="390d5-104">O elemento **SetHoldOnMailboxes** contém uma solicitação de **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="390d5-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 <span data-ttu-id="390d5-105">**SetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="390d5-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="390d5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="390d5-106">Attributes and elements</span></span>

<span data-ttu-id="390d5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="390d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="390d5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="390d5-108">Attributes</span></span>

<span data-ttu-id="390d5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="390d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="390d5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="390d5-110">Child elements</span></span>

<span data-ttu-id="390d5-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [consulta](query.md) | [caixas de correio (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [idioma](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [a eliminação da duplicação ](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)</span><span class="sxs-lookup"><span data-stu-id="390d5-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="390d5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="390d5-112">Parent elements</span></span>

<span data-ttu-id="390d5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="390d5-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="390d5-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="390d5-114">Remarks</span></span>

<span data-ttu-id="390d5-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="390d5-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="390d5-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="390d5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="390d5-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="390d5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="390d5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="390d5-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="390d5-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="390d5-119">Schema name</span></span>  <br/> |<span data-ttu-id="390d5-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="390d5-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="390d5-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="390d5-121">Validation file</span></span>  <br/> |<span data-ttu-id="390d5-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="390d5-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="390d5-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="390d5-123">Can be empty</span></span>  <br/> ||
   

