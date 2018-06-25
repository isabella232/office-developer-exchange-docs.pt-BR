---
title: Estado (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: O elemento de estado contém o estado de ciclo de vida for definido em uma caixa de correio do site.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825571"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="89b65-103">Estado (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="89b65-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="89b65-104">O elemento de **estado** contém o estado de ciclo de vida for definido em uma caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="89b65-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="89b65-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="89b65-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="89b65-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="89b65-106">Attributes and elements</span></span>

<span data-ttu-id="89b65-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89b65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89b65-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="89b65-108">Attributes</span></span>

<span data-ttu-id="89b65-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89b65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89b65-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89b65-110">Child elements</span></span>

<span data-ttu-id="89b65-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89b65-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89b65-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89b65-112">Parent elements</span></span>

[<span data-ttu-id="89b65-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="89b65-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="89b65-114">Text value</span><span class="sxs-lookup"><span data-stu-id="89b65-114">Text value</span></span>

<span data-ttu-id="89b65-115">O valor de texto do elemento de **estado** é o estado de ciclo de vida que é definido em uma caixa de correio do site.</span><span class="sxs-lookup"><span data-stu-id="89b65-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="89b65-116">Um valor de texto de **ativo** indica que uma caixa de correio de site está em uso ativo.</span><span class="sxs-lookup"><span data-stu-id="89b65-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="89b65-117">Um valor de texto **fechado** indica que uma caixa de correio de site foi fechada e não está em uso ativo.</span><span class="sxs-lookup"><span data-stu-id="89b65-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="89b65-118">Um valor de texto de **desvinculados** indica que uma caixa de correio de site não estiver vinculada a um ambiente de colaboração baseado na web.</span><span class="sxs-lookup"><span data-stu-id="89b65-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="89b65-119">Os valores de **ativo**, **fechado**e **PendingDelete** são mutuamente exclusivos, mas o valor **desvinculados** não é mutuamente exclusivos os outros valores.</span><span class="sxs-lookup"><span data-stu-id="89b65-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="89b65-120">Um valor de texto de **PendingDelete** indica que uma caixa de correio de site é exclusão pendente.</span><span class="sxs-lookup"><span data-stu-id="89b65-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="89b65-121">Uma caixa de correio de site deve ser fechado antes que ela pode ser definida como **PendingDelete**.</span><span class="sxs-lookup"><span data-stu-id="89b65-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89b65-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="89b65-122">Remarks</span></span>

<span data-ttu-id="89b65-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="89b65-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="89b65-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89b65-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89b65-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="89b65-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89b65-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="89b65-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89b65-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="89b65-127">Schema name</span></span>  <br/> |<span data-ttu-id="89b65-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="89b65-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89b65-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="89b65-129">Validation file</span></span>  <br/> |<span data-ttu-id="89b65-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89b65-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89b65-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="89b65-131">Can be empty</span></span>  <br/> ||
   

