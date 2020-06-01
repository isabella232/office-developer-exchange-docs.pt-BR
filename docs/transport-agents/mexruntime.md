---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461832"
---
# <a name="mexruntime"></a><span data-ttu-id="1d2f1-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="1d2f1-103">mexRuntime</span></span>
  
<span data-ttu-id="1d2f1-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="1d2f1-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="1d2f1-105">O elemento **mexRuntime** contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração para SMTP e agentes de roteamento instalados.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="1d2f1-106">configuration</span><span class="sxs-lookup"><span data-stu-id="1d2f1-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="1d2f1-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="1d2f1-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="1d2f1-108">**mexRuntimeType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="1d2f1-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1d2f1-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1d2f1-109">Attributes and elements</span></span>

<span data-ttu-id="1d2f1-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d2f1-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="1d2f1-111">Attributes</span></span>

<span data-ttu-id="1d2f1-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d2f1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d2f1-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1d2f1-113">Child elements</span></span>

|<span data-ttu-id="1d2f1-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1d2f1-114">**Element**</span></span>|<span data-ttu-id="1d2f1-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1d2f1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d2f1-116">monitoramento</span><span class="sxs-lookup"><span data-stu-id="1d2f1-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="1d2f1-117">Contém informações de configuração que definem como e quando o transporte monitora agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="1d2f1-118">agentlist</span><span class="sxs-lookup"><span data-stu-id="1d2f1-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="1d2f1-119">Contém um elemento [Agent](agent.md) para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d2f1-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1d2f1-120">Parent elements</span></span>

|<span data-ttu-id="1d2f1-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1d2f1-121">**Element**</span></span>|<span data-ttu-id="1d2f1-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1d2f1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d2f1-123">configuration</span><span class="sxs-lookup"><span data-stu-id="1d2f1-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="1d2f1-124">O elemento raiz para o arquivo de configuração dos agentes.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="1d2f1-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1d2f1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d2f1-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d2f1-126">Namespace</span></span>  <br/> |<span data-ttu-id="1d2f1-127">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="1d2f1-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1d2f1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1d2f1-129">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="1d2f1-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1d2f1-130">Validation File</span></span>  <br/> |<span data-ttu-id="1d2f1-131">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="1d2f1-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1d2f1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d2f1-133">Falso.</span><span class="sxs-lookup"><span data-stu-id="1d2f1-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d2f1-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="1d2f1-134">See also</span></span>

- [<span data-ttu-id="1d2f1-135">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="1d2f1-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

