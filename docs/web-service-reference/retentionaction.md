---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: O elemento RetentionAction especifica a ação executada em itens com a marca de retenção.
ms.openlocfilehash: c16988413e732ddc3cd6ebc355cb73c4d96550c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465230"
---
# <a name="retentionaction"></a><span data-ttu-id="b248b-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="b248b-103">RetentionAction</span></span>

<span data-ttu-id="b248b-104">O elemento **RetentionAction** especifica a ação executada em itens com a marca de retenção.</span><span class="sxs-lookup"><span data-stu-id="b248b-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="b248b-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="b248b-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b248b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b248b-106">Attributes and elements</span></span>

<span data-ttu-id="b248b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b248b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b248b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b248b-108">Attributes</span></span>

<span data-ttu-id="b248b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b248b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b248b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b248b-110">Child elements</span></span>

<span data-ttu-id="b248b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b248b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b248b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b248b-112">Parent elements</span></span>

[<span data-ttu-id="b248b-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="b248b-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="b248b-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b248b-114">Text value</span></span>

<span data-ttu-id="b248b-115">O valor de texto do elemento **RetentionAction** é a ação executada nos itens.</span><span class="sxs-lookup"><span data-stu-id="b248b-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="b248b-116">A lista a seguir contém os valores de texto para o elemento **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="b248b-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="b248b-117">**Nenhuma** -nenhuma ação é executada no item.</span><span class="sxs-lookup"><span data-stu-id="b248b-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="b248b-118">**MoveToDeletedItems** -o item é movido para a pasta itens excluídos padrão.</span><span class="sxs-lookup"><span data-stu-id="b248b-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="b248b-119">**MoveToFolder** -o item é movido para uma pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="b248b-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="b248b-120">**DeleteAndAllowRecovery** -o item é excluído e colocado no dumpster.</span><span class="sxs-lookup"><span data-stu-id="b248b-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="b248b-121">**PermanentlyDelete** -o item é excluído permanentemente da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b248b-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="b248b-122">**MarkAsPastRetentionLimit** -o item está marcado como tendo excedido o limite de tempo de retenção.</span><span class="sxs-lookup"><span data-stu-id="b248b-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="b248b-123">**MoveToArchive** -o item é movido para a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b248b-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="b248b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b248b-124">Remarks</span></span>

<span data-ttu-id="b248b-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b248b-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b248b-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b248b-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b248b-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b248b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b248b-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="b248b-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b248b-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b248b-129">Schema name</span></span>  <br/> |<span data-ttu-id="b248b-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b248b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b248b-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b248b-131">Validation file</span></span>  <br/> |<span data-ttu-id="b248b-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b248b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b248b-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b248b-133">Can be empty</span></span>  <br/> ||
   

