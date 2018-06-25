---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: O elemento ActionType indica o tipo de ação de retenção.
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751036"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="80960-103">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="80960-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="80960-104">O elemento **ActionType** indica o tipo de ação de retenção.</span><span class="sxs-lookup"><span data-stu-id="80960-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="80960-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="80960-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80960-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="80960-106">Attributes and elements</span></span>

<span data-ttu-id="80960-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="80960-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80960-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="80960-108">Attributes</span></span>

<span data-ttu-id="80960-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="80960-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80960-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="80960-110">Child elements</span></span>

<span data-ttu-id="80960-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="80960-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80960-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="80960-112">Parent elements</span></span>

[<span data-ttu-id="80960-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="80960-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="80960-114">Text value</span><span class="sxs-lookup"><span data-stu-id="80960-114">Text value</span></span>

<span data-ttu-id="80960-115">O valor de texto do elemento **ActionType** é o tipo de espera definido em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="80960-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="80960-116">Um valor de texto de **criação** indica que uma isenção de caixa de correio será criada.</span><span class="sxs-lookup"><span data-stu-id="80960-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="80960-117">Um valor de texto da **atualização** indica que uma isenção de caixa de correio será atualizada.</span><span class="sxs-lookup"><span data-stu-id="80960-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="80960-118">Um valor de texto de **Remover** indica que uma isenção de caixa de correio será removida.</span><span class="sxs-lookup"><span data-stu-id="80960-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80960-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="80960-119">Remarks</span></span>

<span data-ttu-id="80960-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="80960-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="80960-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80960-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80960-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="80960-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80960-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="80960-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80960-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="80960-124">Schema name</span></span>  <br/> |<span data-ttu-id="80960-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="80960-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="80960-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="80960-126">Validation file</span></span>  <br/> |<span data-ttu-id="80960-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80960-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80960-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="80960-128">Can be empty</span></span>  <br/> |<span data-ttu-id="80960-129">false</span><span class="sxs-lookup"><span data-stu-id="80960-129">false</span></span>  <br/> |
   

