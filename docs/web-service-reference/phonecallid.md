---
title: Chamada de chamada
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
description: O elemento callid especifica o identificador de uma chamada telefônica. Este elemento é obrigatório.
ms.openlocfilehash: 3e4b9dba5e8be6e45a0c16508531fbc6cf91c170
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459697"
---
# <a name="phonecallid"></a><span data-ttu-id="6d103-104">Chamada de chamada</span><span class="sxs-lookup"><span data-stu-id="6d103-104">PhoneCallId</span></span>

<span data-ttu-id="6d103-105">O **elemento callid especifica o identificador** de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="6d103-105">The **PhoneCallId** element specifies the identifier of a phone call.</span></span> <span data-ttu-id="6d103-106">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d103-106">This element is required.</span></span> 
  
```xml
<PhoneCallId Id="" />
```

 <span data-ttu-id="6d103-107">**PhoneCallIdType**</span><span class="sxs-lookup"><span data-stu-id="6d103-107">**PhoneCallIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d103-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6d103-108">Attributes and elements</span></span>

<span data-ttu-id="6d103-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6d103-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d103-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6d103-110">Attributes</span></span>

|<span data-ttu-id="6d103-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6d103-111">**Attribute**</span></span>|<span data-ttu-id="6d103-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d103-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6d103-113">Id</span><span class="sxs-lookup"><span data-stu-id="6d103-113">Id</span></span>  <br/> |<span data-ttu-id="6d103-114">Identifica a chamada telefônica a ser desconectada.</span><span class="sxs-lookup"><span data-stu-id="6d103-114">Identifies the phone call to disconnect.</span></span> <span data-ttu-id="6d103-115">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6d103-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6d103-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6d103-116">Child elements</span></span>

<span data-ttu-id="6d103-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6d103-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d103-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6d103-118">Parent elements</span></span>

|<span data-ttu-id="6d103-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6d103-119">**Element**</span></span>|<span data-ttu-id="6d103-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6d103-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d103-121">DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="6d103-121">DisconnectPhoneCall</span></span>](disconnectphonecall.md) <br/> |<span data-ttu-id="6d103-122">Representa uma solicitação para desconectar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="6d103-122">Represents a request to disconnect a call.</span></span>  <br/> |
|[<span data-ttu-id="6d103-123">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="6d103-123">GetPhoneCallInformation</span></span>](getphonecallinformation.md) <br/> |<span data-ttu-id="6d103-124">Representa uma solicitação para obter informações de chamadas telefônicas.</span><span class="sxs-lookup"><span data-stu-id="6d103-124">Represents a request to get telephone call information.</span></span>  <br/> |
|[<span data-ttu-id="6d103-125">PlayOnPhoneResponse (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="6d103-125">PlayOnPhoneResponse (Exchange Web Services)</span></span>](playonphoneresponse-exchange-web-services.md) <br/> |<span data-ttu-id="6d103-126">Define uma resposta a uma solicitação PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="6d103-126">Defines a response to a PlayOnPhone request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d103-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="6d103-127">Remarks</span></span>

<span data-ttu-id="6d103-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6d103-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d103-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6d103-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d103-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="6d103-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d103-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6d103-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6d103-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6d103-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6d103-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6d103-133">Validation File</span></span>  <br/> |<span data-ttu-id="6d103-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6d103-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d103-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6d103-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d103-136">False</span><span class="sxs-lookup"><span data-stu-id="6d103-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d103-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="6d103-137">See also</span></span>



- [<span data-ttu-id="6d103-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6d103-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

