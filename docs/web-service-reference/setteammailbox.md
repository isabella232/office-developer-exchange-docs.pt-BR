---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: O elemento SetTeamMailbox contém uma solicitação para definir uma caixa de correio de site.
ms.openlocfilehash: e4b7ebd308f4b58b6b6491289f24b9176c5dcf15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465258"
---
# <a name="setteammailbox"></a><span data-ttu-id="99274-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="99274-103">SetTeamMailbox</span></span>

<span data-ttu-id="99274-104">O elemento **SetTeamMailbox** contém uma solicitação para definir uma caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="99274-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="99274-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="99274-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99274-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="99274-106">Attributes and elements</span></span>

<span data-ttu-id="99274-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99274-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99274-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99274-108">Attributes</span></span>

<span data-ttu-id="99274-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99274-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99274-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99274-110">Child elements</span></span>

<span data-ttu-id="99274-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  |  [SharePointSiteUrl](sharepointsiteurl.md)  |  [Estado (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="99274-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99274-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99274-112">Parent elements</span></span>

<span data-ttu-id="99274-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99274-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99274-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="99274-114">Remarks</span></span>

<span data-ttu-id="99274-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="99274-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="99274-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="99274-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99274-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="99274-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99274-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="99274-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99274-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99274-119">Schema name</span></span>  <br/> |<span data-ttu-id="99274-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="99274-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99274-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99274-121">Validation file</span></span>  <br/> |<span data-ttu-id="99274-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="99274-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99274-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="99274-123">Can be empty</span></span>  <br/> ||
   

