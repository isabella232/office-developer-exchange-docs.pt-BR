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
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468051"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="7c611-103">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="7c611-103">IsAssignmentEditable</span></span>

<span data-ttu-id="7c611-104">O elemento **IsAssignmentEditable** representa o tipo de tarefa.</span><span class="sxs-lookup"><span data-stu-id="7c611-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="7c611-105">**Semantic**</span><span class="sxs-lookup"><span data-stu-id="7c611-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c611-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7c611-106">Attributes and elements</span></span>

<span data-ttu-id="7c611-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7c611-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c611-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7c611-108">Attributes</span></span>

<span data-ttu-id="7c611-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c611-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c611-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7c611-110">Child elements</span></span>

<span data-ttu-id="7c611-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7c611-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c611-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7c611-112">Parent elements</span></span>

|<span data-ttu-id="7c611-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c611-113">**Element**</span></span>|<span data-ttu-id="7c611-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c611-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c611-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="7c611-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="7c611-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c611-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c611-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7c611-117">Text value</span></span>

<span data-ttu-id="7c611-118">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c611-118">This property is read-only.</span></span> <span data-ttu-id="7c611-119">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="7c611-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="7c611-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7c611-120">**Value**</span></span>|<span data-ttu-id="7c611-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c611-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c611-122">,0</span><span class="sxs-lookup"><span data-stu-id="7c611-122">0</span></span>  <br/> |<span data-ttu-id="7c611-123">O padrão para todos os itens de tarefa.</span><span class="sxs-lookup"><span data-stu-id="7c611-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="7c611-124">1 </span><span class="sxs-lookup"><span data-stu-id="7c611-124">1</span></span>  <br/> |<span data-ttu-id="7c611-125">Uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="7c611-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="7c611-126">duas</span><span class="sxs-lookup"><span data-stu-id="7c611-126">2</span></span>  <br/> |<span data-ttu-id="7c611-127">Uma aceitação de tarefa de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="7c611-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="7c611-128">3D</span><span class="sxs-lookup"><span data-stu-id="7c611-128">3</span></span>  <br/> |<span data-ttu-id="7c611-129">Um declínio de tarefa de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="7c611-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="7c611-130">4 </span><span class="sxs-lookup"><span data-stu-id="7c611-130">4</span></span>  <br/> |<span data-ttu-id="7c611-131">Uma atualização para uma solicitação de tarefa anterior.</span><span class="sxs-lookup"><span data-stu-id="7c611-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="7c611-132">5 </span><span class="sxs-lookup"><span data-stu-id="7c611-132">5</span></span>  <br/> |<span data-ttu-id="7c611-133">Não usado.</span><span class="sxs-lookup"><span data-stu-id="7c611-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c611-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="7c611-134">Remarks</span></span>

<span data-ttu-id="7c611-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7c611-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c611-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7c611-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c611-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c611-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c611-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7c611-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7c611-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7c611-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c611-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7c611-140">Validation File</span></span>  <br/> |<span data-ttu-id="7c611-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7c611-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c611-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7c611-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c611-143">False</span><span class="sxs-lookup"><span data-stu-id="7c611-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c611-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="7c611-144">See also</span></span>



- [<span data-ttu-id="7c611-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7c611-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

