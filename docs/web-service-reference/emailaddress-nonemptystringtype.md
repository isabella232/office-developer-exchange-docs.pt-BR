---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: O elemento EmailAddress define o endereço SMTP principal de um usuário de caixa de correio.
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751991"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="9aa2e-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="9aa2e-104">O elemento **EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="9aa2e-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="9aa2e-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9aa2e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9aa2e-106">Attributes and elements</span></span>

<span data-ttu-id="9aa2e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9aa2e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9aa2e-108">Attributes</span></span>

<span data-ttu-id="9aa2e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9aa2e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9aa2e-110">Child elements</span></span>

<span data-ttu-id="9aa2e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9aa2e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9aa2e-112">Parent elements</span></span>

|<span data-ttu-id="9aa2e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9aa2e-113">**Element**</span></span>|<span data-ttu-id="9aa2e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9aa2e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9aa2e-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="9aa2e-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="9aa2e-116">Identifica que o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="9aa2e-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="9aa2e-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="9aa2e-118">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="9aa2e-119">A seguir estão algumas expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="9aa2e-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="9aa2e-120">Estes são os elementos adicionais pai do elemento de caixa de correio:</span><span class="sxs-lookup"><span data-stu-id="9aa2e-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="9aa2e-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="9aa2e-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="9aa2e-123">- [Remetente](sender.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="9aa2e-124">- [De](from.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-124">- [From](from.md)</span></span> <br/><span data-ttu-id="9aa2e-125">- [Organizador](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="9aa2e-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="9aa2e-127">- [Resolução](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="9aa2e-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="9aa2e-129">- [Participante](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="9aa2e-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="9aa2e-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="9aa2e-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="9aa2e-131">Identifica uma lista de salas de reunião pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9aa2e-132">Text value</span><span class="sxs-lookup"><span data-stu-id="9aa2e-132">Text value</span></span>

<span data-ttu-id="9aa2e-133">É necessário um valor de texto que representa um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9aa2e-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="9aa2e-134">Remarks</span></span>

<span data-ttu-id="9aa2e-135">O elemento **EmailAddress** pode representar SMTP ou herdado do Exchange diferenciados endereços nome (também conhecido como DN).</span><span class="sxs-lookup"><span data-stu-id="9aa2e-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="9aa2e-136">O elemento **EmailAddress** é o único elemento de [caixa de correio](mailbox.md) necessário.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="9aa2e-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9aa2e-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9aa2e-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9aa2e-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9aa2e-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="9aa2e-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9aa2e-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9aa2e-140">Schema Name</span></span>  <br/> |<span data-ttu-id="9aa2e-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9aa2e-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="9aa2e-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9aa2e-142">Validation File</span></span>  <br/> |<span data-ttu-id="9aa2e-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9aa2e-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9aa2e-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9aa2e-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="9aa2e-145">False</span><span class="sxs-lookup"><span data-stu-id="9aa2e-145">False</span></span>  <br/> |
   

