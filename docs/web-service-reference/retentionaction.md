---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: O elemento RetentionAction Especifica a ação executada em itens com a marca de retenção.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825215"
---
# <a name="retentionaction"></a><span data-ttu-id="9c8eb-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="9c8eb-103">RetentionAction</span></span>

<span data-ttu-id="9c8eb-104">O elemento **RetentionAction** Especifica a ação executada em itens com a marca de retenção.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="9c8eb-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="9c8eb-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c8eb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9c8eb-106">Attributes and elements</span></span>

<span data-ttu-id="9c8eb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c8eb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9c8eb-108">Attributes</span></span>

<span data-ttu-id="9c8eb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c8eb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9c8eb-110">Child elements</span></span>

<span data-ttu-id="9c8eb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c8eb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9c8eb-112">Parent elements</span></span>

[<span data-ttu-id="9c8eb-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="9c8eb-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="9c8eb-114">Text value</span><span class="sxs-lookup"><span data-stu-id="9c8eb-114">Text value</span></span>

<span data-ttu-id="9c8eb-115">O valor de texto do elemento **RetentionAction** é a ação executada em itens.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="9c8eb-116">A lista a seguir contém os valores de texto para o elemento **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="9c8eb-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="9c8eb-117">**None** - nenhuma ação é executada no item.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="9c8eb-118">**MoveToDeletedItems** - o item é movido para a pasta de itens excluídos padrão.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="9c8eb-119">**MoveToFolder** - o item é movido para uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="9c8eb-120">**DeleteAndAllowRecovery** - o item é excluído e colocar no Dumpster de.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="9c8eb-121">**PermanentlyDelete** - o item é excluído permanentemente da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="9c8eb-122">**MarkAsPastRetentionLimit** - o item está marcado como tendo excedeu o limite de tempo de retenção.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="9c8eb-123">**MoveToArchive** - o item é movido para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="9c8eb-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c8eb-124">Remarks</span></span>

<span data-ttu-id="9c8eb-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9c8eb-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c8eb-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c8eb-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9c8eb-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c8eb-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c8eb-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c8eb-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9c8eb-129">Schema name</span></span>  <br/> |<span data-ttu-id="9c8eb-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9c8eb-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c8eb-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9c8eb-131">Validation file</span></span>  <br/> |<span data-ttu-id="9c8eb-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c8eb-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c8eb-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9c8eb-133">Can be empty</span></span>  <br/> ||
   

