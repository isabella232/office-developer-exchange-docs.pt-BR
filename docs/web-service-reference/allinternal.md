---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: O elemento AllInternal retornará true se todos os destinatários de uma mensagem de email são internos para a organização do remetente.
ms.openlocfilehash: 0ffd4178e711e3117497eed682e3fd3e0594989b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751078"
---
# <a name="allinternal"></a><span data-ttu-id="48884-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="48884-103">AllInternal</span></span>

<span data-ttu-id="48884-104">O elemento **AllInternal** é avaliado como **verdadeiro** se todos os destinatários de uma mensagem de email são internos para a organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="48884-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="48884-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="48884-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48884-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="48884-106">Attributes and elements</span></span>

<span data-ttu-id="48884-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="48884-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48884-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="48884-108">Attributes</span></span>

<span data-ttu-id="48884-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48884-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48884-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="48884-110">Child elements</span></span>

<span data-ttu-id="48884-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48884-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48884-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="48884-112">Parent elements</span></span>

|<span data-ttu-id="48884-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48884-113">**Element**</span></span>|<span data-ttu-id="48884-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48884-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48884-115">Condição</span><span class="sxs-lookup"><span data-stu-id="48884-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="48884-116">Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="48884-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="48884-117">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="48884-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="48884-118">Especifica que todos os elementos filho devem corresponder para avaliar como **true**.</span><span class="sxs-lookup"><span data-stu-id="48884-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48884-119">Text value</span><span class="sxs-lookup"><span data-stu-id="48884-119">Text value</span></span>

<span data-ttu-id="48884-120">O elemento **AllInternal** deve estar vazio.</span><span class="sxs-lookup"><span data-stu-id="48884-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="48884-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="48884-121">Remarks</span></span>

<span data-ttu-id="48884-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="48884-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48884-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="48884-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48884-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="48884-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="48884-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="48884-125">Schema Name</span></span>  <br/> |<span data-ttu-id="48884-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="48884-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="48884-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="48884-127">Validation File</span></span>  <br/> |<span data-ttu-id="48884-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="48884-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="48884-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="48884-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="48884-130">False</span><span class="sxs-lookup"><span data-stu-id="48884-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48884-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="48884-131">See also</span></span>

- [<span data-ttu-id="48884-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="48884-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

