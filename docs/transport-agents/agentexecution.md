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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750993"
---
# <a name="agentexecution"></a><span data-ttu-id="96545-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="96545-103">agentExecution</span></span>
  
<span data-ttu-id="96545-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="96545-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="96545-105">O elemento de **agentExecution** define o tempo, em milissegundos, para o servidor de acesso para cliente ou caixa de correio aguardar um operador retornar a partir de um evento antes que ela foi gravada no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="96545-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="96545-106">configuração</span><span class="sxs-lookup"><span data-stu-id="96545-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="96545-107">monitoramento</span><span class="sxs-lookup"><span data-stu-id="96545-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="96545-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="96545-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="96545-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="96545-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="96545-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="96545-110">Attributes and elements</span></span>

<span data-ttu-id="96545-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96545-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96545-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="96545-112">Attributes</span></span>

|<span data-ttu-id="96545-113">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="96545-113">**Attribute**</span></span>|<span data-ttu-id="96545-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96545-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96545-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="96545-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="96545-116">Um valor de número inteiro positivo que especifica o tempo, em milissegundos, para o servidor deverá esperar um operador retornar a partir de um evento antes que ele grava um aviso no log de eventos.</span><span class="sxs-lookup"><span data-stu-id="96545-116">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log.</span></span> <span data-ttu-id="96545-117">O desempenho pode diminuir se esse valor é muito pequeno.</span><span class="sxs-lookup"><span data-stu-id="96545-117">Performance can decrease if this value is too small.</span></span> <span data-ttu-id="96545-118">O valor sugerido para este atributo é 300.000, que é igual a 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="96545-118">The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="96545-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96545-119">Child elements</span></span>

<span data-ttu-id="96545-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96545-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96545-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96545-121">Parent elements</span></span>

|<span data-ttu-id="96545-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96545-122">**Element**</span></span>|<span data-ttu-id="96545-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96545-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96545-124">monitoramento</span><span class="sxs-lookup"><span data-stu-id="96545-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="96545-125">Contém informações de configuração que define como e quando o serviço Front End Transport ou o serviço de transporte monitora os operadores que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="96545-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="96545-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="96545-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96545-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="96545-127">Namespace</span></span>  <br/> |<span data-ttu-id="96545-128">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="96545-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="96545-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96545-129">Schema Name</span></span>  <br/> |<span data-ttu-id="96545-130">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="96545-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="96545-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96545-131">Validation File</span></span>  <br/> |<span data-ttu-id="96545-132">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="96545-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="96545-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96545-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="96545-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="96545-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96545-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="96545-135">See also</span></span>

- [<span data-ttu-id="96545-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="96545-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

