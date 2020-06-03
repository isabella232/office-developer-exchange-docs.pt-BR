---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: O elemento MovedItemId especifica o identificador do item que foi movido pela operação MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468611"
---
# <a name="moveditemid"></a><span data-ttu-id="e1a64-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="e1a64-103">MovedItemId</span></span>

<span data-ttu-id="e1a64-104">O elemento **MovedItemId** especifica o identificador do item que foi movido pela operação **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="e1a64-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="e1a64-105">**ItemIdtype**</span><span class="sxs-lookup"><span data-stu-id="e1a64-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1a64-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1a64-106">Attributes and elements</span></span>

<span data-ttu-id="e1a64-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1a64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1a64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1a64-108">Attributes</span></span>

|<span data-ttu-id="e1a64-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e1a64-109">**Attribute**</span></span>|<span data-ttu-id="e1a64-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1a64-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1a64-111">Id</span><span class="sxs-lookup"><span data-stu-id="e1a64-111">Id</span></span>  <br/> |<span data-ttu-id="e1a64-112">O valor do atributo **ID** é o identificador do item que é movido pela operação **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="e1a64-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="e1a64-113">O identificador de item permanecerá o mesmo após a movimentação.</span><span class="sxs-lookup"><span data-stu-id="e1a64-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="e1a64-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="e1a64-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="e1a64-115">O valor do atributo **ChangeKey** é a chave de alteração do item movido.</span><span class="sxs-lookup"><span data-stu-id="e1a64-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="e1a64-116">A chave Change muda após o item ser movido pela operação **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="e1a64-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e1a64-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1a64-117">Child elements</span></span>

<span data-ttu-id="e1a64-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1a64-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1a64-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1a64-119">Parent elements</span></span>

[<span data-ttu-id="e1a64-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1a64-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="e1a64-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1a64-121">Remarks</span></span>

<span data-ttu-id="e1a64-122">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e1a64-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e1a64-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1a64-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1a64-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e1a64-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1a64-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1a64-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e1a64-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1a64-126">Schema name</span></span>  <br/> |<span data-ttu-id="e1a64-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e1a64-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e1a64-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1a64-128">Validation file</span></span>  <br/> |<span data-ttu-id="e1a64-129">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e1a64-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e1a64-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e1a64-130">Can be empty</span></span>  <br/> ||
   

