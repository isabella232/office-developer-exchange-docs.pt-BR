---
title: IsTeamTask
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsTeamTask
api_type:
- schema
ms.assetid: af0095da-e5bb-4138-a01c-c203f1a5a33f
description: O elemento IsTeamTask indica se a tarefa pertence a uma equipe.
ms.openlocfilehash: 27b5efbac028dbe7cf5858b198e3a33f9f6cdc86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468443"
---
# <a name="isteamtask"></a><span data-ttu-id="85899-103">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="85899-103">IsTeamTask</span></span>

<span data-ttu-id="85899-104">O elemento **IsTeamTask** indica se a tarefa pertence a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="85899-104">The **IsTeamTask** element indicates whether the task is owned by a team.</span></span> 
  
```xml
<IsTeamTask/>
```

 <span data-ttu-id="85899-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="85899-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85899-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="85899-106">Attributes and elements</span></span>

<span data-ttu-id="85899-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="85899-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85899-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="85899-108">Attributes</span></span>

<span data-ttu-id="85899-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85899-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85899-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="85899-110">Child elements</span></span>

<span data-ttu-id="85899-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85899-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85899-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="85899-112">Parent elements</span></span>

|<span data-ttu-id="85899-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="85899-113">**Element**</span></span>|<span data-ttu-id="85899-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="85899-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85899-115">Tarefa</span><span class="sxs-lookup"><span data-stu-id="85899-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="85899-116">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="85899-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85899-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="85899-117">Text value</span></span>

<span data-ttu-id="85899-118">O valor de texto representa um valor booliano que indica se uma tarefa pertence a uma equipe.</span><span class="sxs-lookup"><span data-stu-id="85899-118">The text value represents a Boolean value that indicates whether a task is owned by a team.</span></span> <span data-ttu-id="85899-119">Esta é uma propriedade somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85899-119">This is a read-only property.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85899-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="85899-120">Remarks</span></span>

<span data-ttu-id="85899-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="85899-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85899-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="85899-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85899-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="85899-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85899-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="85899-124">Schema Name</span></span>  <br/> |<span data-ttu-id="85899-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="85899-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="85899-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="85899-126">Validation File</span></span>  <br/> |<span data-ttu-id="85899-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="85899-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85899-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="85899-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="85899-129">False</span><span class="sxs-lookup"><span data-stu-id="85899-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85899-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="85899-130">See also</span></span>



- [<span data-ttu-id="85899-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="85899-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="85899-132">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="85899-132">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="85899-133">Excluir tarefas</span><span class="sxs-lookup"><span data-stu-id="85899-133">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

