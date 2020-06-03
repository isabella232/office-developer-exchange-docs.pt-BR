---
title: Interno
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
description: O elemento myinterna é avaliado como true se todos os destinatários de uma mensagem de email são internos para a organização do remetente.
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464830"
---
# <a name="allinternal"></a><span data-ttu-id="007d5-103">Interno</span><span class="sxs-lookup"><span data-stu-id="007d5-103">AllInternal</span></span>

<span data-ttu-id="007d5-104">O elemento **myinterna** é avaliado como **true** se todos os destinatários de uma mensagem de email são internos para a organização do remetente.</span><span class="sxs-lookup"><span data-stu-id="007d5-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="007d5-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="007d5-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="007d5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="007d5-106">Attributes and elements</span></span>

<span data-ttu-id="007d5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="007d5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="007d5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="007d5-108">Attributes</span></span>

<span data-ttu-id="007d5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="007d5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="007d5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="007d5-110">Child elements</span></span>

<span data-ttu-id="007d5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="007d5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="007d5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="007d5-112">Parent elements</span></span>

|<span data-ttu-id="007d5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="007d5-113">**Element**</span></span>|<span data-ttu-id="007d5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="007d5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="007d5-115">Condição</span><span class="sxs-lookup"><span data-stu-id="007d5-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="007d5-116">Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.</span><span class="sxs-lookup"><span data-stu-id="007d5-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="007d5-117">E (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="007d5-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="007d5-118">Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**.</span><span class="sxs-lookup"><span data-stu-id="007d5-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="007d5-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="007d5-119">Text value</span></span>

<span data-ttu-id="007d5-120">O elemento **interno** deve estar vazio.</span><span class="sxs-lookup"><span data-stu-id="007d5-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="007d5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="007d5-121">Remarks</span></span>

<span data-ttu-id="007d5-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="007d5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="007d5-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="007d5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="007d5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="007d5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="007d5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="007d5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="007d5-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="007d5-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="007d5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="007d5-127">Validation File</span></span>  <br/> |<span data-ttu-id="007d5-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="007d5-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="007d5-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="007d5-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="007d5-130">False</span><span class="sxs-lookup"><span data-stu-id="007d5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="007d5-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="007d5-131">See also</span></span>

- [<span data-ttu-id="007d5-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="007d5-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

