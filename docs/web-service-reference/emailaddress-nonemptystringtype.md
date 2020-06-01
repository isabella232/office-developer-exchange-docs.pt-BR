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
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463129"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="d9e13-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d9e13-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="d9e13-104">O elemento **EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d9e13-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="d9e13-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="d9e13-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9e13-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d9e13-106">Attributes and elements</span></span>

<span data-ttu-id="d9e13-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9e13-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9e13-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9e13-108">Attributes</span></span>

<span data-ttu-id="d9e13-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9e13-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9e13-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9e13-110">Child elements</span></span>

<span data-ttu-id="d9e13-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9e13-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9e13-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9e13-112">Parent elements</span></span>

|<span data-ttu-id="d9e13-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9e13-113">**Element**</span></span>|<span data-ttu-id="d9e13-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9e13-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9e13-115">Agindo</span><span class="sxs-lookup"><span data-stu-id="d9e13-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="d9e13-116">Identifica quem o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="d9e13-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="d9e13-117">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="d9e13-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="d9e13-118">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="d9e13-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="d9e13-119">A seguir estão algumas expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d9e13-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="d9e13-120">Estes são os elementos pai adicionais do elemento de caixa de correio:</span><span class="sxs-lookup"><span data-stu-id="d9e13-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="d9e13-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="d9e13-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="d9e13-123">- [Enviou](sender.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="d9e13-124">- [De](from.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-124">- [From](from.md)</span></span> <br/><span data-ttu-id="d9e13-125">- [Organizador](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="d9e13-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="d9e13-127">- [Solução](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="d9e13-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="d9e13-129">- [Tende](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="d9e13-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="d9e13-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="d9e13-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="d9e13-131">Identifica uma lista de salas de reunião por endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d9e13-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9e13-132">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d9e13-132">Text value</span></span>

<span data-ttu-id="d9e13-133">Um valor de texto que representa um endereço SMTP é necessário.</span><span class="sxs-lookup"><span data-stu-id="d9e13-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d9e13-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9e13-134">Remarks</span></span>

<span data-ttu-id="d9e13-135">O elemento **EmailAddress** pode representar endereços distintos SMTP ou herdados do Exchange (também conhecidos como DN).</span><span class="sxs-lookup"><span data-stu-id="d9e13-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="d9e13-136">O elemento **EmailAddress** é o único elemento de [caixa de correio](mailbox.md) necessário.</span><span class="sxs-lookup"><span data-stu-id="d9e13-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="d9e13-137">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9e13-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9e13-138">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d9e13-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9e13-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9e13-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9e13-140">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9e13-140">Schema Name</span></span>  <br/> |<span data-ttu-id="d9e13-141">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d9e13-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9e13-142">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9e13-142">Validation File</span></span>  <br/> |<span data-ttu-id="d9e13-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d9e13-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9e13-144">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9e13-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9e13-145">Falso</span><span class="sxs-lookup"><span data-stu-id="d9e13-145">False</span></span>  <br/> |
   

