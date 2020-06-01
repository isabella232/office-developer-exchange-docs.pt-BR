---
title: SentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentToMe
api_type:
- schema
ms.assetid: f18aecd1-ad33-41c3-b275-4ca648ce1da0
description: O elemento SentToMe indica se o proprietário da caixa de correio deve estar na propriedade ToRecipients de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 830125f03ad91a3e6f2beaf11e41be5e940ed48b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44439921"
---
# <a name="senttome"></a><span data-ttu-id="96b2e-103">SentToMe</span><span class="sxs-lookup"><span data-stu-id="96b2e-103">SentToMe</span></span>

<span data-ttu-id="96b2e-104">O elemento **SentToMe** indica se o proprietário da caixa de correio deve estar na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="96b2e-104">The **SentToMe** element indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentToMe>true | false</SentToMe>
```

 <span data-ttu-id="96b2e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="96b2e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96b2e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="96b2e-106">Attributes and elements</span></span>

<span data-ttu-id="96b2e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96b2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96b2e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="96b2e-108">Attributes</span></span>

<span data-ttu-id="96b2e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96b2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96b2e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96b2e-110">Child elements</span></span>

<span data-ttu-id="96b2e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96b2e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96b2e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96b2e-112">Parent elements</span></span>

|<span data-ttu-id="96b2e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96b2e-113">**Element**</span></span>|<span data-ttu-id="96b2e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96b2e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96b2e-115">Condições</span><span class="sxs-lookup"><span data-stu-id="96b2e-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="96b2e-116">Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="96b2e-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="96b2e-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="96b2e-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="96b2e-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="96b2e-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96b2e-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="96b2e-119">Text value</span></span>

<span data-ttu-id="96b2e-120">Um valor de texto **true** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="96b2e-120">A text value of **true** indicates that the owner of the mailbox must be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="96b2e-121">Um valor **false** indica que o proprietário da caixa de correio não deve estar na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada.</span><span class="sxs-lookup"><span data-stu-id="96b2e-121">A value of **false** indicates that the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="96b2e-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="96b2e-122">Remarks</span></span>

<span data-ttu-id="96b2e-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="96b2e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96b2e-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="96b2e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96b2e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="96b2e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96b2e-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96b2e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="96b2e-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="96b2e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96b2e-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96b2e-128">Validation File</span></span>  <br/> |<span data-ttu-id="96b2e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="96b2e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96b2e-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96b2e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="96b2e-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="96b2e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96b2e-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="96b2e-132">See also</span></span>



- [<span data-ttu-id="96b2e-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96b2e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

