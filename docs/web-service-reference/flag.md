---
title: Marca
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: O elemento Flag especifica um sinalizador em um item de caixa de correio.
ms.openlocfilehash: 7229a26181ee9baf80be5c32c0ef99483310ccb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466259"
---
# <a name="flag"></a><span data-ttu-id="cd661-103">Marca</span><span class="sxs-lookup"><span data-stu-id="cd661-103">Flag</span></span>

<span data-ttu-id="cd661-104">O elemento **Flag** especifica um sinalizador em um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cd661-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="cd661-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="cd661-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd661-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cd661-106">Attributes and elements</span></span>

<span data-ttu-id="cd661-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd661-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd661-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd661-108">Attributes</span></span>

<span data-ttu-id="cd661-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd661-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd661-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd661-110">Child elements</span></span>

|<span data-ttu-id="cd661-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd661-111">**Element**</span></span>|<span data-ttu-id="cd661-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd661-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd661-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="cd661-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="cd661-114">Contém o status de sinalizador agregado para itens na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="cd661-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="cd661-115">StartDate</span><span class="sxs-lookup"><span data-stu-id="cd661-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="cd661-116">Representa a data de início de um item.</span><span class="sxs-lookup"><span data-stu-id="cd661-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="cd661-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="cd661-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="cd661-118">Representa a data de vencimento de um item.</span><span class="sxs-lookup"><span data-stu-id="cd661-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="cd661-119">Concluído</span><span class="sxs-lookup"><span data-stu-id="cd661-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="cd661-120">Representa a data em que um item foi concluído.</span><span class="sxs-lookup"><span data-stu-id="cd661-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd661-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd661-121">Parent elements</span></span>

|<span data-ttu-id="cd661-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd661-122">**Element**</span></span>|<span data-ttu-id="cd661-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd661-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd661-124">Conversation</span><span class="sxs-lookup"><span data-stu-id="cd661-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="cd661-125">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="cd661-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="cd661-126">Item</span><span class="sxs-lookup"><span data-stu-id="cd661-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="cd661-127">Representa um item genérico no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd661-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd661-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="cd661-128">Remarks</span></span>

<span data-ttu-id="cd661-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cd661-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cd661-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd661-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd661-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cd661-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd661-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd661-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd661-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd661-133">Schema Name</span></span>  <br/> |<span data-ttu-id="cd661-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="cd661-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="cd661-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd661-135">Validation File</span></span>  <br/> |<span data-ttu-id="cd661-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cd661-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd661-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cd661-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cd661-138">Também consulte</span><span class="sxs-lookup"><span data-stu-id="cd661-138">See also</span></span>



- [<span data-ttu-id="cd661-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd661-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

