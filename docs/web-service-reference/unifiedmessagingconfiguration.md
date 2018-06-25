---
title: UnifiedMessagingConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: O elemento UnifiedMessagingConfiguration contém informações de configuração de serviço para o serviço de Unificação de mensagens.
ms.openlocfilehash: 3ad8f66ecdf21062c00c2a6ac6f65fac875da38c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837829"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="5e3d1-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e3d1-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="5e3d1-104">O elemento **UnifiedMessagingConfiguration** contém informações de configuração de serviço para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="5e3d1-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="5e3d1-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e3d1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5e3d1-106">Attributes and elements</span></span>

<span data-ttu-id="5e3d1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e3d1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5e3d1-108">Attributes</span></span>

<span data-ttu-id="5e3d1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e3d1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5e3d1-110">Child elements</span></span>

|<span data-ttu-id="5e3d1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e3d1-111">**Element**</span></span>|<span data-ttu-id="5e3d1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e3d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e3d1-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="5e3d1-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="5e3d1-114">Indica se a Unificação de mensagens está habilitada para uma conta.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="5e3d1-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5e3d1-116">PlayOnPhoneDialString (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="5e3d1-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="5e3d1-117">Identifica a cadeia de caracteres de discagem de tocar no telefone.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="5e3d1-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5e3d1-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="5e3d1-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="5e3d1-120">Indica se o recurso Tocar no telefone está habilitado.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="5e3d1-121">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e3d1-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5e3d1-122">Parent elements</span></span>

|<span data-ttu-id="5e3d1-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e3d1-123">**Element**</span></span>|<span data-ttu-id="5e3d1-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e3d1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e3d1-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="5e3d1-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="5e3d1-126">Contém as definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5e3d1-127">Text value</span><span class="sxs-lookup"><span data-stu-id="5e3d1-127">Text value</span></span>

<span data-ttu-id="5e3d1-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5e3d1-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="5e3d1-129">Remarks</span></span>

<span data-ttu-id="5e3d1-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e3d1-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e3d1-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5e3d1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e3d1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e3d1-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5e3d1-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5e3d1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5e3d1-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5e3d1-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5e3d1-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5e3d1-135">Validation File</span></span>  <br/> |<span data-ttu-id="5e3d1-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5e3d1-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5e3d1-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5e3d1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e3d1-138">False</span><span class="sxs-lookup"><span data-stu-id="5e3d1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e3d1-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="5e3d1-139">See also</span></span>



- [<span data-ttu-id="5e3d1-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5e3d1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

