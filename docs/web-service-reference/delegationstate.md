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
ms.openlocfilehash: 00b0e41ae223f1c70f9a3a21662e8858f8690a86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751724"
---
# <a name="delegationstate"></a><span data-ttu-id="4089b-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="4089b-103">DelegationState</span></span>

<span data-ttu-id="4089b-104">O elemento **DelegationState** representa o status de uma tarefa delegada.</span><span class="sxs-lookup"><span data-stu-id="4089b-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="4089b-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="4089b-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4089b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4089b-106">Attributes and elements</span></span>

<span data-ttu-id="4089b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4089b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4089b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4089b-108">Attributes</span></span>

<span data-ttu-id="4089b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4089b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4089b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4089b-110">Child elements</span></span>

<span data-ttu-id="4089b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4089b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4089b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4089b-112">Parent elements</span></span>

|<span data-ttu-id="4089b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4089b-113">**Element**</span></span>|<span data-ttu-id="4089b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4089b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4089b-115">Task</span><span class="sxs-lookup"><span data-stu-id="4089b-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="4089b-116">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4089b-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4089b-117">Text value</span><span class="sxs-lookup"><span data-stu-id="4089b-117">Text value</span></span>

<span data-ttu-id="4089b-118">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4089b-118">This is a read-only property.</span></span> <span data-ttu-id="4089b-119">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="4089b-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="4089b-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="4089b-120">NoMatch</span></span>
    
- <span data-ttu-id="4089b-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="4089b-121">OwnNew</span></span>
    
- <span data-ttu-id="4089b-122">Pertencentes</span><span class="sxs-lookup"><span data-stu-id="4089b-122">Owned</span></span>
    
- <span data-ttu-id="4089b-123">Aceito</span><span class="sxs-lookup"><span data-stu-id="4089b-123">Accepted</span></span>
    
- <span data-ttu-id="4089b-124">Recusada</span><span class="sxs-lookup"><span data-stu-id="4089b-124">Declined</span></span>
    
- <span data-ttu-id="4089b-125">Máx.</span><span class="sxs-lookup"><span data-stu-id="4089b-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="4089b-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4089b-126">Remarks</span></span>

<span data-ttu-id="4089b-127">Serviços Web do Exchange no Microsoft Exchange Server 2007 não oferece suporte a atribuições de tarefa.</span><span class="sxs-lookup"><span data-stu-id="4089b-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="4089b-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4089b-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4089b-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4089b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4089b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="4089b-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4089b-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4089b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="4089b-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4089b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="4089b-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4089b-133">Validation File</span></span>  <br/> |<span data-ttu-id="4089b-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4089b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4089b-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4089b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="4089b-136">False</span><span class="sxs-lookup"><span data-stu-id="4089b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4089b-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="4089b-137">See also</span></span>

- [<span data-ttu-id="4089b-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4089b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

