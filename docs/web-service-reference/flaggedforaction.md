---
title: FlaggedForAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: O elemento FlaggedForAction especifica o sinalizador para o valor da ação que deve aparecer nas mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: f996dc4bcf30db32e1d73fb302ab137f0a6ad4d4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466238"
---
# <a name="flaggedforaction"></a><span data-ttu-id="3d84c-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="3d84c-103">FlaggedForAction</span></span>

<span data-ttu-id="3d84c-104">O elemento **FlaggedForAction** especifica o sinalizador para o valor da ação que deve aparecer nas mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="3d84c-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="3d84c-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="3d84c-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d84c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3d84c-106">Attributes and elements</span></span>

<span data-ttu-id="3d84c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3d84c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d84c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3d84c-108">Attributes</span></span>

<span data-ttu-id="3d84c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d84c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d84c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3d84c-110">Child elements</span></span>

<span data-ttu-id="3d84c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d84c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d84c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3d84c-112">Parent elements</span></span>

|<span data-ttu-id="3d84c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d84c-113">**Element**</span></span>|<span data-ttu-id="3d84c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d84c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d84c-115">Condições</span><span class="sxs-lookup"><span data-stu-id="3d84c-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3d84c-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="3d84c-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3d84c-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="3d84c-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3d84c-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="3d84c-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3d84c-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3d84c-119">Text value</span></span>

<span data-ttu-id="3d84c-120">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d84c-120">A text value is required.</span></span> <span data-ttu-id="3d84c-121">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3d84c-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="3d84c-122">Qualquer tamanho</span><span class="sxs-lookup"><span data-stu-id="3d84c-122">Any</span></span>
    
- <span data-ttu-id="3d84c-123">Chamada</span><span class="sxs-lookup"><span data-stu-id="3d84c-123">Call</span></span>
    
- <span data-ttu-id="3d84c-124">DoNotForward</span><span class="sxs-lookup"><span data-stu-id="3d84c-124">DoNotForward</span></span>
    
- <span data-ttu-id="3d84c-125">Acompanhamento</span><span class="sxs-lookup"><span data-stu-id="3d84c-125">FollowUp</span></span>
    
- <span data-ttu-id="3d84c-126">CONHECIMENTO</span><span class="sxs-lookup"><span data-stu-id="3d84c-126">FYI</span></span>
    
- <span data-ttu-id="3d84c-127">Encaminhar</span><span class="sxs-lookup"><span data-stu-id="3d84c-127">Forward</span></span>
    
- <span data-ttu-id="3d84c-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="3d84c-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="3d84c-129">Ler</span><span class="sxs-lookup"><span data-stu-id="3d84c-129">Read</span></span>
    
- <span data-ttu-id="3d84c-130">Responder</span><span class="sxs-lookup"><span data-stu-id="3d84c-130">Reply</span></span>
    
- <span data-ttu-id="3d84c-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="3d84c-131">ReplyToAll</span></span>
    
- <span data-ttu-id="3d84c-132">Revisão</span><span class="sxs-lookup"><span data-stu-id="3d84c-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="3d84c-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d84c-133">Remarks</span></span>

<span data-ttu-id="3d84c-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d84c-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d84c-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3d84c-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d84c-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d84c-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3d84c-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3d84c-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3d84c-138">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3d84c-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3d84c-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3d84c-139">Validation File</span></span>  <br/> |<span data-ttu-id="3d84c-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3d84c-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d84c-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3d84c-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d84c-142">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3d84c-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d84c-143">Também consulte</span><span class="sxs-lookup"><span data-stu-id="3d84c-143">See also</span></span>



- [<span data-ttu-id="3d84c-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3d84c-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

