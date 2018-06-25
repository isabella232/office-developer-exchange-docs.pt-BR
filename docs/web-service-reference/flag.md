---
title: Sinalizador
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: O elemento sinalizador Especifica um sinalizador em um item de caixa de correio.
ms.openlocfilehash: f30f435e8f064d7165ae52de737bbd75b0546206
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752317"
---
# <a name="flag"></a><span data-ttu-id="1f529-103">Sinalizador</span><span class="sxs-lookup"><span data-stu-id="1f529-103">Flag</span></span>

<span data-ttu-id="1f529-104">O elemento **sinalizador** Especifica um sinalizador em um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1f529-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="1f529-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="1f529-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f529-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1f529-106">Attributes and elements</span></span>

<span data-ttu-id="1f529-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1f529-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f529-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1f529-108">Attributes</span></span>

<span data-ttu-id="1f529-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1f529-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f529-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1f529-110">Child elements</span></span>

|<span data-ttu-id="1f529-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1f529-111">**Element**</span></span>|<span data-ttu-id="1f529-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f529-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f529-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="1f529-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="1f529-114">Contém o status do sinalizador agregados para itens na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="1f529-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="1f529-115">StartDate</span><span class="sxs-lookup"><span data-stu-id="1f529-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="1f529-116">Representa a data de início de um item.</span><span class="sxs-lookup"><span data-stu-id="1f529-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="1f529-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="1f529-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="1f529-118">Representa a data quando um item é vencimento.</span><span class="sxs-lookup"><span data-stu-id="1f529-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="1f529-119">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="1f529-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="1f529-120">Representa a data em que um item foi concluído.</span><span class="sxs-lookup"><span data-stu-id="1f529-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f529-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1f529-121">Parent elements</span></span>

|<span data-ttu-id="1f529-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1f529-122">**Element**</span></span>|<span data-ttu-id="1f529-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1f529-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f529-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="1f529-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="1f529-125">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="1f529-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="1f529-126">1.1</span><span class="sxs-lookup"><span data-stu-id="1f529-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="1f529-127">Representa um item genérico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f529-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f529-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="1f529-128">Remarks</span></span>

<span data-ttu-id="1f529-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1f529-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1f529-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f529-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f529-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1f529-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f529-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f529-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f529-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1f529-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1f529-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="1f529-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="1f529-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1f529-135">Validation File</span></span>  <br/> |<span data-ttu-id="1f529-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1f529-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f529-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1f529-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1f529-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="1f529-138">See also</span></span>



- [<span data-ttu-id="1f529-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1f529-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

