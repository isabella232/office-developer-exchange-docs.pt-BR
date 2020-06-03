---
title: InboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxRules
api_type:
- schema
ms.assetid: 7bb9896c-bd12-49ae-842a-a10b5f9a2ef6
description: O elemento InboxRules representa uma matriz de regras na caixa de correio do usuário.
ms.openlocfilehash: a3107c3c317a912d0bd3e60d03da4168f2f3a0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458268"
---
# <a name="inboxrules"></a><span data-ttu-id="796a7-103">InboxRules</span><span class="sxs-lookup"><span data-stu-id="796a7-103">InboxRules</span></span>

<span data-ttu-id="796a7-104">O elemento **InboxRules** representa uma matriz de regras na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="796a7-104">The **InboxRules** element represents an array of rules in the user's mailbox.</span></span> 
  
[<span data-ttu-id="796a7-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="796a7-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="796a7-106">InboxRules</span><span class="sxs-lookup"><span data-stu-id="796a7-106">InboxRules</span></span>](inboxrules.md)
  
```XML
<InboxRules>
   <Rule/>
</InboxRules>
```

 <span data-ttu-id="796a7-107">**ArrayOfRulesType**</span><span class="sxs-lookup"><span data-stu-id="796a7-107">**ArrayOfRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="796a7-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="796a7-108">Attributes and elements</span></span>

<span data-ttu-id="796a7-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="796a7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="796a7-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="796a7-110">Attributes</span></span>

<span data-ttu-id="796a7-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="796a7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="796a7-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="796a7-112">Child elements</span></span>

|<span data-ttu-id="796a7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="796a7-113">**Element**</span></span>|<span data-ttu-id="796a7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="796a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="796a7-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="796a7-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="796a7-116">Contém uma única regra e representa uma regra na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="796a7-116">Contains a single rule and represents a rule in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="796a7-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="796a7-117">Parent elements</span></span>

|<span data-ttu-id="796a7-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="796a7-118">**Element**</span></span>|<span data-ttu-id="796a7-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="796a7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="796a7-120">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="796a7-120">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="796a7-121">Define uma resposta a uma solicitação de [operação GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="796a7-121">Defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="796a7-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="796a7-122">Text value</span></span>

<span data-ttu-id="796a7-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="796a7-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="796a7-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="796a7-124">Remarks</span></span>

<span data-ttu-id="796a7-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="796a7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="796a7-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="796a7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="796a7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="796a7-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="796a7-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="796a7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="796a7-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="796a7-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="796a7-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="796a7-130">Validation File</span></span>  <br/> |<span data-ttu-id="796a7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="796a7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="796a7-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="796a7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="796a7-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="796a7-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="796a7-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="796a7-134">See also</span></span>



[<span data-ttu-id="796a7-135">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="796a7-135">GetInboxRules</span></span>](getinboxrules.md)
  
[<span data-ttu-id="796a7-136">Operação GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="796a7-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)


- [<span data-ttu-id="796a7-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="796a7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

