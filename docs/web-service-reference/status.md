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
description: O elemento status representa o status de um item de tarefa.
ms.openlocfilehash: 5d022827990b96fd8790ae9566ef49028ebe404c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459956"
---
# <a name="status"></a><span data-ttu-id="f97d6-103">Status</span><span class="sxs-lookup"><span data-stu-id="f97d6-103">Status</span></span>

<span data-ttu-id="f97d6-104">O elemento **status** representa o status de um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="f97d6-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="f97d6-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="f97d6-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f97d6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f97d6-106">Attributes and elements</span></span>

<span data-ttu-id="f97d6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f97d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f97d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f97d6-108">Attributes</span></span>

<span data-ttu-id="f97d6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f97d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f97d6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f97d6-110">Child elements</span></span>

<span data-ttu-id="f97d6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f97d6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f97d6-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f97d6-112">Parent elements</span></span>

|<span data-ttu-id="f97d6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f97d6-113">**Element**</span></span>|<span data-ttu-id="f97d6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f97d6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f97d6-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="f97d6-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="f97d6-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f97d6-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f97d6-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f97d6-117">Text value</span></span>

<span data-ttu-id="f97d6-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f97d6-118">A text value is required.</span></span> <span data-ttu-id="f97d6-119">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f97d6-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="f97d6-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="f97d6-120">NotStarted</span></span>
    
- <span data-ttu-id="f97d6-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="f97d6-121">InProgress</span></span>
    
- <span data-ttu-id="f97d6-122">Completed</span><span class="sxs-lookup"><span data-stu-id="f97d6-122">Completed</span></span>
    
- <span data-ttu-id="f97d6-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="f97d6-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="f97d6-124">Adiado</span><span class="sxs-lookup"><span data-stu-id="f97d6-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f97d6-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="f97d6-125">Remarks</span></span>

<span data-ttu-id="f97d6-126">A configuração foi [concluída](completedate.md) tem o mesmo efeito que configurar a [PorcentagemConcluída](percentcomplete.md) como 100 ou **status** como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="f97d6-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="f97d6-127">Em uma solicitação que define pelo menos duas dessas propriedades, a última Propriedade processada determinará o valor definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="f97d6-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="f97d6-128">Por exemplo, se a **PorcentagemConcluída** é 100 **, Completed** é 1/1/2007, e o **status** é não é iniciado e as propriedades são transmitidas nesta ordem, o efeito será definir o **status** da tarefa como não iniciada, **concluída** como **nulo**e a **PorcentagemConcluída** como 0.</span><span class="sxs-lookup"><span data-stu-id="f97d6-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="f97d6-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f97d6-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f97d6-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f97d6-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f97d6-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="f97d6-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f97d6-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f97d6-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f97d6-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f97d6-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f97d6-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f97d6-134">Validation File</span></span>  <br/> |<span data-ttu-id="f97d6-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f97d6-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f97d6-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f97d6-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f97d6-137">False</span><span class="sxs-lookup"><span data-stu-id="f97d6-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f97d6-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="f97d6-138">See also</span></span>



- [<span data-ttu-id="f97d6-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f97d6-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f97d6-140">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="f97d6-140">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="f97d6-141">Excluir tarefas</span><span class="sxs-lookup"><span data-stu-id="f97d6-141">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

