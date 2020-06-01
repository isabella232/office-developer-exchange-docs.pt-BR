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
description: O elemento FindMessageTrackingReport especifica critérios para os tipos de mensagens a serem localizados.
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462933"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="8dd0a-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8dd0a-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="8dd0a-104">O elemento **FindMessageTrackingReport** especifica critérios para os tipos de mensagens a serem localizados.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
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

 <span data-ttu-id="8dd0a-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="8dd0a-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8dd0a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8dd0a-106">Attributes and elements</span></span>

<span data-ttu-id="8dd0a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8dd0a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8dd0a-108">Attributes</span></span>

<span data-ttu-id="8dd0a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8dd0a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8dd0a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8dd0a-110">Child elements</span></span>

|<span data-ttu-id="8dd0a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8dd0a-111">**Element**</span></span>|<span data-ttu-id="8dd0a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8dd0a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8dd0a-113">Escopo (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="8dd0a-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="8dd0a-114">Representa o quão abrangentes o relatório de acompanhamento de mensagens deve ser.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-115">Domínio (controle de mensagens)</span><span class="sxs-lookup"><span data-stu-id="8dd0a-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="8dd0a-116">Contém o nome do domínio onde o controle de mensagens é executado.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-117">Remetente (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="8dd0a-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="8dd0a-118">Contém informações de contato para o remetente da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="8dd0a-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="8dd0a-120">Contém informações de contato para o remetente supostamente de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-121">Recipiente</span><span class="sxs-lookup"><span data-stu-id="8dd0a-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="8dd0a-122">Contém o endereço de email do destinatário da mensagem.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-123">Assunto</span><span class="sxs-lookup"><span data-stu-id="8dd0a-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="8dd0a-124">Contém o assunto da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="8dd0a-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="8dd0a-126">Contém a data e hora inicial da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="8dd0a-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="8dd0a-128">Contém a data e a hora de término da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="8dd0a-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="8dd0a-130">Contém o identificador de mensagem para a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="8dd0a-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="8dd0a-132">Contém o nome da caixa de correio onde a mensagem entre locais foi enviada.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="8dd0a-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="8dd0a-134">Representa o nível de detalhes dos relatórios de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="8dd0a-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="8dd0a-136">Representa o ponto de partida para rastrear uma mensagem em um site ou floresta remoto.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="8dd0a-137">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="8dd0a-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="8dd0a-138">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="8dd0a-139">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8dd0a-140">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8dd0a-140">Parent elements</span></span>

<span data-ttu-id="8dd0a-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8dd0a-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8dd0a-142">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8dd0a-142">Text value</span></span>

<span data-ttu-id="8dd0a-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8dd0a-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="8dd0a-144">Remarks</span></span>

<span data-ttu-id="8dd0a-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8dd0a-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8dd0a-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8dd0a-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8dd0a-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="8dd0a-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8dd0a-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8dd0a-148">Schema Name</span></span>  <br/> |<span data-ttu-id="8dd0a-149">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8dd0a-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8dd0a-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8dd0a-150">Validation File</span></span>  <br/> |<span data-ttu-id="8dd0a-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8dd0a-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8dd0a-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8dd0a-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="8dd0a-153">False</span><span class="sxs-lookup"><span data-stu-id="8dd0a-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8dd0a-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="8dd0a-154">See also</span></span>



[<span data-ttu-id="8dd0a-155">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="8dd0a-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="8dd0a-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8dd0a-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

