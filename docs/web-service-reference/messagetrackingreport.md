---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: O elemento MessageTrackingReport contém uma única mensagem que é retornada em uma operação GetMessageTrackingReport.
ms.openlocfilehash: fc3e56fbb1bee411fa31751f558f520874133076
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463213"
---
# <a name="messagetrackingreport"></a><span data-ttu-id="fcdeb-103">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fcdeb-103">MessageTrackingReport</span></span>

<span data-ttu-id="fcdeb-104">O elemento **MessageTrackingReport** contém uma única mensagem que é retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fcdeb-104">The **MessageTrackingReport** element contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 <span data-ttu-id="fcdeb-105">**MessageTrackingReportType**</span><span class="sxs-lookup"><span data-stu-id="fcdeb-105">**MessageTrackingReportType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcdeb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fcdeb-106">Attributes and elements</span></span>

<span data-ttu-id="fcdeb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcdeb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fcdeb-108">Attributes</span></span>

<span data-ttu-id="fcdeb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fcdeb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcdeb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fcdeb-110">Child elements</span></span>

|<span data-ttu-id="fcdeb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fcdeb-111">**Element**</span></span>|<span data-ttu-id="fcdeb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fcdeb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcdeb-113">Remetente (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="fcdeb-113">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="fcdeb-114">Contém informações de contato para o remetente da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-114">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-115">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="fcdeb-115">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="fcdeb-116">Contém informações de contato para o remetente supostamente de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-116">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-117">Assunto</span><span class="sxs-lookup"><span data-stu-id="fcdeb-117">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="fcdeb-118">Contém o assunto da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-118">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-119">Enviartime</span><span class="sxs-lookup"><span data-stu-id="fcdeb-119">SubmitTime</span></span>](submittime.md) <br/> |<span data-ttu-id="fcdeb-120">Contém a hora do dia em que a mensagem de email foi enviada.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-120">Contains the time of day that the e-mail message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-121">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="fcdeb-121">OriginalRecipients</span></span>](originalrecipients.md) <br/> |<span data-ttu-id="fcdeb-122">Contém uma lista dos destinatários da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-122">Contains a list of the recipients of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-123">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="fcdeb-123">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="fcdeb-124">Contém uma lista de um ou mais eventos de controle para os destinatários.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-124">Contains a list of one or more tracking events for the recipients.</span></span>  <br/> |
|[<span data-ttu-id="fcdeb-125">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="fcdeb-125">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="fcdeb-126">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-126">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fcdeb-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fcdeb-127">Parent elements</span></span>

|<span data-ttu-id="fcdeb-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fcdeb-128">**Element**</span></span>|<span data-ttu-id="fcdeb-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fcdeb-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcdeb-130">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="fcdeb-130">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="fcdeb-131">Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fcdeb-131">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fcdeb-132">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fcdeb-132">Text value</span></span>

<span data-ttu-id="fcdeb-133">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fcdeb-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fcdeb-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="fcdeb-134">Remarks</span></span>

<span data-ttu-id="fcdeb-135">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="fcdeb-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcdeb-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fcdeb-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcdeb-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="fcdeb-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fcdeb-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fcdeb-138">Schema Name</span></span>  <br/> |<span data-ttu-id="fcdeb-139">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fcdeb-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fcdeb-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fcdeb-140">Validation File</span></span>  <br/> |<span data-ttu-id="fcdeb-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fcdeb-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fcdeb-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fcdeb-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="fcdeb-143">False</span><span class="sxs-lookup"><span data-stu-id="fcdeb-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fcdeb-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="fcdeb-144">See also</span></span>



[<span data-ttu-id="fcdeb-145">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fcdeb-145">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="fcdeb-146">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fcdeb-146">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="fcdeb-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fcdeb-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
- [<span data-ttu-id="fcdeb-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fcdeb-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

