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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468051"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="cf4bd-103">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="cf4bd-103">IsAssignmentEditable</span></span>

<span data-ttu-id="cf4bd-104">O elemento **IsAssignmentEditable** representa o tipo de tarefa.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="cf4bd-105">**Semantic**</span><span class="sxs-lookup"><span data-stu-id="cf4bd-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf4bd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cf4bd-106">Attributes and elements</span></span>

<span data-ttu-id="cf4bd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf4bd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf4bd-108">Attributes</span></span>

<span data-ttu-id="cf4bd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf4bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf4bd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf4bd-110">Child elements</span></span>

<span data-ttu-id="cf4bd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf4bd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf4bd-112">Parent elements</span></span>

|<span data-ttu-id="cf4bd-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf4bd-113">**Element**</span></span>|<span data-ttu-id="cf4bd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf4bd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf4bd-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="cf4bd-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="cf4bd-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf4bd-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cf4bd-117">Text value</span></span>

<span data-ttu-id="cf4bd-118">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-118">This property is read-only.</span></span> <span data-ttu-id="cf4bd-119">A tabela a seguir lista os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="cf4bd-120">**Valor**</span><span class="sxs-lookup"><span data-stu-id="cf4bd-120">**Value**</span></span>|<span data-ttu-id="cf4bd-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf4bd-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cf4bd-122">,0</span><span class="sxs-lookup"><span data-stu-id="cf4bd-122">0</span></span>  <br/> |<span data-ttu-id="cf4bd-123">O padrão para todos os itens de tarefa.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="cf4bd-124">1 </span><span class="sxs-lookup"><span data-stu-id="cf4bd-124">1</span></span>  <br/> |<span data-ttu-id="cf4bd-125">Uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="cf4bd-126">duas</span><span class="sxs-lookup"><span data-stu-id="cf4bd-126">2</span></span>  <br/> |<span data-ttu-id="cf4bd-127">Uma aceitação de tarefa de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="cf4bd-128">3D</span><span class="sxs-lookup"><span data-stu-id="cf4bd-128">3</span></span>  <br/> |<span data-ttu-id="cf4bd-129">Um declínio de tarefa de um destinatário de uma solicitação de tarefa.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="cf4bd-130">4 </span><span class="sxs-lookup"><span data-stu-id="cf4bd-130">4</span></span>  <br/> |<span data-ttu-id="cf4bd-131">Uma atualização para uma solicitação de tarefa anterior.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="cf4bd-132">5 </span><span class="sxs-lookup"><span data-stu-id="cf4bd-132">5</span></span>  <br/> |<span data-ttu-id="cf4bd-133">Não usado.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf4bd-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf4bd-134">Remarks</span></span>

<span data-ttu-id="cf4bd-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cf4bd-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf4bd-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cf4bd-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf4bd-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf4bd-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf4bd-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf4bd-138">Schema Name</span></span>  <br/> |<span data-ttu-id="cf4bd-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cf4bd-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf4bd-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf4bd-140">Validation File</span></span>  <br/> |<span data-ttu-id="cf4bd-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cf4bd-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf4bd-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf4bd-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf4bd-143">False</span><span class="sxs-lookup"><span data-stu-id="cf4bd-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf4bd-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="cf4bd-144">See also</span></span>



- [<span data-ttu-id="cf4bd-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cf4bd-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

