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
description: O elemento RequestedConfiguration contém as configurações de serviço solicitadas.
ms.openlocfilehash: bbc503e6d6f7c56c785365924106bc2468965d0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457148"
---
# <a name="requestedconfiguration"></a><span data-ttu-id="3d302-103">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d302-103">RequestedConfiguration</span></span>

<span data-ttu-id="3d302-104">O elemento **RequestedConfiguration** contém as configurações de serviço solicitadas.</span><span class="sxs-lookup"><span data-stu-id="3d302-104">The **RequestedConfiguration** element contains the requested service configurations.</span></span> 
  
```XML
<RequestedConfiguration>
   <ConfigurationName/>
</RequestedConfiguration>
```

 <span data-ttu-id="3d302-105">**ArrayOfServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="3d302-105">**ArrayOfServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d302-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3d302-106">Attributes and elements</span></span>

<span data-ttu-id="3d302-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3d302-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d302-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3d302-108">Attributes</span></span>

<span data-ttu-id="3d302-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d302-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d302-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3d302-110">Child elements</span></span>

|<span data-ttu-id="3d302-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d302-111">**Element**</span></span>|<span data-ttu-id="3d302-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d302-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d302-113">Configuration</span><span class="sxs-lookup"><span data-stu-id="3d302-113">ConfigurationName</span></span>](configurationname.md) <br/> |<span data-ttu-id="3d302-114">Especifica as configurações de serviço solicitadas por nome.</span><span class="sxs-lookup"><span data-stu-id="3d302-114">Specifies the requested service configurations by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d302-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3d302-115">Parent elements</span></span>

|<span data-ttu-id="3d302-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d302-116">**Element**</span></span>|<span data-ttu-id="3d302-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d302-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d302-118">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d302-118">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="3d302-119">Define uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3d302-119">Defines a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3d302-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3d302-120">Text value</span></span>

<span data-ttu-id="3d302-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d302-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3d302-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d302-122">Remarks</span></span>

<span data-ttu-id="3d302-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d302-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d302-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3d302-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d302-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d302-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3d302-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3d302-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3d302-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3d302-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3d302-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3d302-128">Validation File</span></span>  <br/> |<span data-ttu-id="3d302-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3d302-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d302-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3d302-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d302-131">False</span><span class="sxs-lookup"><span data-stu-id="3d302-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d302-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="3d302-132">See also</span></span>



- [<span data-ttu-id="3d302-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3d302-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

