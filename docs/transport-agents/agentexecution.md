---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446487"
---
# <a name="agentexecution"></a><span data-ttu-id="4e373-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="4e373-103">agentExecution</span></span>
  
<span data-ttu-id="4e373-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4e373-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="4e373-105">O elemento **agentExecution** define o tempo, em milissegundos, para o servidor de acesso para cliente ou caixa de correio aguardar que um agente retorne de um evento antes de gravar no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="4e373-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="4e373-106">configuration</span><span class="sxs-lookup"><span data-stu-id="4e373-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="4e373-107">monitoramento</span><span class="sxs-lookup"><span data-stu-id="4e373-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="4e373-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="4e373-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="4e373-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="4e373-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4e373-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4e373-110">Attributes and elements</span></span>

<span data-ttu-id="4e373-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4e373-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e373-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="4e373-112">Attributes</span></span>

|<span data-ttu-id="4e373-113">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="4e373-113">**Attribute**</span></span>|<span data-ttu-id="4e373-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4e373-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e373-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="4e373-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="4e373-116">Um valor inteiro positivo que especifica o tempo, em milissegundos, para que o servidor aguarde um agente retornar de um evento antes de gravar um aviso no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="4e373-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="4e373-117">O desempenho pode diminuir se esse valor for muito pequeno.</span><span class="sxs-lookup"><span data-stu-id="4e373-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="4e373-118">O valor sugerido para este atributo é 300.000, que é igual a 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="4e373-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4e373-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4e373-119">Child elements</span></span>

<span data-ttu-id="4e373-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4e373-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e373-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4e373-121">Parent elements</span></span>

|<span data-ttu-id="4e373-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4e373-122">**Element**</span></span>|<span data-ttu-id="4e373-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4e373-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e373-124">monitoramento</span><span class="sxs-lookup"><span data-stu-id="4e373-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="4e373-125">Contém informações de configuração que definem como e quando o serviço de transporte de front-end ou o serviço de transporte monitora agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="4e373-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4e373-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4e373-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e373-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="4e373-127">Namespace</span></span>  <br/> |<span data-ttu-id="4e373-128">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="4e373-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="4e373-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4e373-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4e373-130">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="4e373-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="4e373-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4e373-131">Validation File</span></span>  <br/> |<span data-ttu-id="4e373-132">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="4e373-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="4e373-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4e373-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e373-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="4e373-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e373-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4e373-135">See also</span></span>

- [<span data-ttu-id="4e373-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4e373-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

