---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: O elemento CreateRuleOperation representa uma operação para criar uma nova regra de caixa de entrada.
ms.openlocfilehash: df857544e6d5840a3f738740114195e4c4bb5798
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460768"
---
# <a name="createruleoperation"></a><span data-ttu-id="6e9f4-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6e9f4-103">CreateRuleOperation</span></span>

<span data-ttu-id="6e9f4-104">O elemento **CreateRuleOperation** representa uma operação para criar uma nova regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="6e9f4-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6e9f4-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="6e9f4-106">Operations</span><span class="sxs-lookup"><span data-stu-id="6e9f4-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="6e9f4-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="6e9f4-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e9f4-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6e9f4-108">Attributes and elements</span></span>

<span data-ttu-id="6e9f4-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e9f4-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e9f4-110">Attributes</span></span>

<span data-ttu-id="6e9f4-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e9f4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e9f4-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e9f4-112">Child elements</span></span>

|<span data-ttu-id="6e9f4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e9f4-113">**Element**</span></span>|<span data-ttu-id="6e9f4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e9f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9f4-115">Regra (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6e9f4-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="6e9f4-116">Representa uma regra a ser criada na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e9f4-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e9f4-117">Parent elements</span></span>

|<span data-ttu-id="6e9f4-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e9f4-118">**Element**</span></span>|<span data-ttu-id="6e9f4-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e9f4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e9f4-120">Operations</span><span class="sxs-lookup"><span data-stu-id="6e9f4-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="6e9f4-121">Contém as operações que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e9f4-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6e9f4-122">Text value</span></span>

<span data-ttu-id="6e9f4-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e9f4-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e9f4-124">Remarks</span></span>

<span data-ttu-id="6e9f4-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e9f4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e9f4-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6e9f4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e9f4-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e9f4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e9f4-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e9f4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6e9f4-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6e9f4-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e9f4-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e9f4-130">Validation File</span></span>  <br/> |<span data-ttu-id="6e9f4-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6e9f4-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e9f4-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6e9f4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e9f4-133">False</span><span class="sxs-lookup"><span data-stu-id="6e9f4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e9f4-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="6e9f4-134">See also</span></span>



[<span data-ttu-id="6e9f4-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6e9f4-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="6e9f4-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6e9f4-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="6e9f4-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6e9f4-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="6e9f4-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6e9f4-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

