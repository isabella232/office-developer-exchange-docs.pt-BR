---
title: Estado (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: O elemento State contém o estado do ciclo de vida definido em uma caixa de correio de site.
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465160"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="19832-103">Estado (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="19832-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="19832-104">O elemento **State** contém o estado do ciclo de vida definido em uma caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="19832-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="19832-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="19832-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="19832-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="19832-106">Attributes and elements</span></span>

<span data-ttu-id="19832-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19832-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19832-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="19832-108">Attributes</span></span>

<span data-ttu-id="19832-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19832-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19832-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19832-110">Child elements</span></span>

<span data-ttu-id="19832-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="19832-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19832-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19832-112">Parent elements</span></span>

[<span data-ttu-id="19832-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="19832-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="19832-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="19832-114">Text value</span></span>

<span data-ttu-id="19832-115">O valor de texto do elemento **State** é o estado do ciclo de vida definido em uma caixa de correio de site.</span><span class="sxs-lookup"><span data-stu-id="19832-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="19832-116">Um valor de texto **ativo** indica que uma caixa de correio de site está em uso ativo.</span><span class="sxs-lookup"><span data-stu-id="19832-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="19832-117">Um valor de texto **fechado** indica que uma caixa de correio de site foi fechada e não está em uso ativo.</span><span class="sxs-lookup"><span data-stu-id="19832-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="19832-118">Um valor de texto **desvinculado** indica que uma caixa de correio de site não está vinculada a um ambiente de colaboração baseado na Web.</span><span class="sxs-lookup"><span data-stu-id="19832-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="19832-119">Os valores **Active**, **Closed**e **PendingDelete** são mutuamente exclusivos, mas o valor **desvinculado** não é mutuamente exclusivo dos outros valores.</span><span class="sxs-lookup"><span data-stu-id="19832-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="19832-120">Um valor de texto de **PendingDelete** indica que uma caixa de correio de site está aguardando a exclusão.</span><span class="sxs-lookup"><span data-stu-id="19832-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="19832-121">Uma caixa de correio de site deve ser fechada para que possa ser definida como **PendingDelete**.</span><span class="sxs-lookup"><span data-stu-id="19832-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19832-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="19832-122">Remarks</span></span>

<span data-ttu-id="19832-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="19832-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19832-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19832-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19832-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="19832-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19832-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="19832-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19832-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19832-127">Schema name</span></span>  <br/> |<span data-ttu-id="19832-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="19832-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="19832-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19832-129">Validation file</span></span>  <br/> |<span data-ttu-id="19832-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19832-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19832-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="19832-131">Can be empty</span></span>  <br/> ||
   

