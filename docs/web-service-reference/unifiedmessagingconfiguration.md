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
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528689"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="38875-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="38875-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="38875-104">O elemento **UnifiedMessagingConfiguration** contém informações de configuração de serviço para o serviço de Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="38875-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="38875-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="38875-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38875-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="38875-106">Attributes and elements</span></span>

<span data-ttu-id="38875-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38875-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38875-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="38875-108">Attributes</span></span>

<span data-ttu-id="38875-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38875-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38875-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38875-110">Child elements</span></span>

|<span data-ttu-id="38875-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38875-111">**Element**</span></span>|<span data-ttu-id="38875-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38875-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38875-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="38875-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="38875-114">Indica se a Unificação de mensagens está habilitada para uma conta.</span><span class="sxs-lookup"><span data-stu-id="38875-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="38875-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38875-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="38875-116">PlayOnPhoneDialString (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="38875-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="38875-117">Identifica a cadeia de caracteres de discagem de reprodução no telefone.</span><span class="sxs-lookup"><span data-stu-id="38875-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="38875-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38875-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="38875-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="38875-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="38875-120">Indica se o recurso de reproduzir no telefone está habilitado.</span><span class="sxs-lookup"><span data-stu-id="38875-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="38875-121">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38875-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38875-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38875-122">Parent elements</span></span>

|<span data-ttu-id="38875-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38875-123">**Element**</span></span>|<span data-ttu-id="38875-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38875-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38875-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="38875-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="38875-126">Contém definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="38875-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38875-127">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="38875-127">Text value</span></span>

<span data-ttu-id="38875-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38875-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38875-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="38875-129">Remarks</span></span>

<span data-ttu-id="38875-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="38875-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38875-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="38875-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38875-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="38875-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38875-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38875-133">Schema Name</span></span>  <br/> |<span data-ttu-id="38875-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="38875-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38875-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38875-135">Validation File</span></span>  <br/> |<span data-ttu-id="38875-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38875-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38875-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="38875-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="38875-138">False</span><span class="sxs-lookup"><span data-stu-id="38875-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38875-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="38875-139">See also</span></span>



- [<span data-ttu-id="38875-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="38875-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

