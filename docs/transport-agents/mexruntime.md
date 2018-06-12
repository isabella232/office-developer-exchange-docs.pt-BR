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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751027"
---
# <a name="mexruntime"></a><span data-ttu-id="64fd0-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="64fd0-103">mexRuntime</span></span>
  
<span data-ttu-id="64fd0-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="64fd0-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="64fd0-105">O elemento **mexRuntime** contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração de SMTP e os agentes de roteamento que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="64fd0-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="64fd0-106">configuração</span><span class="sxs-lookup"><span data-stu-id="64fd0-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="64fd0-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="64fd0-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="64fd0-108">**mexRuntimeType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="64fd0-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="64fd0-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="64fd0-109">Attributes and elements</span></span>

<span data-ttu-id="64fd0-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="64fd0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64fd0-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="64fd0-111">Attributes</span></span>

<span data-ttu-id="64fd0-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="64fd0-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64fd0-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="64fd0-113">Child elements</span></span>

|<span data-ttu-id="64fd0-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64fd0-114">**Element**</span></span>|<span data-ttu-id="64fd0-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64fd0-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64fd0-116">monitoramento</span><span class="sxs-lookup"><span data-stu-id="64fd0-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="64fd0-117">Contém informações de configuração que define como e quando o transporte monitora os operadores que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="64fd0-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="64fd0-118">agentList</span><span class="sxs-lookup"><span data-stu-id="64fd0-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="64fd0-119">Contém um elemento de [agente](agent.md) para cada agente que está instalado.</span><span class="sxs-lookup"><span data-stu-id="64fd0-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64fd0-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="64fd0-120">Parent elements</span></span>

|<span data-ttu-id="64fd0-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64fd0-121">**Element**</span></span>|<span data-ttu-id="64fd0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64fd0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64fd0-123">configuração</span><span class="sxs-lookup"><span data-stu-id="64fd0-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="64fd0-124">O elemento raiz para o arquivo de configuração de agentes.</span><span class="sxs-lookup"><span data-stu-id="64fd0-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="64fd0-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="64fd0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64fd0-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="64fd0-126">Namespace</span></span>  <br/> |<span data-ttu-id="64fd0-127">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="64fd0-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="64fd0-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="64fd0-128">Schema Name</span></span>  <br/> |<span data-ttu-id="64fd0-129">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="64fd0-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="64fd0-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="64fd0-130">Validation File</span></span>  <br/> |<span data-ttu-id="64fd0-131">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="64fd0-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="64fd0-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="64fd0-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="64fd0-133">Falso.</span><span class="sxs-lookup"><span data-stu-id="64fd0-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64fd0-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="64fd0-134">See also</span></span>

- [<span data-ttu-id="64fd0-135">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="64fd0-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

