---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: O elemento SentOnlyToMe indica se o proprietário da caixa de correio deve ser a única pessoa na propriedade ToRecipients de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 91c31069652a35dc7a38ad6b6e1512cc07d67a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825353"
---
# <a name="sentonlytome"></a><span data-ttu-id="aa846-103">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="aa846-103">SentOnlyToMe</span></span>

<span data-ttu-id="aa846-104">O elemento **SentOnlyToMe** indica se o proprietário da caixa de correio deve ser a única pessoa na propriedade **ToRecipients** de mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="aa846-104">The **SentOnlyToMe** element indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 <span data-ttu-id="aa846-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="aa846-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa846-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aa846-106">Attributes and elements</span></span>

<span data-ttu-id="aa846-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aa846-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa846-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aa846-108">Attributes</span></span>

<span data-ttu-id="aa846-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa846-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa846-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aa846-110">Child elements</span></span>

<span data-ttu-id="aa846-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aa846-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa846-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aa846-112">Parent elements</span></span>

|<span data-ttu-id="aa846-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aa846-113">**Element**</span></span>|<span data-ttu-id="aa846-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aa846-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa846-115">Condições</span><span class="sxs-lookup"><span data-stu-id="aa846-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="aa846-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="aa846-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="aa846-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="aa846-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="aa846-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="aa846-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa846-119">Text value</span><span class="sxs-lookup"><span data-stu-id="aa846-119">Text value</span></span>

<span data-ttu-id="aa846-120">Um valor de texto de **true** indica que o proprietário da caixa de correio deve ser a única pessoa na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="aa846-120">A text value of **true** indicates that the owner of the mailbox must be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="aa846-121">Um valor **false** indica que o proprietário da caixa de correio não deve ser a única pessoa na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="aa846-121">A value of **false** indicates that the owner of the mailbox must not be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aa846-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="aa846-122">Remarks</span></span>

<span data-ttu-id="aa846-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa846-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aa846-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aa846-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa846-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa846-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa846-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aa846-126">Schema Name</span></span>  <br/> |<span data-ttu-id="aa846-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="aa846-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aa846-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aa846-128">Validation File</span></span>  <br/> |<span data-ttu-id="aa846-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aa846-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa846-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aa846-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa846-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="aa846-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa846-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="aa846-132">See also</span></span>



- [<span data-ttu-id="aa846-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aa846-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

