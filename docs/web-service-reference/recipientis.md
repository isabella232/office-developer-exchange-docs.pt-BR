---
title: Destinatário
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
description: O elemento Recipientis especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos de valor filho (ProtectionRuleValueType).
ms.openlocfilehash: 8f27c4484ce310c62f9bab0e6ffeea2bfac1d3ef
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463878"
---
# <a name="recipientis"></a><span data-ttu-id="79917-103">Destinatário</span><span class="sxs-lookup"><span data-stu-id="79917-103">RecipientIs</span></span>

<span data-ttu-id="79917-104">O elemento **recipientis** especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="79917-104">The **RecipientIs** element specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```xml
<RecipientIs>   <Value/></RecipientIs>
```

 <span data-ttu-id="79917-105">**ProtectionRuleRecipientIsType**</span><span class="sxs-lookup"><span data-stu-id="79917-105">**ProtectionRuleRecipientIsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79917-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="79917-106">Attributes and elements</span></span>

<span data-ttu-id="79917-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="79917-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79917-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="79917-108">Attributes</span></span>

<span data-ttu-id="79917-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79917-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79917-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="79917-110">Child elements</span></span>

|<span data-ttu-id="79917-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="79917-111">**Element**</span></span>|<span data-ttu-id="79917-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="79917-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79917-113">Valor (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="79917-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="79917-114">Identifica um destinatário.</span><span class="sxs-lookup"><span data-stu-id="79917-114">Identifies a recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79917-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="79917-115">Parent elements</span></span>

|<span data-ttu-id="79917-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="79917-116">**Element**</span></span>|<span data-ttu-id="79917-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="79917-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79917-118">Condição</span><span class="sxs-lookup"><span data-stu-id="79917-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="79917-119">Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="79917-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="79917-120">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="79917-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="79917-121">Indica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="79917-121">Indicates that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="79917-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="79917-122">Remarks</span></span>

<span data-ttu-id="79917-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="79917-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79917-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="79917-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79917-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="79917-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79917-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="79917-126">Schema Name</span></span>  <br/> |<span data-ttu-id="79917-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="79917-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="79917-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="79917-128">Validation File</span></span>  <br/> |<span data-ttu-id="79917-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="79917-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79917-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="79917-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="79917-131">False</span><span class="sxs-lookup"><span data-stu-id="79917-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79917-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="79917-132">See also</span></span>



- [<span data-ttu-id="79917-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="79917-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

