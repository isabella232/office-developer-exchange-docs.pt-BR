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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751991"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="a9437-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a9437-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="a9437-104">O elemento **EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a9437-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="a9437-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="a9437-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9437-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a9437-106">Attributes and elements</span></span>

<span data-ttu-id="a9437-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a9437-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9437-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a9437-108">Attributes</span></span>

<span data-ttu-id="a9437-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9437-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9437-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a9437-110">Child elements</span></span>

<span data-ttu-id="a9437-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9437-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9437-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a9437-112">Parent elements</span></span>

|<span data-ttu-id="a9437-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9437-113">**Element**</span></span>|<span data-ttu-id="a9437-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9437-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9437-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="a9437-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="a9437-116">Identifica que o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="a9437-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="a9437-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="a9437-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="a9437-118">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="a9437-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="a9437-119">A seguir estão algumas expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a9437-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="a9437-120">Estes são os elementos adicionais pai do elemento de caixa de correio:</span><span class="sxs-lookup"><span data-stu-id="a9437-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="a9437-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="a9437-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="a9437-123">- [Remetente](sender.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="a9437-124">- [De](from.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-124">- [From](from.md)</span></span> <br/><span data-ttu-id="a9437-125">- [Organizador](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="a9437-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="a9437-127">- [Resolução](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="a9437-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="a9437-129">- [Participante](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="a9437-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="a9437-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="a9437-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="a9437-131">Identifica uma lista de salas de reunião pelo endereço de email.</span><span class="sxs-lookup"><span data-stu-id="a9437-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9437-132">Text value</span><span class="sxs-lookup"><span data-stu-id="a9437-132">Text value</span></span>

<span data-ttu-id="a9437-133">É necessário um valor de texto que representa um endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="a9437-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a9437-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="a9437-134">Remarks</span></span>

<span data-ttu-id="a9437-135">O elemento **EmailAddress** pode representar SMTP ou herdado do Exchange diferenciados endereços nome (também conhecido como DN).</span><span class="sxs-lookup"><span data-stu-id="a9437-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="a9437-136">O elemento **EmailAddress** é o único elemento de [caixa de correio](mailbox.md) necessário.</span><span class="sxs-lookup"><span data-stu-id="a9437-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="a9437-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9437-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9437-138">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a9437-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9437-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9437-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9437-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a9437-140">Schema Name</span></span>  <br/> |<span data-ttu-id="a9437-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a9437-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9437-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a9437-142">Validation File</span></span>  <br/> |<span data-ttu-id="a9437-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a9437-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9437-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a9437-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9437-145">False</span><span class="sxs-lookup"><span data-stu-id="a9437-145">False</span></span>  <br/> |
   

