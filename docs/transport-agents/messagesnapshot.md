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
description: 'Modificado pela última vez: 17 de setembro de 2015'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751024"
---
# <a name="messagesnapshot"></a><span data-ttu-id="97aac-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="97aac-103">messageSnapshot</span></span>

<span data-ttu-id="97aac-104">**Aplica-se a:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="97aac-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="97aac-105">O elemento **messageSnapshot** contém um atributo que especifica se o recurso de rastreamento de pipeline está habilitado para o servidor do Exchange que tem o acesso para cliente ou a função de servidor de caixa de correio instalada.</span><span class="sxs-lookup"><span data-stu-id="97aac-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="97aac-106">configuração</span><span class="sxs-lookup"><span data-stu-id="97aac-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="97aac-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="97aac-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="97aac-108">monitoramento</span><span class="sxs-lookup"><span data-stu-id="97aac-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="97aac-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="97aac-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="97aac-110">**messageSnapshotType (booleano)**</span><span class="sxs-lookup"><span data-stu-id="97aac-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="97aac-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="97aac-111">Attributes and elements</span></span>

<span data-ttu-id="97aac-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97aac-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97aac-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="97aac-113">Attributes</span></span>

|<span data-ttu-id="97aac-114">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="97aac-114">**Attribute**</span></span>|<span data-ttu-id="97aac-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97aac-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97aac-116">**habilitado**</span><span class="sxs-lookup"><span data-stu-id="97aac-116">**enabled**</span></span> <br/> |<span data-ttu-id="97aac-117">Um valor Boolean que indica se o recurso de rastreamento de pipeline está habilitado para o acesso do cliente ou o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="97aac-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="97aac-118">O valor é **true** se o rastreamento de pipeline estiver habilitado; Caso contrário, o valor é **false** , ou o elemento não está presente.</span><span class="sxs-lookup"><span data-stu-id="97aac-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97aac-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97aac-119">Child elements</span></span>

<span data-ttu-id="97aac-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="97aac-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="97aac-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97aac-121">Parent elements</span></span>

|<span data-ttu-id="97aac-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97aac-122">**Element**</span></span>|<span data-ttu-id="97aac-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97aac-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97aac-124">monitoramento</span><span class="sxs-lookup"><span data-stu-id="97aac-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="97aac-125">Contém informações de configuração que define como e quando o serviço de transporte monitora os operadores que estão instalados.</span><span class="sxs-lookup"><span data-stu-id="97aac-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="97aac-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="97aac-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97aac-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="97aac-127">Namespace</span></span>  <br/> |<span data-ttu-id="97aac-128">Esse arquivo não define um namespace.</span><span class="sxs-lookup"><span data-stu-id="97aac-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="97aac-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97aac-129">Schema Name</span></span>  <br/> |<span data-ttu-id="97aac-130">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="97aac-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="97aac-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97aac-131">Validation File</span></span>  <br/> |<span data-ttu-id="97aac-132">Não disponível.</span><span class="sxs-lookup"><span data-stu-id="97aac-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="97aac-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="97aac-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="97aac-134">Falso.</span><span class="sxs-lookup"><span data-stu-id="97aac-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97aac-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="97aac-135">See also</span></span>

- [<span data-ttu-id="97aac-136">Elementos de arquivo de configuração de agentes para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="97aac-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

