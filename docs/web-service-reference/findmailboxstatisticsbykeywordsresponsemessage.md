---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: O elemento FindMailboxStatisticsByKeywordsResponseMessage Especifica a mensagem de resposta para uma solicitação de FindMailboxStatisticsByKeywords.
ms.openlocfilehash: 9479252ed53335d07a6402707bc69e5eaadfa7c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752292"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="e7f1d-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e7f1d-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="e7f1d-104">O elemento **FindMailboxStatisticsByKeywordsResponseMessage** Especifica a mensagem de resposta para uma solicitação de **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="e7f1d-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="e7f1d-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7f1d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e7f1d-106">Attributes and elements</span></span>

<span data-ttu-id="e7f1d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7f1d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e7f1d-108">Attributes</span></span>

|<span data-ttu-id="e7f1d-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-109">**Attribute**</span></span>|<span data-ttu-id="e7f1d-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f1d-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e7f1d-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="e7f1d-112">Especifica a classe de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="e7f1d-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="e7f1d-113">ResponseClass</span></span>

|<span data-ttu-id="e7f1d-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-114">**Value**</span></span>|<span data-ttu-id="e7f1d-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e7f1d-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="e7f1d-116">Success</span></span>  <br/> |<span data-ttu-id="e7f1d-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="e7f1d-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="e7f1d-118">Warning</span></span>  <br/> |<span data-ttu-id="e7f1d-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="e7f1d-120">Erro</span><span class="sxs-lookup"><span data-stu-id="e7f1d-120">Error</span></span>  <br/> |<span data-ttu-id="e7f1d-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e7f1d-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e7f1d-122">Child elements</span></span>

|<span data-ttu-id="e7f1d-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-123">**Element**</span></span>|<span data-ttu-id="e7f1d-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f1d-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="e7f1d-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="e7f1d-126">Especifica o resultado de uma pesquisa de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="e7f1d-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="e7f1d-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e7f1d-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e7f1d-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e7f1d-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e7f1d-130">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="e7f1d-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e7f1d-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e7f1d-132">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="e7f1d-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e7f1d-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e7f1d-134">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e7f1d-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e7f1d-135">Parent elements</span></span>

|<span data-ttu-id="e7f1d-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-136">**Element**</span></span>|<span data-ttu-id="e7f1d-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e7f1d-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7f1d-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e7f1d-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e7f1d-139">Especifica uma matriz de mensagens de resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e7f1d-140">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e7f1d-140">Remarks</span></span>

<span data-ttu-id="e7f1d-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e7f1d-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7f1d-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7f1d-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e7f1d-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7f1d-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="e7f1d-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e7f1d-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e7f1d-145">Schema Name</span></span>  <br/> |<span data-ttu-id="e7f1d-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="e7f1d-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="e7f1d-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e7f1d-147">Validation File</span></span>  <br/> |<span data-ttu-id="e7f1d-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e7f1d-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e7f1d-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e7f1d-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e7f1d-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="e7f1d-150">See also</span></span>



- [<span data-ttu-id="e7f1d-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e7f1d-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

