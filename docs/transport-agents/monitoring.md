---
title: monitoramento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455825"
---
# <a name="monitoring"></a><span data-ttu-id="0a40a-103">monitoramento</span><span class="sxs-lookup"><span data-stu-id="0a40a-103">monitoring</span></span>
  
<span data-ttu-id="0a40a-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0a40a-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0a40a-105">O elemento **Monitoring** contém informações de configuração que definem como e quando o serviço de transporte de front-end ou o serviço de transporte monitora os agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="0a40a-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="0a40a-106">configuration</span><span class="sxs-lookup"><span data-stu-id="0a40a-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="0a40a-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="0a40a-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="0a40a-108">monitoramento</span><span class="sxs-lookup"><span data-stu-id="0a40a-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="0a40a-109">**monitortype (complexType)**</span><span class="sxs-lookup"><span data-stu-id="0a40a-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0a40a-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0a40a-110">Attributes and elements</span></span>

<span data-ttu-id="0a40a-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0a40a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a40a-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="0a40a-112">Attributes</span></span>

<span data-ttu-id="0a40a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a40a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a40a-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0a40a-114">Child elements</span></span>

|<span data-ttu-id="0a40a-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a40a-115">**Element**</span></span>|<span data-ttu-id="0a40a-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a40a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a40a-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="0a40a-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="0a40a-118">Define o tempo, em milissegundos, para o acesso do cliente ou o servidor de caixa de correio para aguardar que um agente retorne de um evento antes de gravar no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="0a40a-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="0a40a-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="0a40a-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="0a40a-120">Contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0a40a-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a40a-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0a40a-121">Parent elements</span></span>

|<span data-ttu-id="0a40a-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a40a-122">**Element**</span></span>|<span data-ttu-id="0a40a-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a40a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a40a-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="0a40a-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="0a40a-125">Contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração para SMTP e agentes de roteamento instalados.</span><span class="sxs-lookup"><span data-stu-id="0a40a-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0a40a-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0a40a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a40a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a40a-127">Namespace</span></span>  <br/> |<span data-ttu-id="0a40a-128">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="0a40a-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="0a40a-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0a40a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0a40a-130">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="0a40a-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="0a40a-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0a40a-131">Validation File</span></span>  <br/> |<span data-ttu-id="0a40a-132">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="0a40a-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="0a40a-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0a40a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a40a-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="0a40a-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a40a-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0a40a-135">See also</span></span>

- [<span data-ttu-id="0a40a-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0a40a-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

