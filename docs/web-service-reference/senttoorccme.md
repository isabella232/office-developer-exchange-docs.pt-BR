---
title: SentToOrCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToOrCcMe
api_type:
- schema
ms.assetid: ca43e05d-df37-485b-9276-34678025f2b7
description: O elemento SentToOrCcMe indica se o proprietário da caixa de correio deve ser na propriedade um ToRecipients ou CC das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: baed8f71349c9ec06173d0b494ece688f6fc2c5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825361"
---
# <a name="senttoorccme"></a><span data-ttu-id="7a1ab-103">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="7a1ab-103">SentToOrCcMe</span></span>

<span data-ttu-id="7a1ab-104">O elemento **SentToOrCcMe** indica se o proprietário da caixa de correio deve ser na propriedade um **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-104">The **SentToOrCcMe** element indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
```

 <span data-ttu-id="7a1ab-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7a1ab-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a1ab-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7a1ab-106">Attributes and elements</span></span>

<span data-ttu-id="7a1ab-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a1ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7a1ab-108">Attributes</span></span>

<span data-ttu-id="7a1ab-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a1ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7a1ab-110">Child elements</span></span>

<span data-ttu-id="7a1ab-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a1ab-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7a1ab-112">Parent elements</span></span>

|<span data-ttu-id="7a1ab-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a1ab-113">**Element**</span></span>|<span data-ttu-id="7a1ab-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a1ab-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a1ab-115">Condições</span><span class="sxs-lookup"><span data-stu-id="7a1ab-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7a1ab-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7a1ab-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="7a1ab-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7a1ab-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a1ab-119">Text value</span><span class="sxs-lookup"><span data-stu-id="7a1ab-119">Text value</span></span>

<span data-ttu-id="7a1ab-120">Um valor de texto de **true** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="7a1ab-121">Um valor **false** indica que o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** ou **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7a1ab-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="7a1ab-122">Remarks</span></span>

<span data-ttu-id="7a1ab-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a1ab-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a1ab-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7a1ab-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a1ab-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a1ab-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a1ab-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7a1ab-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7a1ab-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7a1ab-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7a1ab-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7a1ab-128">Validation File</span></span>  <br/> |<span data-ttu-id="7a1ab-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7a1ab-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a1ab-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7a1ab-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a1ab-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="7a1ab-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a1ab-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="7a1ab-132">See also</span></span>



- [<span data-ttu-id="7a1ab-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a1ab-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

