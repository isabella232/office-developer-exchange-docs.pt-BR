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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752292"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="edd98-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="edd98-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="edd98-104">O elemento **FindMailboxStatisticsByKeywordsResponseMessage** Especifica a mensagem de resposta para uma solicitação de **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="edd98-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="edd98-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="edd98-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edd98-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="edd98-106">Attributes and elements</span></span>

<span data-ttu-id="edd98-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="edd98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edd98-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="edd98-108">Attributes</span></span>

|<span data-ttu-id="edd98-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="edd98-109">**Attribute**</span></span>|<span data-ttu-id="edd98-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edd98-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="edd98-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="edd98-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="edd98-112">Especifica a classe de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd98-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="edd98-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="edd98-113">ResponseClass</span></span>

|<span data-ttu-id="edd98-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="edd98-114">**Value**</span></span>|<span data-ttu-id="edd98-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edd98-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="edd98-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="edd98-116">Success</span></span>  <br/> |<span data-ttu-id="edd98-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="edd98-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="edd98-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="edd98-118">Warning</span></span>  <br/> |<span data-ttu-id="edd98-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="edd98-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="edd98-120">Erro</span><span class="sxs-lookup"><span data-stu-id="edd98-120">Error</span></span>  <br/> |<span data-ttu-id="edd98-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="edd98-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="edd98-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="edd98-122">Child elements</span></span>

|<span data-ttu-id="edd98-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="edd98-123">**Element**</span></span>|<span data-ttu-id="edd98-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edd98-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edd98-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="edd98-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="edd98-126">Especifica o resultado de uma pesquisa de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="edd98-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="edd98-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="edd98-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="edd98-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="edd98-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="edd98-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="edd98-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="edd98-130">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="edd98-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="edd98-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="edd98-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="edd98-132">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="edd98-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="edd98-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="edd98-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="edd98-134">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="edd98-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="edd98-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="edd98-135">Parent elements</span></span>

|<span data-ttu-id="edd98-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="edd98-136">**Element**</span></span>|<span data-ttu-id="edd98-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="edd98-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edd98-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="edd98-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="edd98-139">Especifica uma matriz de mensagens de resposta.</span><span class="sxs-lookup"><span data-stu-id="edd98-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="edd98-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="edd98-140">Remarks</span></span>

<span data-ttu-id="edd98-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="edd98-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="edd98-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="edd98-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edd98-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="edd98-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edd98-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="edd98-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="edd98-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="edd98-145">Schema Name</span></span>  <br/> |<span data-ttu-id="edd98-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="edd98-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="edd98-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="edd98-147">Validation File</span></span>  <br/> |<span data-ttu-id="edd98-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="edd98-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="edd98-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="edd98-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="edd98-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="edd98-150">See also</span></span>



- [<span data-ttu-id="edd98-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="edd98-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

