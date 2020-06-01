---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: O elemento SetHoldOnMailboxes contém uma solicitação SetHoldOnMailboxes.
ms.openlocfilehash: c96ff50cb1204d86abc66829e1c5da7124f407f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448349"
---
# <a name="setholdonmailboxes"></a><span data-ttu-id="ec2e3-103">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ec2e3-103">SetHoldOnMailboxes</span></span>

<span data-ttu-id="ec2e3-104">O elemento **SetHoldOnMailboxes** contém uma solicitação **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="ec2e3-104">The **SetHoldOnMailboxes** element contains a **SetHoldOnMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="ec2e3-105">**SetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="ec2e3-105">**SetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec2e3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ec2e3-106">Attributes and elements</span></span>

<span data-ttu-id="ec2e3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec2e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec2e3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec2e3-108">Attributes</span></span>

<span data-ttu-id="ec2e3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec2e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec2e3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec2e3-110">Child elements</span></span>

<span data-ttu-id="ec2e3-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md)  |  [Isenção](holdid.md)  |  [Consulta](query.md)  |  [Caixas de correio (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  |  [Idioma](language.md)  |  [IncludeNonIndexableItems](includenonindexableitems.md)  |  [Eliminação de duplicação](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)</span><span class="sxs-lookup"><span data-stu-id="ec2e3-111">[ActionType (HoldActionType)](actiontype-holdactiontype.md) | [HoldId](holdid.md) | [Query](query.md) | [Mailboxes (ArrayOfStringsType)](mailboxes-arrayofstringstype.md) | [Language](language.md) | [IncludeNonIndexableItems](includenonindexableitems.md) | [Deduplication](deduplication.md) | [InPlaceHoldIdentity](inplaceholdidentity.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec2e3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec2e3-112">Parent elements</span></span>

<span data-ttu-id="ec2e3-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec2e3-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec2e3-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec2e3-114">Remarks</span></span>

<span data-ttu-id="ec2e3-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ec2e3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ec2e3-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec2e3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec2e3-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ec2e3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec2e3-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec2e3-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec2e3-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec2e3-119">Schema name</span></span>  <br/> |<span data-ttu-id="ec2e3-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ec2e3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec2e3-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec2e3-121">Validation file</span></span>  <br/> |<span data-ttu-id="ec2e3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec2e3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec2e3-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ec2e3-123">Can be empty</span></span>  <br/> ||
   

