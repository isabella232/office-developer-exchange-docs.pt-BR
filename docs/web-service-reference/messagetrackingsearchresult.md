---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: O elemento MessageTrackingSearchResult contém um resultado de mensagem única de um elemento FindMessageTrackingReportResponse.
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824460"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="7c3dc-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="7c3dc-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="7c3dc-104">O elemento **MessageTrackingSearchResult** contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7c3dc-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 <span data-ttu-id="7c3dc-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="7c3dc-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c3dc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7c3dc-106">Attributes and elements</span></span>

<span data-ttu-id="7c3dc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c3dc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7c3dc-108">Attributes</span></span>

<span data-ttu-id="7c3dc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c3dc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7c3dc-110">Child elements</span></span>

|<span data-ttu-id="7c3dc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c3dc-111">**Element**</span></span>|<span data-ttu-id="7c3dc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c3dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c3dc-113">Assunto</span><span class="sxs-lookup"><span data-stu-id="7c3dc-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="7c3dc-114">Contém o assunto da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-115">Remetente (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7c3dc-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="7c3dc-116">Contém o endereço do remetente de mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="7c3dc-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="7c3dc-118">Contém informações de contato para o emissor Denúncia de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-119">Destinatários (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="7c3dc-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="7c3dc-120">Contém uma lista de endereços de email que recebeu esta mensagem.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="7c3dc-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="7c3dc-122">Contém a hora em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-123">Messagetrackingreportid deve ser passado</span><span class="sxs-lookup"><span data-stu-id="7c3dc-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="7c3dc-124">Contém uma ID interna que identifica a mensagem no banco de dados de transporte.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="7c3dc-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="7c3dc-126">Contém o nome do servidor na floresta que anteriormente aceita a mensagem.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="7c3dc-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="7c3dc-128">Contém o nome do servidor na floresta que primeiro aceita a mensagem.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="7c3dc-129">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="7c3dc-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="7c3dc-130">Contém uma lista de uma ou mais propriedades de controle.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c3dc-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7c3dc-131">Parent elements</span></span>

|<span data-ttu-id="7c3dc-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c3dc-132">**Element**</span></span>|<span data-ttu-id="7c3dc-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c3dc-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c3dc-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="7c3dc-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="7c3dc-135">Contém uma lista de mensagens que correspondem aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c3dc-136">Text value</span><span class="sxs-lookup"><span data-stu-id="7c3dc-136">Text value</span></span>

<span data-ttu-id="7c3dc-137">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7c3dc-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c3dc-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="7c3dc-138">Remarks</span></span>

<span data-ttu-id="7c3dc-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7c3dc-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c3dc-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7c3dc-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c3dc-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c3dc-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c3dc-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7c3dc-142">Schema Name</span></span>  <br/> |<span data-ttu-id="7c3dc-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7c3dc-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c3dc-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7c3dc-144">Validation File</span></span>  <br/> |<span data-ttu-id="7c3dc-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c3dc-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c3dc-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7c3dc-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c3dc-147">False</span><span class="sxs-lookup"><span data-stu-id="7c3dc-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c3dc-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="7c3dc-148">See also</span></span>



[<span data-ttu-id="7c3dc-149">Operação FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7c3dc-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="7c3dc-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7c3dc-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

