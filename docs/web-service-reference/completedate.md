---
title: Concluído
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
description: O elemento CompleteD representa a data em que um item foi concluído.
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461419"
---
# <a name="completedate"></a><span data-ttu-id="fc646-103">Concluído</span><span class="sxs-lookup"><span data-stu-id="fc646-103">CompleteDate</span></span>

<span data-ttu-id="fc646-104">O elemento **Completed** representa a data em que um item foi concluído.</span><span class="sxs-lookup"><span data-stu-id="fc646-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="fc646-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="fc646-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc646-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc646-106">Attributes and elements</span></span>

<span data-ttu-id="fc646-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc646-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc646-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc646-108">Attributes</span></span>

<span data-ttu-id="fc646-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc646-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc646-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc646-110">Child elements</span></span>

<span data-ttu-id="fc646-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc646-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc646-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc646-112">Parent elements</span></span>

|<span data-ttu-id="fc646-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc646-113">**Element**</span></span>|<span data-ttu-id="fc646-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc646-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc646-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="fc646-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="fc646-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc646-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="fc646-117">Flag</span><span class="sxs-lookup"><span data-stu-id="fc646-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="fc646-118">Especifica um sinalizador em um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fc646-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc646-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fc646-119">Text value</span></span>

<span data-ttu-id="fc646-120">Um valor de texto que representa a data e hora é necessário se esse elemento é usado.</span><span class="sxs-lookup"><span data-stu-id="fc646-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc646-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc646-121">Remarks</span></span>

<span data-ttu-id="fc646-122">A configuração foi **concluída** tem o mesmo efeito que configurar a [PorcentagemConcluída](percentcomplete.md) como 100 ou [status](status.md) como **concluído**.</span><span class="sxs-lookup"><span data-stu-id="fc646-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="fc646-123">Em uma solicitação que define pelo menos duas dessas propriedades, a última Propriedade processada determinará o valor definido para esses elementos.</span><span class="sxs-lookup"><span data-stu-id="fc646-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="fc646-124">Por exemplo, se [a PorcentagemConcluída](percentcomplete.md) for 100, **Completed** for 1 de janeiro de 2007, e o [status](status.md) não for **iniciado**e as propriedades forem transmitidas nessa ordem, o efeito será definir o [status](status.md) da tarefa como não **iniciada**, [concluída](completedate.md) como **nulo**e [PorcentagemConcluída](percentcomplete.md) como 0.</span><span class="sxs-lookup"><span data-stu-id="fc646-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="fc646-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fc646-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc646-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc646-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc646-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc646-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc646-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc646-128">Schema Name</span></span>  <br/> |<span data-ttu-id="fc646-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fc646-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc646-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc646-130">Validation File</span></span>  <br/> |<span data-ttu-id="fc646-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc646-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc646-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc646-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc646-133">False</span><span class="sxs-lookup"><span data-stu-id="fc646-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc646-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc646-134">See also</span></span>



- [<span data-ttu-id="fc646-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc646-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fc646-136">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="fc646-136">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="fc646-137">Excluir tarefas</span><span class="sxs-lookup"><span data-stu-id="fc646-137">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

