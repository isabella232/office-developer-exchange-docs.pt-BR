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
ms.openlocfilehash: b7dd2f18bd3ef6addeb6d3a7b004510f35b9cb3d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456882"
---
# <a name="percentcomplete"></a><span data-ttu-id="cc883-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="cc883-103">PercentComplete</span></span>

<span data-ttu-id="cc883-104">O elemento **PercentComplete** descreve o status de conclusão de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="cc883-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="cc883-105">**dois**</span><span class="sxs-lookup"><span data-stu-id="cc883-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc883-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cc883-106">Attributes and elements</span></span>

<span data-ttu-id="cc883-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cc883-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc883-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cc883-108">Attributes</span></span>

<span data-ttu-id="cc883-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc883-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc883-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cc883-110">Child elements</span></span>

<span data-ttu-id="cc883-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc883-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc883-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cc883-112">Parent elements</span></span>

|<span data-ttu-id="cc883-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc883-113">**Element**</span></span>|<span data-ttu-id="cc883-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc883-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc883-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="cc883-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="cc883-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc883-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc883-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cc883-117">Text value</span></span>

<span data-ttu-id="cc883-118">Um valor de texto que representa um inteiro entre 0 e 100 é necessário.</span><span class="sxs-lookup"><span data-stu-id="cc883-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc883-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="cc883-119">Remarks</span></span>

<span data-ttu-id="cc883-120">A configuração de **PorcentagemConcluída** como 100 tem o mesmo efeito que configurar o elemento [Completed](completedate.md) ou definir o elemento [status](status.md) como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="cc883-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="cc883-121">Em uma solicitação que define pelo menos duas dessas propriedades, a última Propriedade processada determinará o valor definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="cc883-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="cc883-122">Por exemplo, se a **PorcentagemConcluída** for 100, [Completed](completedate.md) for 1 de janeiro de 2007, e o [status](status.md) não for iniciado, e as propriedades forem transmitidas nesta ordem, o efeito será definir o [status](status.md) da tarefa como não iniciado, [concluída](completedate.md) como **nulo**e a **PorcentagemConcluída** como 0.</span><span class="sxs-lookup"><span data-stu-id="cc883-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="cc883-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cc883-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc883-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cc883-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc883-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc883-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc883-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cc883-126">Schema Name</span></span>  <br/> |<span data-ttu-id="cc883-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cc883-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc883-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cc883-128">Validation File</span></span>  <br/> |<span data-ttu-id="cc883-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cc883-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc883-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cc883-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc883-131">False</span><span class="sxs-lookup"><span data-stu-id="cc883-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc883-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="cc883-132">See also</span></span>



- [<span data-ttu-id="cc883-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cc883-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="cc883-134">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="cc883-134">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="cc883-135">Excluir tarefas</span><span class="sxs-lookup"><span data-stu-id="cc883-135">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

