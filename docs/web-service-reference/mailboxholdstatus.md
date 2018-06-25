---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: O elemento MailboxHoldStatus Especifica o status de retenção da caixa de correio.
ms.openlocfilehash: 6703c909d0a7b4e83e190807fc3202ecd4699e7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824288"
---
# <a name="mailboxholdstatus"></a><span data-ttu-id="5892c-103">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="5892c-103">MailboxHoldStatus</span></span>

<span data-ttu-id="5892c-104">O elemento **MailboxHoldStatus** Especifica o status de retenção da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5892c-104">The **MailboxHoldStatus** element specifies the hold status of the mailbox.</span></span> 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

<span data-ttu-id="5892c-105">**MailboxHoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="5892c-105">**MailboxHoldStatusType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5892c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5892c-106">Attributes and elements</span></span>

<span data-ttu-id="5892c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5892c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5892c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5892c-108">Attributes</span></span>

<span data-ttu-id="5892c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5892c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5892c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5892c-110">Child elements</span></span>

<span data-ttu-id="5892c-111">[Caixa de correio (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span><span class="sxs-lookup"><span data-stu-id="5892c-111">[Mailbox (string)](mailbox-string.md) | [Status (HoldStatusType)](status-holdstatustype.md) | [AdditionalInfo](additionalinfo.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5892c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5892c-112">Parent elements</span></span>

[<span data-ttu-id="5892c-113">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="5892c-113">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
  
## <a name="remarks"></a><span data-ttu-id="5892c-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="5892c-114">Remarks</span></span>

<span data-ttu-id="5892c-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5892c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5892c-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5892c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5892c-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5892c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5892c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="5892c-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5892c-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5892c-119">Schema name</span></span>  <br/> |<span data-ttu-id="5892c-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5892c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="5892c-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5892c-121">Validation file</span></span>  <br/> |<span data-ttu-id="5892c-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5892c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5892c-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5892c-123">Can be empty</span></span>  <br/> ||
   

