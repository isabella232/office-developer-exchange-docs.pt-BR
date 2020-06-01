---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: O elemento DelegationState representa o status de uma tarefa delegada.
ms.openlocfilehash: b938b5a2240283c265006dd47cd6ff475ad80978
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457365"
---
# <a name="delegationstate"></a><span data-ttu-id="021b1-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="021b1-103">DelegationState</span></span>

<span data-ttu-id="021b1-104">O elemento **DelegationState** representa o status de uma tarefa delegada.</span><span class="sxs-lookup"><span data-stu-id="021b1-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="021b1-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="021b1-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="021b1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="021b1-106">Attributes and elements</span></span>

<span data-ttu-id="021b1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="021b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="021b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="021b1-108">Attributes</span></span>

<span data-ttu-id="021b1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="021b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="021b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="021b1-110">Child elements</span></span>

<span data-ttu-id="021b1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="021b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="021b1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="021b1-112">Parent elements</span></span>

|<span data-ttu-id="021b1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="021b1-113">**Element**</span></span>|<span data-ttu-id="021b1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="021b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="021b1-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="021b1-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="021b1-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="021b1-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="021b1-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="021b1-117">Text value</span></span>

<span data-ttu-id="021b1-118">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="021b1-118">This is a read-only property.</span></span> <span data-ttu-id="021b1-119">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="021b1-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="021b1-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="021b1-120">NoMatch</span></span>
    
- <span data-ttu-id="021b1-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="021b1-121">OwnNew</span></span>
    
- <span data-ttu-id="021b1-122">Possuir</span><span class="sxs-lookup"><span data-stu-id="021b1-122">Owned</span></span>
    
- <span data-ttu-id="021b1-123">Accepted</span><span class="sxs-lookup"><span data-stu-id="021b1-123">Accepted</span></span>
    
- <span data-ttu-id="021b1-124">Recusada</span><span class="sxs-lookup"><span data-stu-id="021b1-124">Declined</span></span>
    
- <span data-ttu-id="021b1-125">Máx.</span><span class="sxs-lookup"><span data-stu-id="021b1-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="021b1-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="021b1-126">Remarks</span></span>

<span data-ttu-id="021b1-127">Os serviços Web do Exchange no Microsoft Exchange Server 2007 não dão suporte a atribuições de tarefas.</span><span class="sxs-lookup"><span data-stu-id="021b1-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="021b1-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="021b1-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="021b1-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="021b1-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="021b1-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="021b1-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="021b1-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="021b1-131">Schema Name</span></span>  <br/> |<span data-ttu-id="021b1-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="021b1-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="021b1-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="021b1-133">Validation File</span></span>  <br/> |<span data-ttu-id="021b1-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="021b1-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="021b1-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="021b1-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="021b1-136">False</span><span class="sxs-lookup"><span data-stu-id="021b1-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="021b1-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="021b1-137">See also</span></span>

- [<span data-ttu-id="021b1-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="021b1-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

