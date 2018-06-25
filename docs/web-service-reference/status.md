---
title: Status
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: O elemento de Status representa o status de um item de tarefa.
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825584"
---
# <a name="status"></a><span data-ttu-id="d5e07-103">Status</span><span class="sxs-lookup"><span data-stu-id="d5e07-103">Status</span></span>

<span data-ttu-id="d5e07-104">O elemento de **Status** representa o status de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="d5e07-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="d5e07-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="d5e07-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5e07-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d5e07-106">Attributes and elements</span></span>

<span data-ttu-id="d5e07-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d5e07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5e07-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d5e07-108">Attributes</span></span>

<span data-ttu-id="d5e07-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d5e07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5e07-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d5e07-110">Child elements</span></span>

<span data-ttu-id="d5e07-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d5e07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5e07-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d5e07-112">Parent elements</span></span>

|<span data-ttu-id="d5e07-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d5e07-113">**Element**</span></span>|<span data-ttu-id="d5e07-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d5e07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5e07-115">Task</span><span class="sxs-lookup"><span data-stu-id="d5e07-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="d5e07-116">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5e07-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d5e07-117">Text value</span><span class="sxs-lookup"><span data-stu-id="d5e07-117">Text value</span></span>

<span data-ttu-id="d5e07-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="d5e07-118">A text value is required.</span></span> <span data-ttu-id="d5e07-119">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d5e07-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="d5e07-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="d5e07-120">NotStarted</span></span>
    
- <span data-ttu-id="d5e07-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="d5e07-121">InProgress</span></span>
    
- <span data-ttu-id="d5e07-122">Completed</span><span class="sxs-lookup"><span data-stu-id="d5e07-122">Completed</span></span>
    
- <span data-ttu-id="d5e07-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="d5e07-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="d5e07-124">Adiada</span><span class="sxs-lookup"><span data-stu-id="d5e07-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="d5e07-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="d5e07-125">Remarks</span></span>

<span data-ttu-id="d5e07-126">A definição de [CompleteDate](completedate.md) tem o mesmo efeito que a definição de [PercentComplete](percentcomplete.md) como 100 ou **Status** como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="d5e07-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="d5e07-127">Em uma solicitação que conjuntos de pelo menos dois dessas propriedades, a propriedade processada última determinará o valor que está definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="d5e07-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="d5e07-128">Por exemplo, se **PercentComplete** for 100, **CompleteDate** é 1/1/2007 e **o Status** é NotStarted e as propriedades são transmitidas nesta ordem, o efeito será definir o **Status** da tarefa como NotStarted, o **CompleteDate ** **Nulo**e a **PercentComplete** como 0.</span><span class="sxs-lookup"><span data-stu-id="d5e07-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="d5e07-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d5e07-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5e07-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d5e07-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5e07-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5e07-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5e07-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d5e07-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d5e07-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d5e07-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5e07-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d5e07-134">Validation File</span></span>  <br/> |<span data-ttu-id="d5e07-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5e07-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5e07-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d5e07-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5e07-137">False</span><span class="sxs-lookup"><span data-stu-id="d5e07-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5e07-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="d5e07-138">See also</span></span>



- [<span data-ttu-id="d5e07-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d5e07-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d5e07-140">Criação de tarefas</span><span class="sxs-lookup"><span data-stu-id="d5e07-140">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="d5e07-141">A exclusão de tarefas</span><span class="sxs-lookup"><span data-stu-id="d5e07-141">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

