---
title: PhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallInformation
api_type:
- schema
ms.assetid: a0363c42-6d35-4074-bc17-946eb12736ff
description: O elemento PhoneCallInformation Especifica as informações de estado de uma chamada telefônica.
ms.openlocfilehash: e64e7b38b3801c60df8a966e95d980746533d3a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824758"
---
# <a name="phonecallinformation"></a><span data-ttu-id="706d7-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="706d7-103">PhoneCallInformation</span></span>

<span data-ttu-id="706d7-104">O elemento **PhoneCallInformation** Especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="706d7-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="706d7-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="706d7-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="706d7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="706d7-106">Attributes and elements</span></span>

<span data-ttu-id="706d7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="706d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="706d7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="706d7-108">Attributes</span></span>

<span data-ttu-id="706d7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="706d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="706d7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="706d7-110">Child elements</span></span>

|<span data-ttu-id="706d7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="706d7-111">**Element**</span></span>|<span data-ttu-id="706d7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="706d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="706d7-113">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="706d7-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="706d7-114">Especifica o estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="706d7-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="706d7-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="706d7-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="706d7-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="706d7-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="706d7-117">Especifica a causa de uma falha de conexão.</span><span class="sxs-lookup"><span data-stu-id="706d7-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="706d7-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="706d7-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="706d7-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="706d7-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="706d7-120">Especifica o texto de resposta SIP.</span><span class="sxs-lookup"><span data-stu-id="706d7-120">Specifies the SIP response text.</span></span> <span data-ttu-id="706d7-121">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="706d7-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="706d7-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="706d7-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="706d7-123">Especifica o código de resposta SIP.</span><span class="sxs-lookup"><span data-stu-id="706d7-123">Specifies the SIP response code.</span></span> <span data-ttu-id="706d7-124">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="706d7-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="706d7-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="706d7-125">Parent elements</span></span>

|<span data-ttu-id="706d7-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="706d7-126">**Element**</span></span>|<span data-ttu-id="706d7-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="706d7-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="706d7-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="706d7-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="706d7-129">Define uma resposta a uma solicitação de [operação GetPhoneCallInformation](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="706d7-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="706d7-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="706d7-130">Remarks</span></span>

<span data-ttu-id="706d7-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="706d7-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="706d7-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="706d7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="706d7-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="706d7-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="706d7-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="706d7-134">Schema Name</span></span>  <br/> |<span data-ttu-id="706d7-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="706d7-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="706d7-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="706d7-136">Validation File</span></span>  <br/> |<span data-ttu-id="706d7-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="706d7-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="706d7-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="706d7-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="706d7-139">False</span><span class="sxs-lookup"><span data-stu-id="706d7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="706d7-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="706d7-140">See also</span></span>



- [<span data-ttu-id="706d7-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="706d7-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

