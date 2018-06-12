---
title: RequestedConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedConfiguration
api_type:
- schema
ms.assetid: 24921387-f676-49e6-8d7a-ef3115024866
description: O elemento RequestedConfiguration contém as configurações do serviço solicitado.
ms.openlocfilehash: 1edc6394360250c9a9810fe614c975cb48eba3f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825130"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="577df-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="577df-103">RequestedConfiguration</span></span>

<span data-ttu-id="577df-104">O elemento **RequestedConfiguration** contém as configurações do serviço solicitado.</span><span class="sxs-lookup"><span data-stu-id="577df-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="577df-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="577df-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="577df-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="577df-106">Attributes and elements</span></span>

<span data-ttu-id="577df-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="577df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="577df-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="577df-108">Attributes</span></span>

<span data-ttu-id="577df-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="577df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="577df-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="577df-110">Child elements</span></span>

|<span data-ttu-id="577df-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="577df-111">**Element**</span></span>|<span data-ttu-id="577df-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="577df-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="577df-113">ConfigurationName</span><span class="sxs-lookup"><span data-stu-id="577df-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="577df-114">Especifica as configurações de serviço solicitado pelo nome.</span><span class="sxs-lookup"><span data-stu-id="577df-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="577df-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="577df-115">Parent elements</span></span>

|<span data-ttu-id="577df-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="577df-116">**Element**</span></span>|<span data-ttu-id="577df-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="577df-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="577df-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="577df-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="577df-119">Define uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="577df-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="577df-120">Text value</span><span class="sxs-lookup"><span data-stu-id="577df-120">Text value</span></span>

<span data-ttu-id="577df-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="577df-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="577df-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="577df-122">Remarks</span></span>

<span data-ttu-id="577df-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="577df-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="577df-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="577df-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="577df-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="577df-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="577df-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="577df-126">Schema Name</span></span>  <br/> |<span data-ttu-id="577df-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="577df-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="577df-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="577df-128">Validation File</span></span>  <br/> |<span data-ttu-id="577df-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="577df-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="577df-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="577df-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="577df-131">False</span><span class="sxs-lookup"><span data-stu-id="577df-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="577df-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="577df-132">See also</span></span>



- [<span data-ttu-id="577df-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="577df-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

