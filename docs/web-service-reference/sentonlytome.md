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
description: O elemento SentOnlyToMe indica se o proprietário da caixa de correio deve ser a única na propriedade ToRecipients de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 3127550b09d6f5ccf5ba87ad34557afd047f8be0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458646"
---
# <a name="sentonlytome"></a><span data-ttu-id="32879-103">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="32879-103">SentOnlyToMe</span></span>

<span data-ttu-id="32879-104">O elemento **SentOnlyToMe** indica se o proprietário da caixa de correio deve ser a única na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="32879-104">The **SentOnlyToMe** element indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 <span data-ttu-id="32879-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="32879-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32879-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="32879-106">Attributes and elements</span></span>

<span data-ttu-id="32879-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="32879-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32879-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="32879-108">Attributes</span></span>

<span data-ttu-id="32879-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32879-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32879-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="32879-110">Child elements</span></span>

<span data-ttu-id="32879-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32879-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32879-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="32879-112">Parent elements</span></span>

|<span data-ttu-id="32879-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="32879-113">**Element**</span></span>|<span data-ttu-id="32879-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="32879-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32879-115">Condições</span><span class="sxs-lookup"><span data-stu-id="32879-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="32879-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="32879-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="32879-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="32879-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="32879-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="32879-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32879-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="32879-119">Text value</span></span>

<span data-ttu-id="32879-120">Um valor de texto **true** indica que o proprietário da caixa de correio deve ser o único na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="32879-120">A text value of **true** indicates that the owner of the mailbox must be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="32879-121">Um valor **false** indica que o proprietário da caixa de correio não deve ser o único na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="32879-121">A value of **false** indicates that the owner of the mailbox must not be the only one in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="32879-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="32879-122">Remarks</span></span>

<span data-ttu-id="32879-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="32879-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32879-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="32879-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32879-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="32879-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32879-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="32879-126">Schema Name</span></span>  <br/> |<span data-ttu-id="32879-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="32879-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32879-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="32879-128">Validation File</span></span>  <br/> |<span data-ttu-id="32879-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32879-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32879-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="32879-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="32879-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="32879-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32879-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="32879-132">See also</span></span>



- [<span data-ttu-id="32879-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="32879-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

