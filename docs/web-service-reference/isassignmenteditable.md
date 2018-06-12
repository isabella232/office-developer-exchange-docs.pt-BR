---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: O elemento IsAssignmentEditable representa o tipo de tarefa.
ms.openlocfilehash: 91922c4d6abd4d88ac9e36dd3d4c0224fc1ee716
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823992"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="64e51-103">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="64e51-103">IsAssignmentEditable</span></span>

<span data-ttu-id="64e51-104">O elemento **IsAssignmentEditable** representa o tipo de tarefa.</span><span class="sxs-lookup"><span data-stu-id="64e51-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="64e51-105">**inteiro**</span><span class="sxs-lookup"><span data-stu-id="64e51-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64e51-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="64e51-106">Attributes and elements</span></span>

<span data-ttu-id="64e51-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="64e51-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64e51-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="64e51-108">Attributes</span></span>

<span data-ttu-id="64e51-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="64e51-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64e51-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="64e51-110">Child elements</span></span>

<span data-ttu-id="64e51-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="64e51-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64e51-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="64e51-112">Parent elements</span></span>

|<span data-ttu-id="64e51-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64e51-113">**Element**</span></span>|<span data-ttu-id="64e51-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64e51-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64e51-115">Task</span><span class="sxs-lookup"><span data-stu-id="64e51-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="64e51-116">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="64e51-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="64e51-117">Text value</span><span class="sxs-lookup"><span data-stu-id="64e51-117">Text value</span></span>

<span data-ttu-id="64e51-118">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64e51-118">This property is read-only.</span></span> <span data-ttu-id="64e51-119">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="64e51-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="64e51-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="64e51-120">**Value**</span></span>|<span data-ttu-id="64e51-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64e51-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64e51-122">0</span><span class="sxs-lookup"><span data-stu-id="64e51-122">0</span></span>  <br/> |<span data-ttu-id="64e51-123">O padrão para todos os itens de tarefa.</span><span class="sxs-lookup"><span data-stu-id="64e51-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="64e51-124">1</span><span class="sxs-lookup"><span data-stu-id="64e51-124">1</span></span>  <br/> |<span data-ttu-id="64e51-125">Uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="64e51-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="64e51-126">2</span><span class="sxs-lookup"><span data-stu-id="64e51-126">2</span></span>  <br/> |<span data-ttu-id="64e51-127">Aceitação de uma tarefa a partir de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="64e51-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="64e51-128">3</span><span class="sxs-lookup"><span data-stu-id="64e51-128">3</span></span>  <br/> |<span data-ttu-id="64e51-129">Recusa de uma tarefa a partir de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="64e51-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="64e51-130">4</span><span class="sxs-lookup"><span data-stu-id="64e51-130">4</span></span>  <br/> |<span data-ttu-id="64e51-131">Uma atualização para uma solicitação de tarefa anterior.</span><span class="sxs-lookup"><span data-stu-id="64e51-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="64e51-132">5</span><span class="sxs-lookup"><span data-stu-id="64e51-132">5</span></span>  <br/> |<span data-ttu-id="64e51-133">Não usado.</span><span class="sxs-lookup"><span data-stu-id="64e51-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64e51-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="64e51-134">Remarks</span></span>

<span data-ttu-id="64e51-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="64e51-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64e51-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="64e51-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64e51-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="64e51-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64e51-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="64e51-138">Schema Name</span></span>  <br/> |<span data-ttu-id="64e51-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="64e51-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="64e51-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="64e51-140">Validation File</span></span>  <br/> |<span data-ttu-id="64e51-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64e51-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64e51-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="64e51-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="64e51-143">False</span><span class="sxs-lookup"><span data-stu-id="64e51-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64e51-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="64e51-144">See also</span></span>



- [<span data-ttu-id="64e51-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="64e51-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

