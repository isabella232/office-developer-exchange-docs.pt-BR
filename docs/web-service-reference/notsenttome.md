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
description: O elemento NotSentToMe indica se o proprietário da caixa de correio não deve estar na propriedade ToRecipients das mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 58efe4381fe0c9f5bd0645a9eba471a13b5e4064
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462609"
---
# <a name="notsenttome"></a><span data-ttu-id="2414c-103">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="2414c-103">NotSentToMe</span></span>

<span data-ttu-id="2414c-104">O elemento **NotSentToMe** indica se o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="2414c-104">The **NotSentToMe** element indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 <span data-ttu-id="2414c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2414c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2414c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2414c-106">Attributes and elements</span></span>

<span data-ttu-id="2414c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2414c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2414c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2414c-108">Attributes</span></span>

<span data-ttu-id="2414c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2414c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2414c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2414c-110">Child elements</span></span>

<span data-ttu-id="2414c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2414c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2414c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2414c-112">Parent elements</span></span>

|<span data-ttu-id="2414c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2414c-113">**Element**</span></span>|<span data-ttu-id="2414c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2414c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2414c-115">Condições</span><span class="sxs-lookup"><span data-stu-id="2414c-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="2414c-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="2414c-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="2414c-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="2414c-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="2414c-118">Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="2414c-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2414c-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2414c-119">Text value</span></span>

<span data-ttu-id="2414c-120">Um valor de texto **true** indica que o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="2414c-120">A text value of **true** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="2414c-121">Um valor **false** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** da mensagem de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="2414c-121">A value of **false** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2414c-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="2414c-122">Remarks</span></span>

<span data-ttu-id="2414c-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2414c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2414c-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2414c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2414c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="2414c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2414c-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2414c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2414c-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2414c-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2414c-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2414c-128">Validation File</span></span>  <br/> |<span data-ttu-id="2414c-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2414c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2414c-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2414c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2414c-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="2414c-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2414c-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="2414c-132">See also</span></span>



- [<span data-ttu-id="2414c-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2414c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

