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
description: O elemento FlaggedForAction Especifica o sinalizador para o valor de ação que deverá aparecer nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 5b6e714512edcf12ded2c04f414d047b8622d305
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752323"
---
# <a name="flaggedforaction"></a><span data-ttu-id="8ed8e-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="8ed8e-103">FlaggedForAction</span></span>

<span data-ttu-id="8ed8e-104">O elemento **FlaggedForAction** Especifica o sinalizador para o valor de ação que deverá aparecer nas mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="8ed8e-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="8ed8e-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ed8e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8ed8e-106">Attributes and elements</span></span>

<span data-ttu-id="8ed8e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ed8e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8ed8e-108">Attributes</span></span>

<span data-ttu-id="8ed8e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ed8e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8ed8e-110">Child elements</span></span>

<span data-ttu-id="8ed8e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ed8e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8ed8e-112">Parent elements</span></span>

|<span data-ttu-id="8ed8e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8ed8e-113">**Element**</span></span>|<span data-ttu-id="8ed8e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8ed8e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed8e-115">Condições</span><span class="sxs-lookup"><span data-stu-id="8ed8e-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="8ed8e-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="8ed8e-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="8ed8e-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="8ed8e-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ed8e-119">Text value</span><span class="sxs-lookup"><span data-stu-id="8ed8e-119">Text value</span></span>

<span data-ttu-id="8ed8e-120">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-120">A text value is required.</span></span> <span data-ttu-id="8ed8e-121">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="8ed8e-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="8ed8e-122">Qualquer</span><span class="sxs-lookup"><span data-stu-id="8ed8e-122">Any</span></span>
    
- <span data-ttu-id="8ed8e-123">Chamada</span><span class="sxs-lookup"><span data-stu-id="8ed8e-123">Call</span></span>
    
- <span data-ttu-id="8ed8e-124">DoNotForward</span><span class="sxs-lookup"><span data-stu-id="8ed8e-124">DoNotForward</span></span>
    
- <span data-ttu-id="8ed8e-125">Acompanhamento</span><span class="sxs-lookup"><span data-stu-id="8ed8e-125">FollowUp</span></span>
    
- <span data-ttu-id="8ed8e-126">FYI</span><span class="sxs-lookup"><span data-stu-id="8ed8e-126">FYI</span></span>
    
- <span data-ttu-id="8ed8e-127">Encaminhar</span><span class="sxs-lookup"><span data-stu-id="8ed8e-127">Forward</span></span>
    
- <span data-ttu-id="8ed8e-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="8ed8e-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="8ed8e-129">Ler</span><span class="sxs-lookup"><span data-stu-id="8ed8e-129">Read</span></span>
    
- <span data-ttu-id="8ed8e-130">Responder</span><span class="sxs-lookup"><span data-stu-id="8ed8e-130">Reply</span></span>
    
- <span data-ttu-id="8ed8e-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="8ed8e-131">ReplyToAll</span></span>
    
- <span data-ttu-id="8ed8e-132">Revisão</span><span class="sxs-lookup"><span data-stu-id="8ed8e-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8ed8e-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ed8e-133">Remarks</span></span>

<span data-ttu-id="8ed8e-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ed8e-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ed8e-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8ed8e-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ed8e-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="8ed8e-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ed8e-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8ed8e-137">Schema Name</span></span>  <br/> |<span data-ttu-id="8ed8e-138">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8ed8e-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ed8e-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8ed8e-139">Validation File</span></span>  <br/> |<span data-ttu-id="8ed8e-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8ed8e-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ed8e-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8ed8e-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ed8e-142">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="8ed8e-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ed8e-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="8ed8e-143">See also</span></span>



- [<span data-ttu-id="8ed8e-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8ed8e-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

