---
title: MailboxHoldResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: da03b877-37c6-4ecb-8549-c639f140302e
description: O elemento MailboxHoldResult contém o resultado da solicitação GetHoldOnMailboxes.
ms.openlocfilehash: 3895c1351587db45881c661809a19dad1929b4a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466392"
---
# <a name="mailboxholdresult"></a><span data-ttu-id="9e3a0-103">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="9e3a0-103">MailboxHoldResult</span></span>

<span data-ttu-id="9e3a0-104">O elemento **MailboxHoldResult** contém o resultado da solicitação **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="9e3a0-104">The **MailboxHoldResult** element contains the result of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<MailboxHoldResult>
   <HoldId/>
   <Query/>
   <MailboxHoldStatuses/>
</MailboxHoldResult>
```

<span data-ttu-id="9e3a0-105">**MailboxHoldResultType**</span><span class="sxs-lookup"><span data-stu-id="9e3a0-105">**MailboxHoldResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9e3a0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9e3a0-106">Attributes and elements</span></span>

<span data-ttu-id="9e3a0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e3a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e3a0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e3a0-108">Attributes</span></span>

<span data-ttu-id="9e3a0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e3a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e3a0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e3a0-110">Child elements</span></span>

<span data-ttu-id="9e3a0-111">[Isenção](holdid.md)  |  [Consulta](query.md)  |  [MailboxHoldStatuses](mailboxholdstatuses.md)</span><span class="sxs-lookup"><span data-stu-id="9e3a0-111">[HoldId](holdid.md) | [Query](query.md) | [MailboxHoldStatuses](mailboxholdstatuses.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e3a0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e3a0-112">Parent elements</span></span>

<span data-ttu-id="9e3a0-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e3a0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e3a0-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e3a0-114">Remarks</span></span>

<span data-ttu-id="9e3a0-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9e3a0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e3a0-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e3a0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e3a0-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9e3a0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e3a0-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e3a0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e3a0-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e3a0-119">Schema name</span></span>  <br/> |<span data-ttu-id="9e3a0-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9e3a0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e3a0-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e3a0-121">Validation file</span></span>  <br/> |<span data-ttu-id="9e3a0-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e3a0-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e3a0-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9e3a0-123">Can be empty</span></span>  <br/> ||
   

