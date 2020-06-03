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
description: O elemento ResponseMessages contém uma matriz de mensagens de resposta de configuração de serviço.
ms.openlocfilehash: cf271224141ffeb6dc00069abf430ab33d3ca2fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457449"
---
# <a name="responsemessages-arrayofserviceconfigurationresponsemessagetype"></a><span data-ttu-id="6b816-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="6b816-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>

<span data-ttu-id="6b816-104">O elemento **ResponseMessages** contém uma matriz de mensagens de resposta de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="6b816-104">The **ResponseMessages** element contains an array of service configuration response messages.</span></span> 
  
```XML
<ResponseMessages>
   <ServiceConfigurationResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="6b816-105">**ArrayOfServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6b816-105">**ArrayOfServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b816-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6b816-106">Attributes and elements</span></span>

<span data-ttu-id="6b816-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6b816-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b816-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6b816-108">Attributes</span></span>

<span data-ttu-id="6b816-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b816-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b816-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6b816-110">Child elements</span></span>

|<span data-ttu-id="6b816-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6b816-111">**Element**</span></span>|<span data-ttu-id="6b816-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b816-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b816-113">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="6b816-113">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="6b816-114">Contém definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="6b816-114">Contains service configuration settings.</span></span> <span data-ttu-id="6b816-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b816-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b816-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6b816-116">Parent elements</span></span>

|<span data-ttu-id="6b816-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6b816-117">**Element**</span></span>|<span data-ttu-id="6b816-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b816-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b816-119">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="6b816-119">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="6b816-120">Define uma resposta a uma solicitação GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6b816-120">Defines a response to a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b816-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6b816-121">Text value</span></span>

<span data-ttu-id="6b816-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6b816-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b816-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="6b816-123">Remarks</span></span>

<span data-ttu-id="6b816-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b816-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b816-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6b816-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b816-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b816-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b816-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6b816-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6b816-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6b816-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b816-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6b816-129">Validation File</span></span>  <br/> |<span data-ttu-id="6b816-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b816-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b816-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6b816-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b816-132">False</span><span class="sxs-lookup"><span data-stu-id="6b816-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b816-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="6b816-133">See also</span></span>



- [<span data-ttu-id="6b816-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6b816-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

