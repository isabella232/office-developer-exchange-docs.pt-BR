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
description: O elemento SentToOrCcMe indica se o proprietário da caixa de correio deve estar em uma propriedade ToRecipients ou CcRecipients de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 906e5d9fd405b9aa6f772bcedbd1869b5023a05e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462077"
---
# <a name="senttoorccme"></a><span data-ttu-id="d8640-103">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="d8640-103">SentToOrCcMe</span></span>

<span data-ttu-id="d8640-104">O elemento **SentToOrCcMe** indica se o proprietário da caixa de correio deve estar em uma propriedade **ToRecipients** ou **CcRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="d8640-104">The **SentToOrCcMe** element indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToOrCcMe>true | false</SentToOrCcMe>
```

 <span data-ttu-id="d8640-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d8640-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8640-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d8640-106">Attributes and elements</span></span>

<span data-ttu-id="d8640-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8640-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8640-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8640-108">Attributes</span></span>

<span data-ttu-id="d8640-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8640-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8640-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8640-110">Child elements</span></span>

<span data-ttu-id="d8640-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d8640-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8640-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8640-112">Parent elements</span></span>

|<span data-ttu-id="d8640-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8640-113">**Element**</span></span>|<span data-ttu-id="d8640-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8640-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8640-115">Condições</span><span class="sxs-lookup"><span data-stu-id="d8640-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="d8640-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="d8640-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="d8640-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="d8640-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="d8640-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d8640-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8640-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d8640-119">Text value</span></span>

<span data-ttu-id="d8640-120">Um valor de texto **true** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** ou **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="d8640-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="d8640-121">Um valor **false** indica que o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** ou **CcRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="d8640-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** or **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d8640-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8640-122">Remarks</span></span>

<span data-ttu-id="d8640-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8640-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8640-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d8640-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8640-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8640-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d8640-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8640-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d8640-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d8640-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d8640-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8640-128">Validation File</span></span>  <br/> |<span data-ttu-id="d8640-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d8640-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8640-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d8640-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8640-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d8640-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8640-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d8640-132">See also</span></span>



- [<span data-ttu-id="d8640-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d8640-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

