---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: O elemento de Status Especifica o status de retenção para uma caixa de correio.
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825579"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="b86f1-103">Status (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="b86f1-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="b86f1-104">O elemento de **Status** Especifica o status de retenção para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86f1-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="b86f1-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="b86f1-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b86f1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b86f1-106">Attributes and elements</span></span>

<span data-ttu-id="b86f1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b86f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b86f1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b86f1-108">Attributes</span></span>

<span data-ttu-id="b86f1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b86f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b86f1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b86f1-110">Child elements</span></span>

<span data-ttu-id="b86f1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b86f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b86f1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b86f1-112">Parent elements</span></span>

[<span data-ttu-id="b86f1-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="b86f1-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="b86f1-114">Text value</span><span class="sxs-lookup"><span data-stu-id="b86f1-114">Text value</span></span>

<span data-ttu-id="b86f1-115">O valor de texto do elemento de **Status** é o status de retenção de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86f1-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="b86f1-116">O elemento de **Status** pode ter os valores na lista a seguir.</span><span class="sxs-lookup"><span data-stu-id="b86f1-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="b86f1-117">NotOnHold - a caixa de correio não está em espera.</span><span class="sxs-lookup"><span data-stu-id="b86f1-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="b86f1-118">Pendente - a caixa de correio é pendentes que estão sendo colocados ou lançados em espera.</span><span class="sxs-lookup"><span data-stu-id="b86f1-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="b86f1-119">OnHold - isenção foi aplicada com êxito à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86f1-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="b86f1-120">PartialHold - isenção foi aplicada com êxito a algumas caixas de correio, mas não para todas as caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="b86f1-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="b86f1-121">Isenção falha - falha aplicar à caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b86f1-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b86f1-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="b86f1-122">Remarks</span></span>

<span data-ttu-id="b86f1-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b86f1-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b86f1-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b86f1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b86f1-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b86f1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b86f1-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b86f1-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b86f1-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b86f1-127">Schema name</span></span>  <br/> |<span data-ttu-id="b86f1-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b86f1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="b86f1-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b86f1-129">Validation file</span></span>  <br/> |<span data-ttu-id="b86f1-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b86f1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b86f1-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b86f1-131">Can be empty</span></span>  <br/> ||
   

