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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750995"
---
# <a name="agentlist"></a><span data-ttu-id="39d92-103">agentList</span><span class="sxs-lookup"><span data-stu-id="39d92-103">agentList</span></span>
  
<span data-ttu-id="39d92-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="39d92-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="39d92-105">O elemento **agentList** contém um elemento de [agente](agent.md) para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="39d92-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="39d92-106">configuração</span><span class="sxs-lookup"><span data-stu-id="39d92-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="39d92-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="39d92-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="39d92-108">agentList</span><span class="sxs-lookup"><span data-stu-id="39d92-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="39d92-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="39d92-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="39d92-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="39d92-110">Attributes and elements</span></span>

<span data-ttu-id="39d92-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="39d92-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39d92-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="39d92-112">Attributes</span></span>

<span data-ttu-id="39d92-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="39d92-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39d92-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="39d92-114">Child elements</span></span>

|<span data-ttu-id="39d92-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="39d92-115">**Element**</span></span>|<span data-ttu-id="39d92-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="39d92-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39d92-117">agente</span><span class="sxs-lookup"><span data-stu-id="39d92-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="39d92-118">Contém informações de configuração sobre um agente instalado.</span><span class="sxs-lookup"><span data-stu-id="39d92-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39d92-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="39d92-119">Parent elements</span></span>

|<span data-ttu-id="39d92-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="39d92-120">**Element**</span></span>|<span data-ttu-id="39d92-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="39d92-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39d92-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="39d92-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="39d92-123">Contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração sobre agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="39d92-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="39d92-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="39d92-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39d92-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="39d92-125">Namespace</span></span>  <br/> |<span data-ttu-id="39d92-126">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="39d92-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="39d92-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="39d92-127">Schema Name</span></span>  <br/> |<span data-ttu-id="39d92-128">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="39d92-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="39d92-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="39d92-129">Validation File</span></span>  <br/> |<span data-ttu-id="39d92-130">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="39d92-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="39d92-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="39d92-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="39d92-132">Falso.</span><span class="sxs-lookup"><span data-stu-id="39d92-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39d92-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="39d92-133">See also</span></span>

- [<span data-ttu-id="39d92-134">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="39d92-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

