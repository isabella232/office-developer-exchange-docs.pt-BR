---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: O elemento FindMessageTrackingReport Especifica os critérios para os tipos de mensagens para encontrar.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752294"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="a77e6-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a77e6-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="a77e6-104">O elemento **FindMessageTrackingReport** Especifica os critérios para os tipos de mensagens para encontrar.</span><span class="sxs-lookup"><span data-stu-id="a77e6-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 <span data-ttu-id="a77e6-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="a77e6-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a77e6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a77e6-106">Attributes and elements</span></span>

<span data-ttu-id="a77e6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a77e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a77e6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a77e6-108">Attributes</span></span>

<span data-ttu-id="a77e6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a77e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a77e6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a77e6-110">Child elements</span></span>

|<span data-ttu-id="a77e6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a77e6-111">**Element**</span></span>|<span data-ttu-id="a77e6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a77e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a77e6-113">Escopo (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a77e6-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="a77e6-114">Representa o quão abrangente o relatório de controle de mensagens devem ser.</span><span class="sxs-lookup"><span data-stu-id="a77e6-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-115">Domínio (rastreamento de mensagens)</span><span class="sxs-lookup"><span data-stu-id="a77e6-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="a77e6-116">Contém o nome do domínio onde a acompanhamento de mensagens é executada.</span><span class="sxs-lookup"><span data-stu-id="a77e6-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-117">Remetente (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a77e6-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="a77e6-118">Contém informações de contato para o remetente da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="a77e6-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="a77e6-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="a77e6-120">Contém informações de contato para o emissor Denúncia de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="a77e6-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-121">Recipient</span><span class="sxs-lookup"><span data-stu-id="a77e6-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="a77e6-122">Contém o endereço de email para o destinatário da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a77e6-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="a77e6-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="a77e6-124">Contém o assunto da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="a77e6-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="a77e6-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="a77e6-126">Contém a data e a hora para a pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="a77e6-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="a77e6-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="a77e6-128">Contém a data e a hora para a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a77e6-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="a77e6-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="a77e6-130">Contém o identificador de mensagem para a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a77e6-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="a77e6-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="a77e6-132">Contém o nome da caixa de correio em que a mensagem de entre local foi enviada.</span><span class="sxs-lookup"><span data-stu-id="a77e6-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="a77e6-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="a77e6-134">Representa o nível de detalhe para relatórios de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="a77e6-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="a77e6-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="a77e6-136">Representa o ponto de partida para rastreamento de uma mensagem em um site remoto ou da floresta.</span><span class="sxs-lookup"><span data-stu-id="a77e6-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="a77e6-137">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="a77e6-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="a77e6-138">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="a77e6-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="a77e6-139">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="a77e6-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a77e6-140">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a77e6-140">Parent elements</span></span>

<span data-ttu-id="a77e6-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a77e6-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a77e6-142">Text value</span><span class="sxs-lookup"><span data-stu-id="a77e6-142">Text value</span></span>

<span data-ttu-id="a77e6-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a77e6-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a77e6-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="a77e6-144">Remarks</span></span>

<span data-ttu-id="a77e6-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a77e6-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a77e6-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a77e6-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a77e6-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="a77e6-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a77e6-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a77e6-148">Schema Name</span></span>  <br/> |<span data-ttu-id="a77e6-149">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a77e6-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a77e6-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a77e6-150">Validation File</span></span>  <br/> |<span data-ttu-id="a77e6-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a77e6-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a77e6-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a77e6-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="a77e6-153">False</span><span class="sxs-lookup"><span data-stu-id="a77e6-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a77e6-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="a77e6-154">See also</span></span>



[<span data-ttu-id="a77e6-155">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a77e6-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="a77e6-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a77e6-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

