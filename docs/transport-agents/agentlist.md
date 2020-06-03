---
title: agentlist
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
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446389"
---
# <a name="agentlist"></a><span data-ttu-id="188da-103">agentlist</span><span class="sxs-lookup"><span data-stu-id="188da-103">agentList</span></span>
  
<span data-ttu-id="188da-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="188da-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="188da-105">O elemento **agentlist** contém um elemento [Agent](agent.md) para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="188da-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="188da-106">configuration</span><span class="sxs-lookup"><span data-stu-id="188da-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="188da-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="188da-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="188da-108">agentlist</span><span class="sxs-lookup"><span data-stu-id="188da-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="188da-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="188da-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="188da-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="188da-110">Attributes and elements</span></span>

<span data-ttu-id="188da-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="188da-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="188da-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="188da-112">Attributes</span></span>

<span data-ttu-id="188da-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="188da-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="188da-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="188da-114">Child elements</span></span>

|<span data-ttu-id="188da-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="188da-115">**Element**</span></span>|<span data-ttu-id="188da-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="188da-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="188da-117">Agente</span><span class="sxs-lookup"><span data-stu-id="188da-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="188da-118">Contém informações de configuração sobre um agente instalado.</span><span class="sxs-lookup"><span data-stu-id="188da-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="188da-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="188da-119">Parent elements</span></span>

|<span data-ttu-id="188da-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="188da-120">**Element**</span></span>|<span data-ttu-id="188da-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="188da-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="188da-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="188da-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="188da-123">Contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração sobre agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="188da-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="188da-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="188da-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="188da-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="188da-125">Namespace</span></span>  <br/> |<span data-ttu-id="188da-126">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="188da-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="188da-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="188da-127">Schema Name</span></span>  <br/> |<span data-ttu-id="188da-128">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="188da-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="188da-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="188da-129">Validation File</span></span>  <br/> |<span data-ttu-id="188da-130">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="188da-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="188da-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="188da-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="188da-132">Falso.</span><span class="sxs-lookup"><span data-stu-id="188da-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="188da-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="188da-133">See also</span></span>

- [<span data-ttu-id="188da-134">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="188da-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

