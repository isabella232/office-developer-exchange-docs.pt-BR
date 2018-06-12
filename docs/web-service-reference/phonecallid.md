---
title: PhoneCallId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallId
api_type:
- schema
ms.assetid: 79e31a4c-fc84-4802-8761-470df8d63694
description: O elemento PhoneCallId Especifica o identificador de uma chamada telefônica. Este elemento é obrigatório.
ms.openlocfilehash: 1886d9510fe254c016779166efccc9882fd77d2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824757"
---
# <a name="phonecallid"></a><span data-ttu-id="4a739-104">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="4a739-104">PhoneCallId</span></span>

<span data-ttu-id="4a739-105">O elemento **PhoneCallId** Especifica o identificador de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="4a739-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="4a739-106">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a739-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="4a739-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="4a739-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a739-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4a739-108">Attributes and elements</span></span>

<span data-ttu-id="4a739-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4a739-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a739-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="4a739-110">Attributes</span></span>

|<span data-ttu-id="4a739-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="4a739-111">**Attribute**</span></span>|<span data-ttu-id="4a739-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4a739-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a739-113">Id</span><span class="sxs-lookup"><span data-stu-id="4a739-113">Id</span></span>  <br/> |<span data-ttu-id="4a739-114">Identifica a chamada telefônica para desconectar.</span><span class="sxs-lookup"><span data-stu-id="4a739-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="4a739-115">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="4a739-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4a739-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4a739-116">Child elements</span></span>

<span data-ttu-id="4a739-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4a739-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a739-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4a739-118">Parent elements</span></span>

|<span data-ttu-id="4a739-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4a739-119">**Element**</span></span>|<span data-ttu-id="4a739-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4a739-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a739-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="4a739-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="4a739-122">Representa uma solicitação para desconectar chamada.</span><span class="sxs-lookup"><span data-stu-id="4a739-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="4a739-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="4a739-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="4a739-124">Representa uma solicitação para obter informações de chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="4a739-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="4a739-125">PlayOnPhoneResponse (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="4a739-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="4a739-126">Define uma resposta a uma solicitação PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="4a739-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a739-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4a739-127">Remarks</span></span>

<span data-ttu-id="4a739-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4a739-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a739-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4a739-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a739-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="4a739-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a739-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4a739-131">Schema Name</span></span>  <br/> |<span data-ttu-id="4a739-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4a739-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4a739-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4a739-133">Validation File</span></span>  <br/> |<span data-ttu-id="4a739-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4a739-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a739-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4a739-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a739-136">False</span><span class="sxs-lookup"><span data-stu-id="4a739-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a739-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="4a739-137">See also</span></span>



- [<span data-ttu-id="4a739-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4a739-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

