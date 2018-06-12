---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: O elemento PercentComplete descreve o status de conclusão de uma tarefa.
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824717"
---
# <a name="percentcomplete"></a><span data-ttu-id="615e9-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="615e9-103">PercentComplete</span></span>

<span data-ttu-id="615e9-104">O elemento **PercentComplete** descreve o status de conclusão de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="615e9-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="615e9-105">**duplo**</span><span class="sxs-lookup"><span data-stu-id="615e9-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="615e9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="615e9-106">Attributes and elements</span></span>

<span data-ttu-id="615e9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="615e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="615e9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="615e9-108">Attributes</span></span>

<span data-ttu-id="615e9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="615e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="615e9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="615e9-110">Child elements</span></span>

<span data-ttu-id="615e9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="615e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="615e9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="615e9-112">Parent elements</span></span>

|<span data-ttu-id="615e9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="615e9-113">**Element**</span></span>|<span data-ttu-id="615e9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="615e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="615e9-115">Task</span><span class="sxs-lookup"><span data-stu-id="615e9-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="615e9-116">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="615e9-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="615e9-117">Text value</span><span class="sxs-lookup"><span data-stu-id="615e9-117">Text value</span></span>

<span data-ttu-id="615e9-118">É necessário um valor de texto que representa um número inteiro entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="615e9-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="615e9-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="615e9-119">Remarks</span></span>

<span data-ttu-id="615e9-120">A definição de **PercentComplete** como 100 tem o mesmo efeito que a configuração do elemento [CompleteDate](completedate.md) ou configuração do elemento de [Status](status.md) como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="615e9-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="615e9-121">Em uma solicitação que conjuntos de pelo menos dois dessas propriedades, a propriedade processada última determinará o valor que está definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="615e9-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="615e9-122">Por exemplo, se **PercentComplete** é 100, [CompleteDate](completedate.md) é 1º de janeiro de 2007, [o Status](status.md) é NotStarted e as propriedades são transmitidas nesta ordem, o efeito será definir o [Status](status.md) da tarefa como NotStarted, o [ CompleteDate](completedate.md) **Nulo**e a **PercentComplete** como 0.</span><span class="sxs-lookup"><span data-stu-id="615e9-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="615e9-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="615e9-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="615e9-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="615e9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="615e9-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="615e9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="615e9-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="615e9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="615e9-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="615e9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="615e9-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="615e9-128">Validation File</span></span>  <br/> |<span data-ttu-id="615e9-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="615e9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="615e9-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="615e9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="615e9-131">False</span><span class="sxs-lookup"><span data-stu-id="615e9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="615e9-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="615e9-132">See also</span></span>



- [<span data-ttu-id="615e9-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="615e9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="615e9-134">Criação de tarefas</span><span class="sxs-lookup"><span data-stu-id="615e9-134">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="615e9-135">A exclusão de tarefas</span><span class="sxs-lookup"><span data-stu-id="615e9-135">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

