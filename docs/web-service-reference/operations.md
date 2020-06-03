---
title: Operações
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Operations
api_type:
- schema
ms.assetid: d8cd41b1-28ae-4c95-9ff6-8b25c8e18306
description: O elemento Operations contém uma matriz de operações de regra que podem ser executadas em uma caixa de entrada.
ms.openlocfilehash: 4bbec4ad6424f802bb6781a870d65f23705e88c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462483"
---
# <a name="operations"></a><span data-ttu-id="92ede-103">Operações</span><span class="sxs-lookup"><span data-stu-id="92ede-103">Operations</span></span>

<span data-ttu-id="92ede-104">O elemento **Operations** contém uma matriz de operações de regra que podem ser executadas em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="92ede-104">The **Operations** element contains an array of rule operations that can be performed on an Inbox.</span></span> 
  
[<span data-ttu-id="92ede-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92ede-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
```XML
<Operations>
    <CreateRuleOperation/>
    <SetRuleOperation/>
    <DeleteRuleOperation/>
</Operations>
```

 <span data-ttu-id="92ede-106">**ArrayOfRuleOperationsType**</span><span class="sxs-lookup"><span data-stu-id="92ede-106">**ArrayOfRuleOperationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92ede-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="92ede-107">Attributes and elements</span></span>

<span data-ttu-id="92ede-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="92ede-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92ede-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="92ede-109">Attributes</span></span>

<span data-ttu-id="92ede-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92ede-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92ede-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="92ede-111">Child elements</span></span>

|<span data-ttu-id="92ede-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92ede-112">**Element**</span></span>|<span data-ttu-id="92ede-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92ede-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92ede-114">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92ede-114">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="92ede-115">Representa uma operação para criar uma nova regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="92ede-115">Represents an operation to create a new Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="92ede-116">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92ede-116">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="92ede-117">Representa uma operação para atualizar uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="92ede-117">Represents an operation to update an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="92ede-118">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="92ede-118">DeleteRuleOperation</span></span>](deleteruleoperation.md) <br/> |<span data-ttu-id="92ede-119">Representa uma operação para excluir uma regra de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="92ede-119">Represents an operation to delete an Inbox rule.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92ede-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="92ede-120">Parent elements</span></span>

|<span data-ttu-id="92ede-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92ede-121">**Element**</span></span>|<span data-ttu-id="92ede-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92ede-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92ede-123">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92ede-123">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="92ede-124">Define uma solicitação para atualizar as regras de caixa de entrada em uma caixa de correio no repositório do servidor.</span><span class="sxs-lookup"><span data-stu-id="92ede-124">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="92ede-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="92ede-125">Remarks</span></span>

<span data-ttu-id="92ede-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ede-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92ede-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="92ede-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92ede-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="92ede-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92ede-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="92ede-129">Schema Name</span></span>  <br/> |<span data-ttu-id="92ede-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="92ede-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="92ede-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="92ede-131">Validation File</span></span>  <br/> |<span data-ttu-id="92ede-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="92ede-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92ede-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="92ede-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="92ede-134">False</span><span class="sxs-lookup"><span data-stu-id="92ede-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92ede-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="92ede-135">See also</span></span>



[<span data-ttu-id="92ede-136">Operação UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="92ede-136">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="92ede-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="92ede-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

