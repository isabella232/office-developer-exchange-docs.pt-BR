---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: O elemento DiscoverySearchConfigurations Especifica uma matriz de elementos de DiscoverySearchConfiguration.
ms.openlocfilehash: a95bb35b88114e8e72e22de424679993fd4eef2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751864"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="5c1d6-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="5c1d6-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="5c1d6-104">O elemento **DiscoverySearchConfigurations** Especifica uma matriz de elementos de **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="5c1d6-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="5c1d6-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="5c1d6-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c1d6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5c1d6-106">Attributes and elements</span></span>

<span data-ttu-id="5c1d6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c1d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c1d6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c1d6-108">Attributes</span></span>

<span data-ttu-id="5c1d6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c1d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c1d6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c1d6-110">Child elements</span></span>

|<span data-ttu-id="5c1d6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c1d6-111">**Element**</span></span>|<span data-ttu-id="5c1d6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c1d6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c1d6-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c1d6-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="5c1d6-114">Especifica a configuração de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="5c1d6-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c1d6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c1d6-115">Parent elements</span></span>

|<span data-ttu-id="5c1d6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c1d6-116">**Element**</span></span>|<span data-ttu-id="5c1d6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c1d6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c1d6-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c1d6-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="5c1d6-119">Especifica a mensagem de resposta para uma solicitação de **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="5c1d6-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c1d6-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="5c1d6-120">Remarks</span></span>

<span data-ttu-id="5c1d6-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5c1d6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5c1d6-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c1d6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c1d6-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5c1d6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c1d6-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c1d6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c1d6-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c1d6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5c1d6-126">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="5c1d6-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="5c1d6-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c1d6-127">Validation File</span></span>  <br/> |<span data-ttu-id="5c1d6-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c1d6-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c1d6-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5c1d6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5c1d6-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c1d6-130">See also</span></span>

- [<span data-ttu-id="5c1d6-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c1d6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

