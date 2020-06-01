---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: 'Última modificação: 17 de setembro de 2015'
ms.openlocfilehash: 8a58444580c803efb7312df95d75d697bc42e8e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461839"
---
# <a name="messagesnapshot"></a><span data-ttu-id="987a9-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="987a9-103">messageSnapshot</span></span>

<span data-ttu-id="987a9-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="987a9-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="987a9-105">O elemento **messageSnapshot** contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o servidor Exchange que tem a função de servidor de acesso para cliente ou caixa de Correio instalada.</span><span class="sxs-lookup"><span data-stu-id="987a9-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="987a9-106">configuration</span><span class="sxs-lookup"><span data-stu-id="987a9-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="987a9-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="987a9-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="987a9-108">monitoramento</span><span class="sxs-lookup"><span data-stu-id="987a9-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="987a9-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="987a9-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="987a9-110">**messageSnapshotType (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="987a9-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="987a9-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="987a9-111">Attributes and elements</span></span>

<span data-ttu-id="987a9-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="987a9-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="987a9-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="987a9-113">Attributes</span></span>

|<span data-ttu-id="987a9-114">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="987a9-114">**Attribute**</span></span>|<span data-ttu-id="987a9-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="987a9-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="987a9-116">**enabled**</span><span class="sxs-lookup"><span data-stu-id="987a9-116">**enabled**</span></span> <br/> |<span data-ttu-id="987a9-117">Um valor Boolean que indica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="987a9-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="987a9-118">O valor é **true** se o rastreamento de pipeline estiver habilitado; caso contrário, o valor será **false** ou o elemento não estará presente.</span><span class="sxs-lookup"><span data-stu-id="987a9-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="987a9-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="987a9-119">Child elements</span></span>

<span data-ttu-id="987a9-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="987a9-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="987a9-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="987a9-121">Parent elements</span></span>

|<span data-ttu-id="987a9-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="987a9-122">**Element**</span></span>|<span data-ttu-id="987a9-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="987a9-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="987a9-124">monitoramento</span><span class="sxs-lookup"><span data-stu-id="987a9-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="987a9-125">Contém informações de configuração que definem como e quando o serviço de transporte monitora os agentes instalados.</span><span class="sxs-lookup"><span data-stu-id="987a9-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="987a9-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="987a9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="987a9-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="987a9-127">Namespace</span></span>  <br/> |<span data-ttu-id="987a9-128">Este arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="987a9-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="987a9-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="987a9-129">Schema Name</span></span>  <br/> |<span data-ttu-id="987a9-130">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="987a9-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="987a9-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="987a9-131">Validation File</span></span>  <br/> |<span data-ttu-id="987a9-132">Indisponível.</span><span class="sxs-lookup"><span data-stu-id="987a9-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="987a9-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="987a9-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="987a9-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="987a9-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="987a9-135">Também consulte</span><span class="sxs-lookup"><span data-stu-id="987a9-135">See also</span></span>

- [<span data-ttu-id="987a9-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="987a9-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

