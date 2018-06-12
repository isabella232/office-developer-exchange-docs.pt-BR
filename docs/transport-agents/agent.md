---
title: agente
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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750996"
---
# <a name="agent"></a><span data-ttu-id="c8192-103">agente</span><span class="sxs-lookup"><span data-stu-id="c8192-103">agent</span></span>
  
<span data-ttu-id="c8192-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c8192-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="c8192-105">O elemento de **agente** contém informações de configuração sobre um agente instalado.</span><span class="sxs-lookup"><span data-stu-id="c8192-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="c8192-106">configuração</span><span class="sxs-lookup"><span data-stu-id="c8192-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="c8192-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="c8192-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="c8192-108">agentList</span><span class="sxs-lookup"><span data-stu-id="c8192-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="c8192-109">agente</span><span class="sxs-lookup"><span data-stu-id="c8192-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="c8192-110">**agentType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="c8192-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c8192-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c8192-111">Attributes and elements</span></span>

<span data-ttu-id="c8192-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8192-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8192-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8192-113">Attributes</span></span>

|<span data-ttu-id="c8192-114">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="c8192-114">**Attribute**</span></span>|<span data-ttu-id="c8192-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8192-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c8192-116">**name**</span><span class="sxs-lookup"><span data-stu-id="c8192-116">**name**</span></span> <br/> |<span data-ttu-id="c8192-117">O nome que foi especificado quando o agente foi instalado.</span><span class="sxs-lookup"><span data-stu-id="c8192-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="c8192-118">Este atributo requer um valor de cadeia de caracteres vazia que contém um máximo de 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="c8192-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="c8192-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="c8192-119">**baseType**</span></span> <br/> |<span data-ttu-id="c8192-120">O nome completo, incluindo o namespace, da classe do qual o agente deriva.</span><span class="sxs-lookup"><span data-stu-id="c8192-120">The full name, including the namespace, of the class from which the agent derives.</span></span> <span data-ttu-id="c8192-121">Este atributo requer um valor de cadeia de caracteres vazia que contém pelo menos um caractere.</span><span class="sxs-lookup"><span data-stu-id="c8192-121">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="c8192-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="c8192-122">**classFactory**</span></span> <br/> |<span data-ttu-id="c8192-123">O nome completo, incluindo o namespace, da classe que implementa o alocador de agente que cria instâncias do agente.</span><span class="sxs-lookup"><span data-stu-id="c8192-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="c8192-124">Este atributo deve conter o nome totalmente qualificado da classe que implementa o alocador de agente que cria instâncias do agente.</span><span class="sxs-lookup"><span data-stu-id="c8192-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="c8192-125">Esta classe deve derivar de classe no [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c8192-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="c8192-126">**assemblyPath**</span><span class="sxs-lookup"><span data-stu-id="c8192-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="c8192-127">O caminho totalmente qualificado, incluindo o nome do arquivo do assembly que contém o código para o agente.</span><span class="sxs-lookup"><span data-stu-id="c8192-127">The fully qualified path, including the file name, of the assembly that contains the code for the agent.</span></span> <span data-ttu-id="c8192-128">Este atributo requer um valor de cadeia de caracteres vazia que contém pelo menos um caractere.</span><span class="sxs-lookup"><span data-stu-id="c8192-128">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="c8192-129">**habilitado**</span><span class="sxs-lookup"><span data-stu-id="c8192-129">**enabled**</span></span> <br/> |<span data-ttu-id="c8192-130">Um valor Boolean que indica se o agente está habilitado.</span><span class="sxs-lookup"><span data-stu-id="c8192-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="c8192-131">O valor é **true** se o agente estiver habilitado; Caso contrário, o valor é **false**.</span><span class="sxs-lookup"><span data-stu-id="c8192-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="c8192-132">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="c8192-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c8192-133">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8192-133">Child elements</span></span>

<span data-ttu-id="c8192-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8192-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8192-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8192-135">Parent elements</span></span>

|<span data-ttu-id="c8192-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8192-136">**Element**</span></span>|<span data-ttu-id="c8192-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8192-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8192-138">agentList</span><span class="sxs-lookup"><span data-stu-id="c8192-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="c8192-139">Contém um elemento de **agente** para cada agente instalado.</span><span class="sxs-lookup"><span data-stu-id="c8192-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c8192-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c8192-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8192-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8192-141">Namespace</span></span>  <br/> |<span data-ttu-id="c8192-142">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="c8192-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="c8192-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c8192-143">Schema Name</span></span>  <br/> |<span data-ttu-id="c8192-144">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="c8192-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="c8192-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c8192-145">Validation File</span></span>  <br/> |<span data-ttu-id="c8192-146">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="c8192-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="c8192-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c8192-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8192-148">Falso.</span><span class="sxs-lookup"><span data-stu-id="c8192-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8192-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="c8192-149">See also</span></span>

- [<span data-ttu-id="c8192-150">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="c8192-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

