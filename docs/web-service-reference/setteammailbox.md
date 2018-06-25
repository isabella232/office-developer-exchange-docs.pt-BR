---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: O elemento SetTeamMailbox contém uma solicitação para definir uma caixa de correio do site.
ms.openlocfilehash: 708863168f4e89775deee8c5d66427df41515089
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825455"
---
# <a name="setteammailbox"></a><span data-ttu-id="30258-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="30258-103">SetTeamMailbox</span></span>

<span data-ttu-id="30258-104">O elemento **SetTeamMailbox** contém uma solicitação para definir uma caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="30258-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="30258-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="30258-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30258-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30258-106">Attributes and elements</span></span>

<span data-ttu-id="30258-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30258-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30258-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30258-108">Attributes</span></span>

<span data-ttu-id="30258-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30258-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30258-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30258-110">Child elements</span></span>

<span data-ttu-id="30258-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [estado (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="30258-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30258-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30258-112">Parent elements</span></span>

<span data-ttu-id="30258-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30258-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30258-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="30258-114">Remarks</span></span>

<span data-ttu-id="30258-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="30258-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30258-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30258-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30258-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30258-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30258-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="30258-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30258-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30258-119">Schema name</span></span>  <br/> |<span data-ttu-id="30258-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="30258-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30258-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30258-121">Validation file</span></span>  <br/> |<span data-ttu-id="30258-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30258-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30258-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="30258-123">Can be empty</span></span>  <br/> ||
   

