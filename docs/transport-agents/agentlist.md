---
title: agentList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750995"
---
# <a name="agentlist"></a><span data-ttu-id="edbc8-103">agentList</span><span class="sxs-lookup"><span data-stu-id="edbc8-103">agentList</span></span>
  
<span data-ttu-id="edbc8-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="edbc8-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="edbc8-105">O elemento **agentList** contém um elemento de [agente](agent.md) para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="edbc8-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="edbc8-106">configuração</span><span class="sxs-lookup"><span data-stu-id="edbc8-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="edbc8-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="edbc8-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="edbc8-108">agentList</span><span class="sxs-lookup"><span data-stu-id="edbc8-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="edbc8-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="edbc8-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="edbc8-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="edbc8-110">Attributes and elements</span></span>

<span data-ttu-id="edbc8-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="edbc8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edbc8-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="edbc8-112">Attributes</span></span>

<span data-ttu-id="edbc8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="edbc8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edbc8-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="edbc8-114">Child elements</span></span>

|<span data-ttu-id="edbc8-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="edbc8-115">**Element**</span></span>|<span data-ttu-id="edbc8-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edbc8-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edbc8-117">agente</span><span class="sxs-lookup"><span data-stu-id="edbc8-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="edbc8-118">Contém informações de configuração sobre um agente instalado.</span><span class="sxs-lookup"><span data-stu-id="edbc8-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="edbc8-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="edbc8-119">Parent elements</span></span>

|<span data-ttu-id="edbc8-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="edbc8-120">**Element**</span></span>|<span data-ttu-id="edbc8-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edbc8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edbc8-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="edbc8-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="edbc8-123">Contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração sobre agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="edbc8-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="edbc8-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="edbc8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edbc8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="edbc8-125">Namespace</span></span>  <br/> |<span data-ttu-id="edbc8-126">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="edbc8-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="edbc8-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="edbc8-127">Schema Name</span></span>  <br/> |<span data-ttu-id="edbc8-128">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="edbc8-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="edbc8-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="edbc8-129">Validation File</span></span>  <br/> |<span data-ttu-id="edbc8-130">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="edbc8-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="edbc8-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="edbc8-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="edbc8-132">Falso.</span><span class="sxs-lookup"><span data-stu-id="edbc8-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edbc8-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="edbc8-133">See also</span></span>

- [<span data-ttu-id="edbc8-134">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="edbc8-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

