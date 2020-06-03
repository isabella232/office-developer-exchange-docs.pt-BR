---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: O elemento status especifica o status de espera para uma caixa de correio.
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459984"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="95050-103">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="95050-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="95050-104">O elemento **status** especifica o status de espera para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95050-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="95050-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="95050-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95050-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="95050-106">Attributes and elements</span></span>

<span data-ttu-id="95050-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95050-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95050-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="95050-108">Attributes</span></span>

<span data-ttu-id="95050-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95050-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95050-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95050-110">Child elements</span></span>

<span data-ttu-id="95050-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95050-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95050-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95050-112">Parent elements</span></span>

[<span data-ttu-id="95050-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="95050-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="95050-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="95050-114">Text value</span></span>

<span data-ttu-id="95050-115">O valor de texto do elemento **status** é o status de espera de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95050-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="95050-116">O elemento **status** pode ter os valores na lista a seguir.</span><span class="sxs-lookup"><span data-stu-id="95050-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="95050-117">NotOnHold-a caixa de correio não está em espera.</span><span class="sxs-lookup"><span data-stu-id="95050-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="95050-118">Pendente-a caixa de correio está pendente que está sendo colocada ou liberada em espera.</span><span class="sxs-lookup"><span data-stu-id="95050-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="95050-119">OnHold-a retenção foi aplicada com êxito à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95050-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="95050-120">PartialHold-a retenção foi aplicada com êxito a algumas caixas de correio, mas não a todas as caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="95050-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="95050-121">Failed-Falha ao aplicar à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95050-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="95050-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="95050-122">Remarks</span></span>

<span data-ttu-id="95050-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="95050-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="95050-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95050-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95050-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="95050-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95050-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="95050-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95050-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95050-127">Schema name</span></span>  <br/> |<span data-ttu-id="95050-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="95050-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="95050-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95050-129">Validation file</span></span>  <br/> |<span data-ttu-id="95050-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95050-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95050-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="95050-131">Can be empty</span></span>  <br/> ||
   

