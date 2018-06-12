---
title: SentCcMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentCcMe
api_type:
- schema
ms.assetid: bf5044e4-cbdf-4e24-a16f-b6454a51fcd5
description: O elemento SentCcMe indica se o proprietário da caixa de correio deve ser na propriedade CC das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 634a83d477efbe8683255c4fab71e3f7f1ab2191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825354"
---
# <a name="sentccme"></a><span data-ttu-id="3fbaf-103">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="3fbaf-103">SentCcMe</span></span>

<span data-ttu-id="3fbaf-104">O elemento **SentCcMe** indica se o proprietário da caixa de correio deve ser na propriedade **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-104">The **SentCcMe** element indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<SentCcMe>true | false</SentCcMe>
```

 <span data-ttu-id="3fbaf-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3fbaf-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fbaf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3fbaf-106">Attributes and elements</span></span>

<span data-ttu-id="3fbaf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fbaf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3fbaf-108">Attributes</span></span>

<span data-ttu-id="3fbaf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fbaf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3fbaf-110">Child elements</span></span>

<span data-ttu-id="3fbaf-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3fbaf-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3fbaf-112">Parent elements</span></span>

|<span data-ttu-id="3fbaf-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3fbaf-113">**Element**</span></span>|<span data-ttu-id="3fbaf-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3fbaf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fbaf-115">Condições</span><span class="sxs-lookup"><span data-stu-id="3fbaf-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3fbaf-116">Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3fbaf-117">Exceções</span><span class="sxs-lookup"><span data-stu-id="3fbaf-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3fbaf-118">Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3fbaf-119">Text value</span><span class="sxs-lookup"><span data-stu-id="3fbaf-119">Text value</span></span>

<span data-ttu-id="3fbaf-120">Um valor de texto de **true** indica que o proprietário da caixa de correio deve estar na propriedade **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-120">A text value of **true** indicates that the owner of the mailbox must be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> <span data-ttu-id="3fbaf-121">Um valor **false** indica que o proprietário da caixa de correio não deve ser na propriedade **Cc** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-121">A value of **false** indicates that the owner of the mailbox must not be in the **CcRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3fbaf-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="3fbaf-122">Remarks</span></span>

<span data-ttu-id="3fbaf-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fbaf-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fbaf-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3fbaf-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fbaf-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3fbaf-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3fbaf-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3fbaf-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3fbaf-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3fbaf-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3fbaf-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3fbaf-128">Validation File</span></span>  <br/> |<span data-ttu-id="3fbaf-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3fbaf-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3fbaf-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3fbaf-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fbaf-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3fbaf-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fbaf-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="3fbaf-132">See also</span></span>



- [<span data-ttu-id="3fbaf-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3fbaf-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

