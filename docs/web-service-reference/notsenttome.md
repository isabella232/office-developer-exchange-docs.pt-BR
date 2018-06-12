---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: O elemento NotSentToMe indica se o proprietário da caixa de correio não deve ser na propriedade ToRecipients das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 917648f811855961877d1aba4924573e95e3962a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824555"
---
# <a name="notsenttome"></a><span data-ttu-id="6c6f4-103">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="6c6f4-103">NotSentToMe</span></span>

<span data-ttu-id="6c6f4-104">O elemento **NotSentToMe** indica se o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-104">The **NotSentToMe** element indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 <span data-ttu-id="6c6f4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6c6f4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c6f4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6c6f4-106">Attributes and elements</span></span>

<span data-ttu-id="6c6f4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c6f4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6c6f4-108">Attributes</span></span>

<span data-ttu-id="6c6f4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c6f4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6c6f4-110">Child elements</span></span>

<span data-ttu-id="6c6f4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c6f4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6c6f4-112">Parent elements</span></span>

|<span data-ttu-id="6c6f4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6c6f4-113">**Element**</span></span>|<span data-ttu-id="6c6f4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6c6f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c6f4-115">Condições</span><span class="sxs-lookup"><span data-stu-id="6c6f4-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="6c6f4-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="6c6f4-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="6c6f4-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="6c6f4-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6c6f4-119">Text value</span><span class="sxs-lookup"><span data-stu-id="6c6f4-119">Text value</span></span>

<span data-ttu-id="6c6f4-120">Um valor de texto de **true** indica que o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-120">A text value of **true** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="6c6f4-121">Um valor **false** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** das mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-121">A value of **false** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6c6f4-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6c6f4-122">Remarks</span></span>

<span data-ttu-id="6c6f4-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6c6f4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c6f4-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6c6f4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c6f4-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c6f4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c6f4-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6c6f4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6c6f4-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6c6f4-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c6f4-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6c6f4-128">Validation File</span></span>  <br/> |<span data-ttu-id="6c6f4-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6c6f4-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c6f4-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6c6f4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c6f4-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="6c6f4-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c6f4-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="6c6f4-132">See also</span></span>



- [<span data-ttu-id="6c6f4-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6c6f4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

