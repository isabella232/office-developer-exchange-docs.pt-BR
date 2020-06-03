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
description: O elemento PhoneCallInformation especifica as informações de estado de uma chamada telefônica.
ms.openlocfilehash: 75370bccb841818a8302bdd055ad96fd16b2e8df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468842"
---
# <a name="phonecallinformation"></a><span data-ttu-id="9dc6e-103">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="9dc6e-103">PhoneCallInformation</span></span>

<span data-ttu-id="9dc6e-104">O elemento **PhoneCallInformation** especifica as informações de estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-104">The **PhoneCallInformation** element specifies the state information for a phone call.</span></span> 
  
```XML
<PhoneCallInformation>
   <PhoneCallState/>
   <ConnectionFailureCause/>
   <SIPResponseText/>
   <SIPResponseCode/>
</PhoneCallInformation>
```

 <span data-ttu-id="9dc6e-105">**PhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="9dc6e-105">**PhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9dc6e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9dc6e-106">Attributes and elements</span></span>

<span data-ttu-id="9dc6e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9dc6e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9dc6e-108">Attributes</span></span>

<span data-ttu-id="9dc6e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9dc6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9dc6e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9dc6e-110">Child elements</span></span>

|<span data-ttu-id="9dc6e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9dc6e-111">**Element**</span></span>|<span data-ttu-id="9dc6e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9dc6e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dc6e-113">Chamada do telefonema</span><span class="sxs-lookup"><span data-stu-id="9dc6e-113">PhoneCallState</span></span>](phonecallstate.md) <br/> |<span data-ttu-id="9dc6e-114">Especifica o estado de uma chamada telefônica.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-114">Specifies the state for a phone call.</span></span> <span data-ttu-id="9dc6e-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9dc6e-116">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="9dc6e-116">ConnectionFailureCause</span></span>](connectionfailurecause.md) <br/> |<span data-ttu-id="9dc6e-117">Especifica a causa de uma falha de conexão.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-117">Specifies the cause of a connection failure.</span></span> <span data-ttu-id="9dc6e-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9dc6e-119">SIPResponseText</span><span class="sxs-lookup"><span data-stu-id="9dc6e-119">SIPResponseText</span></span>](sipresponsetext.md) <br/> |<span data-ttu-id="9dc6e-120">Especifica o texto de resposta SIP.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-120">Specifies the SIP response text.</span></span> <span data-ttu-id="9dc6e-121">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9dc6e-122">SIPResponseCode</span><span class="sxs-lookup"><span data-stu-id="9dc6e-122">SIPResponseCode</span></span>](sipresponsecode.md) <br/> |<span data-ttu-id="9dc6e-123">Especifica o código de resposta SIP.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-123">Specifies the SIP response code.</span></span> <span data-ttu-id="9dc6e-124">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-124">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9dc6e-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9dc6e-125">Parent elements</span></span>

|<span data-ttu-id="9dc6e-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9dc6e-126">**Element**</span></span>|<span data-ttu-id="9dc6e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9dc6e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9dc6e-128">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="9dc6e-128">GetPhoneCallInformationResponse</span></span>](getphonecallinformationresponse.md) <br/> |<span data-ttu-id="9dc6e-129">Define uma resposta a uma solicitação de [operação GetPhoneCallInformation](getphonecallinformation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9dc6e-129">Defines a response to a [GetPhoneCallInformation operation](getphonecallinformation-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9dc6e-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="9dc6e-130">Remarks</span></span>

<span data-ttu-id="9dc6e-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9dc6e-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9dc6e-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9dc6e-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9dc6e-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="9dc6e-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9dc6e-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9dc6e-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9dc6e-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9dc6e-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9dc6e-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9dc6e-136">Validation File</span></span>  <br/> |<span data-ttu-id="9dc6e-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9dc6e-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9dc6e-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9dc6e-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9dc6e-139">False</span><span class="sxs-lookup"><span data-stu-id="9dc6e-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9dc6e-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="9dc6e-140">See also</span></span>



- [<span data-ttu-id="9dc6e-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9dc6e-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

