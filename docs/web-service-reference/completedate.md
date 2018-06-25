---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: O elemento CompleteDate representa a data em que um item foi concluído.
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751403"
---
# <a name="completedate"></a><span data-ttu-id="56451-103">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="56451-103">CompleteDate</span></span>

<span data-ttu-id="56451-104">O elemento **CompleteDate** representa a data em que um item foi concluído.</span><span class="sxs-lookup"><span data-stu-id="56451-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="56451-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="56451-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56451-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="56451-106">Attributes and elements</span></span>

<span data-ttu-id="56451-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="56451-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56451-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="56451-108">Attributes</span></span>

<span data-ttu-id="56451-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56451-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56451-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="56451-110">Child elements</span></span>

<span data-ttu-id="56451-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56451-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56451-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="56451-112">Parent elements</span></span>

|<span data-ttu-id="56451-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="56451-113">**Element**</span></span>|<span data-ttu-id="56451-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56451-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56451-115">Task</span><span class="sxs-lookup"><span data-stu-id="56451-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="56451-116">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56451-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="56451-117">Flag</span><span class="sxs-lookup"><span data-stu-id="56451-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="56451-118">Especifica um sinalizador em um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56451-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56451-119">Text value</span><span class="sxs-lookup"><span data-stu-id="56451-119">Text value</span></span>

<span data-ttu-id="56451-120">Se este elemento for usado, será necessário um valor de texto que representa a data e hora.</span><span class="sxs-lookup"><span data-stu-id="56451-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56451-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="56451-121">Remarks</span></span>

<span data-ttu-id="56451-122">A definição de **CompleteDate** tem o mesmo efeito que a definição de [PercentComplete](percentcomplete.md) como 100 ou [Status](status.md) como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="56451-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="56451-123">Em uma solicitação que conjuntos de pelo menos dois dessas propriedades, a propriedade processada última determinará o valor que está definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="56451-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="56451-124">Por exemplo, se [PercentComplete](percentcomplete.md) é 100, **CompleteDate** é 1º de janeiro de 2007, [o Status](status.md) é **NotStarted**e as propriedades são transmitidas nesta ordem, o efeito será definir o [Status](status.md) da tarefa a ser **NotStarted **, o [CompleteDate](completedate.md) **Nulo**e [PercentComplete](percentcomplete.md) como 0.</span><span class="sxs-lookup"><span data-stu-id="56451-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="56451-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="56451-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56451-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="56451-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56451-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="56451-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56451-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="56451-128">Schema Name</span></span>  <br/> |<span data-ttu-id="56451-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="56451-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="56451-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="56451-130">Validation File</span></span>  <br/> |<span data-ttu-id="56451-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56451-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56451-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="56451-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="56451-133">False</span><span class="sxs-lookup"><span data-stu-id="56451-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56451-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="56451-134">See also</span></span>



- [<span data-ttu-id="56451-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="56451-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="56451-136">Criação de tarefas</span><span class="sxs-lookup"><span data-stu-id="56451-136">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="56451-137">A exclusão de tarefas</span><span class="sxs-lookup"><span data-stu-id="56451-137">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

