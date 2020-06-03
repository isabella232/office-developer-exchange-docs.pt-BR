---
title: Configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: b886851b9a0c17d58428f49281d664930d0e4070
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461559"
---
# <a name="configuration"></a><span data-ttu-id="8b61b-103">Configuration</span><span class="sxs-lookup"><span data-stu-id="8b61b-103">configuration</span></span>
  
<span data-ttu-id="8b61b-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="8b61b-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="8b61b-105">O elemento **Configuration** é o elemento raiz do arquivo de configuração dos agentes.</span><span class="sxs-lookup"><span data-stu-id="8b61b-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="8b61b-106">configuration</span><span class="sxs-lookup"><span data-stu-id="8b61b-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="8b61b-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="8b61b-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="8b61b-108">**ConfigurationType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="8b61b-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8b61b-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8b61b-109">Attributes and elements</span></span>

<span data-ttu-id="8b61b-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8b61b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b61b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="8b61b-111">Attributes</span></span>

<span data-ttu-id="8b61b-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b61b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b61b-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8b61b-113">Child elements</span></span>

|<span data-ttu-id="8b61b-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b61b-114">**Element**</span></span>|<span data-ttu-id="8b61b-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b61b-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b61b-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="8b61b-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="8b61b-117">Contém elementos que definem informações de configuração para o monitoramento de agentes e informações de configuração para SMTP e agentes de roteamento instalados.</span><span class="sxs-lookup"><span data-stu-id="8b61b-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b61b-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8b61b-118">Parent elements</span></span>

<span data-ttu-id="8b61b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b61b-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b61b-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8b61b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b61b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b61b-121">Namespace</span></span>  <br/> |<span data-ttu-id="8b61b-122">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="8b61b-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="8b61b-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8b61b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8b61b-124">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="8b61b-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="8b61b-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8b61b-125">Validation File</span></span>  <br/> |<span data-ttu-id="8b61b-126">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="8b61b-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="8b61b-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8b61b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b61b-128">Falso.</span><span class="sxs-lookup"><span data-stu-id="8b61b-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b61b-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="8b61b-129">See also</span></span>

- [<span data-ttu-id="8b61b-130">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8b61b-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

