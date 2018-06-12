---
title: configuration
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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750997"
---
# <a name="configuration"></a><span data-ttu-id="9cf29-103">configuration</span><span class="sxs-lookup"><span data-stu-id="9cf29-103">configuration</span></span>
  
<span data-ttu-id="9cf29-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9cf29-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="9cf29-105">O elemento de **configuração** é o elemento raiz para o arquivo de configuração de agentes.</span><span class="sxs-lookup"><span data-stu-id="9cf29-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="9cf29-106">configuração</span><span class="sxs-lookup"><span data-stu-id="9cf29-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="9cf29-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="9cf29-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="9cf29-108">**configurationType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="9cf29-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9cf29-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9cf29-109">Attributes and elements</span></span>

<span data-ttu-id="9cf29-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9cf29-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cf29-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="9cf29-111">Attributes</span></span>

<span data-ttu-id="9cf29-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9cf29-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cf29-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9cf29-113">Child elements</span></span>

|<span data-ttu-id="9cf29-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9cf29-114">**Element**</span></span>|<span data-ttu-id="9cf29-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9cf29-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cf29-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="9cf29-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="9cf29-117">Contém os elementos que definem as informações de configuração de monitoramento de agente e informações de configuração de SMTP e os agentes de roteamento que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="9cf29-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9cf29-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9cf29-118">Parent elements</span></span>

<span data-ttu-id="9cf29-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9cf29-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cf29-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9cf29-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cf29-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="9cf29-121">Namespace</span></span>  <br/> |<span data-ttu-id="9cf29-122">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="9cf29-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="9cf29-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9cf29-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9cf29-124">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="9cf29-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="9cf29-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9cf29-125">Validation File</span></span>  <br/> |<span data-ttu-id="9cf29-126">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="9cf29-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="9cf29-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9cf29-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cf29-128">Falso.</span><span class="sxs-lookup"><span data-stu-id="9cf29-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cf29-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9cf29-129">See also</span></span>

- [<span data-ttu-id="9cf29-130">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9cf29-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

