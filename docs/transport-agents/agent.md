---
title: Agente
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455678"
---
# <a name="agent"></a><span data-ttu-id="4fe90-103">Agente</span><span class="sxs-lookup"><span data-stu-id="4fe90-103">agent</span></span>
  
<span data-ttu-id="4fe90-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4fe90-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="4fe90-105">O elemento **Agent** contém informações de configuração sobre um agente instalado.</span><span class="sxs-lookup"><span data-stu-id="4fe90-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="4fe90-106">configuration</span><span class="sxs-lookup"><span data-stu-id="4fe90-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="4fe90-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="4fe90-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="4fe90-108">agentlist</span><span class="sxs-lookup"><span data-stu-id="4fe90-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="4fe90-109">Agente</span><span class="sxs-lookup"><span data-stu-id="4fe90-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="4fe90-110">**AgentType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="4fe90-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4fe90-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4fe90-111">Attributes and elements</span></span>

<span data-ttu-id="4fe90-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4fe90-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe90-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="4fe90-113">Attributes</span></span>

|<span data-ttu-id="4fe90-114">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="4fe90-114">**Attribute**</span></span>|<span data-ttu-id="4fe90-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fe90-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4fe90-116">**name**</span><span class="sxs-lookup"><span data-stu-id="4fe90-116">**name**</span></span> <br/> |<span data-ttu-id="4fe90-117">O nome que foi especificado quando o agente foi instalado.</span><span class="sxs-lookup"><span data-stu-id="4fe90-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="4fe90-118">Este atributo requer um valor de cadeia de caracteres não vazio que contenha um máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4fe90-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="4fe90-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="4fe90-119">**baseType**</span></span> <br/> |<span data-ttu-id="4fe90-120">O nome completo, incluindo o namespace, da classe a partir da qual o agente deriva.</span><span class="sxs-lookup"><span data-stu-id="4fe90-120">The full name, including the namespace, of the class from which the agent derives.</span></span> <span data-ttu-id="4fe90-121">Este atributo requer um valor de cadeia de caracteres não vazio que contenha pelo menos um caractere.</span><span class="sxs-lookup"><span data-stu-id="4fe90-121">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="4fe90-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="4fe90-122">**classFactory**</span></span> <br/> |<span data-ttu-id="4fe90-123">O nome completo, incluindo o namespace, da classe que implementa o alocador de agentes que cria instâncias do agente.</span><span class="sxs-lookup"><span data-stu-id="4fe90-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="4fe90-124">Este atributo deve conter o nome totalmente qualificado da classe que implementa o alocador de agentes que cria instâncias do agente.</span><span class="sxs-lookup"><span data-stu-id="4fe90-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="4fe90-125">Essa classe deve ser derivada da classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4fe90-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="4fe90-126">**assemblyPath**</span><span class="sxs-lookup"><span data-stu-id="4fe90-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="4fe90-127">O caminho totalmente qualificado, incluindo o nome do arquivo, do assembly que contém o código para o agente.</span><span class="sxs-lookup"><span data-stu-id="4fe90-127">The fully qualified path, including the file name, of the assembly that contains the code for the agent.</span></span> <span data-ttu-id="4fe90-128">Este atributo requer um valor de cadeia de caracteres não vazio que contenha pelo menos um caractere.</span><span class="sxs-lookup"><span data-stu-id="4fe90-128">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="4fe90-129">**enabled**</span><span class="sxs-lookup"><span data-stu-id="4fe90-129">**enabled**</span></span> <br/> |<span data-ttu-id="4fe90-130">Um valor Boolean que indica se o agente está habilitado.</span><span class="sxs-lookup"><span data-stu-id="4fe90-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="4fe90-131">O valor será **true** se o agente estiver habilitado; caso contrário, o valor será **false**.</span><span class="sxs-lookup"><span data-stu-id="4fe90-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="4fe90-132">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="4fe90-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4fe90-133">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4fe90-133">Child elements</span></span>

<span data-ttu-id="4fe90-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4fe90-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fe90-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4fe90-135">Parent elements</span></span>

|<span data-ttu-id="4fe90-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4fe90-136">**Element**</span></span>|<span data-ttu-id="4fe90-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4fe90-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe90-138">agentlist</span><span class="sxs-lookup"><span data-stu-id="4fe90-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="4fe90-139">Contém um elemento **Agent** para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="4fe90-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4fe90-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4fe90-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe90-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="4fe90-141">Namespace</span></span>  <br/> |<span data-ttu-id="4fe90-142">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="4fe90-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="4fe90-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4fe90-143">Schema Name</span></span>  <br/> |<span data-ttu-id="4fe90-144">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="4fe90-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="4fe90-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4fe90-145">Validation File</span></span>  <br/> |<span data-ttu-id="4fe90-146">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="4fe90-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="4fe90-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4fe90-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="4fe90-148">Falso.</span><span class="sxs-lookup"><span data-stu-id="4fe90-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fe90-149">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4fe90-149">See also</span></span>

- [<span data-ttu-id="4fe90-150">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4fe90-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

