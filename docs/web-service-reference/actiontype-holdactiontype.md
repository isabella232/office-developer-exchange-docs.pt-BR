---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: O elemento ActionType indica o tipo de ação para a isenção.
ms.openlocfilehash: 8f2796df818dac2bd285b055aa44fbcecd0de5e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457855"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="aea7b-103">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="aea7b-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="aea7b-104">O elemento **ActionType** indica o tipo de ação para a isenção.</span><span class="sxs-lookup"><span data-stu-id="aea7b-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="aea7b-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="aea7b-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aea7b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aea7b-106">Attributes and elements</span></span>

<span data-ttu-id="aea7b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aea7b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aea7b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aea7b-108">Attributes</span></span>

<span data-ttu-id="aea7b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aea7b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aea7b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aea7b-110">Child elements</span></span>

<span data-ttu-id="aea7b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aea7b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aea7b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aea7b-112">Parent elements</span></span>

[<span data-ttu-id="aea7b-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="aea7b-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="aea7b-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="aea7b-114">Text value</span></span>

<span data-ttu-id="aea7b-115">O valor de texto do elemento **ActionType** é o tipo de retenção definido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="aea7b-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="aea7b-116">Um valor de texto de **Create** indica que uma retenção de caixa de correio será criada.</span><span class="sxs-lookup"><span data-stu-id="aea7b-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="aea7b-117">Um valor de texto de **Update** indica que um bloqueio de caixa de correio será atualizado.</span><span class="sxs-lookup"><span data-stu-id="aea7b-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="aea7b-118">Um valor de texto **Remove** indica que uma retenção de caixa de correio será removida.</span><span class="sxs-lookup"><span data-stu-id="aea7b-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aea7b-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="aea7b-119">Remarks</span></span>

<span data-ttu-id="aea7b-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aea7b-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aea7b-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aea7b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aea7b-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aea7b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aea7b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="aea7b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aea7b-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aea7b-124">Schema name</span></span>  <br/> |<span data-ttu-id="aea7b-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aea7b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="aea7b-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aea7b-126">Validation file</span></span>  <br/> |<span data-ttu-id="aea7b-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aea7b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aea7b-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aea7b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="aea7b-129">falso</span><span class="sxs-lookup"><span data-stu-id="aea7b-129">false</span></span>  <br/> |
   

