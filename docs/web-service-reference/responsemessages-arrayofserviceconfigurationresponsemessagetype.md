---
title: ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: c7cfa0d1-fcb2-441f-8489-3a549da33b34
description: O elemento ResponseMessages contém uma matriz das mensagens de resposta de configuração do serviço.
ms.openlocfilehash: af8a6db8d6e9d3ec76b532a81ef2a7392dcfde7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825194"
---
# <a name="responsemessages-arrayofserviceconfigurationresponsemessagetype"></a><span data-ttu-id="5c827-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="5c827-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>

<span data-ttu-id="5c827-104">O elemento **ResponseMessages** contém uma matriz das mensagens de resposta de configuração do serviço.</span><span class="sxs-lookup"><span data-stu-id="5c827-104">The **ResponseMessages** element contains an array of service configuration response messages.</span></span> 
  
```XML
<ResponseMessages>
   <ServiceConfigurationResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="5c827-105">**ArrayOfServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5c827-105">**ArrayOfServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c827-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5c827-106">Attributes and elements</span></span>

<span data-ttu-id="5c827-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c827-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c827-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c827-108">Attributes</span></span>

<span data-ttu-id="5c827-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c827-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c827-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c827-110">Child elements</span></span>

|<span data-ttu-id="5c827-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c827-111">**Element**</span></span>|<span data-ttu-id="5c827-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c827-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c827-113">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="5c827-113">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="5c827-114">Contém as definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="5c827-114">Contains service configuration settings.</span></span> <span data-ttu-id="5c827-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c827-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c827-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c827-116">Parent elements</span></span>

|<span data-ttu-id="5c827-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c827-117">**Element**</span></span>|<span data-ttu-id="5c827-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c827-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c827-119">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="5c827-119">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="5c827-120">Define uma resposta a uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5c827-120">Defines a response to a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c827-121">Text value</span><span class="sxs-lookup"><span data-stu-id="5c827-121">Text value</span></span>

<span data-ttu-id="5c827-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c827-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c827-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c827-123">Remarks</span></span>

<span data-ttu-id="5c827-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c827-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c827-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5c827-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c827-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c827-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c827-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c827-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5c827-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5c827-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c827-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c827-129">Validation File</span></span>  <br/> |<span data-ttu-id="5c827-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c827-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c827-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c827-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c827-132">False</span><span class="sxs-lookup"><span data-stu-id="5c827-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c827-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="5c827-133">See also</span></span>



- [<span data-ttu-id="5c827-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c827-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

