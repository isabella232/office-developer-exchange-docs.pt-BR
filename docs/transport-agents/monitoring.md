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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 1b5484467def0bf3d22ba0707357977d5ed461ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751023"
---
# <a name="monitoring"></a><span data-ttu-id="9f5e0-103">monitoramento</span><span class="sxs-lookup"><span data-stu-id="9f5e0-103">monitoring</span></span>
  
<span data-ttu-id="9f5e0-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9f5e0-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="9f5e0-105">O elemento de **monitoramento** contém informações de configuração que definem como e quando o serviço de transporte de Front-End ou o serviço de transporte monitora os operadores que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="9f5e0-106">configuração</span><span class="sxs-lookup"><span data-stu-id="9f5e0-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="9f5e0-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="9f5e0-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="9f5e0-108">monitoramento</span><span class="sxs-lookup"><span data-stu-id="9f5e0-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="9f5e0-109">**monitoringType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="9f5e0-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f5e0-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9f5e0-110">Attributes and elements</span></span>

<span data-ttu-id="9f5e0-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f5e0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f5e0-112">Attributes</span></span>

<span data-ttu-id="9f5e0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f5e0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f5e0-114">Child elements</span></span>

|<span data-ttu-id="9f5e0-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f5e0-115">**Element**</span></span>|<span data-ttu-id="9f5e0-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f5e0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f5e0-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="9f5e0-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="9f5e0-118">Define o tempo, em milissegundos, para o acesso do cliente ou o servidor de caixa de correio aguardar um operador retornar a partir de um evento antes que ela foi gravada no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="9f5e0-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="9f5e0-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="9f5e0-120">Contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou no servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f5e0-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f5e0-121">Parent elements</span></span>

|<span data-ttu-id="9f5e0-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f5e0-122">**Element**</span></span>|<span data-ttu-id="9f5e0-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f5e0-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f5e0-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="9f5e0-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="9f5e0-125">Contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração de SMTP e os agentes de roteamento que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="9f5e0-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9f5e0-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f5e0-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f5e0-127">Namespace</span></span>  <br/> |<span data-ttu-id="9f5e0-128">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="9f5e0-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f5e0-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9f5e0-130">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="9f5e0-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f5e0-131">Validation File</span></span>  <br/> |<span data-ttu-id="9f5e0-132">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="9f5e0-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9f5e0-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f5e0-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="9f5e0-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f5e0-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="9f5e0-135">See also</span></span>

- [<span data-ttu-id="9f5e0-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9f5e0-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

