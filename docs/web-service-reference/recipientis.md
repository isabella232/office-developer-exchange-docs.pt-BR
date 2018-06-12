---
title: RecipientIs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientIs
api_type:
- schema
ms.assetid: 5d2fd7ce-6137-4b3c-a716-c0218dcc8a09
description: O elemento RecipientIs Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos filho valor (ProtectionRuleValueType).
ms.openlocfilehash: b6d5c150cd874d1aced7f2d83ff36409e0738728
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824975"
---
# <a name="recipientis"></a><span data-ttu-id="b4991-103">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="b4991-103">RecipientIs</span></span>

<span data-ttu-id="b4991-104">O elemento **RecipientIs** Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="b4991-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="b4991-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="b4991-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4991-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b4991-106">Attributes and elements</span></span>

<span data-ttu-id="b4991-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b4991-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4991-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b4991-108">Attributes</span></span>

<span data-ttu-id="b4991-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b4991-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4991-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b4991-110">Child elements</span></span>

|<span data-ttu-id="b4991-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b4991-111">**Element**</span></span>|<span data-ttu-id="b4991-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b4991-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4991-113">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="b4991-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="b4991-114">Identifica um destinatário.</span><span class="sxs-lookup"><span data-stu-id="b4991-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4991-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b4991-115">Parent elements</span></span>

|<span data-ttu-id="b4991-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b4991-116">**Element**</span></span>|<span data-ttu-id="b4991-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b4991-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4991-118">Condição</span><span class="sxs-lookup"><span data-stu-id="b4991-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="b4991-119">Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="b4991-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="b4991-120">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="b4991-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="b4991-121">Indica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="b4991-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4991-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="b4991-122">Remarks</span></span>

<span data-ttu-id="b4991-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b4991-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4991-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b4991-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4991-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="b4991-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4991-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b4991-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b4991-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b4991-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4991-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b4991-128">Validation File</span></span>  <br/> |<span data-ttu-id="b4991-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b4991-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4991-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b4991-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4991-131">False</span><span class="sxs-lookup"><span data-stu-id="b4991-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4991-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="b4991-132">See also</span></span>



- [<span data-ttu-id="b4991-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b4991-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

