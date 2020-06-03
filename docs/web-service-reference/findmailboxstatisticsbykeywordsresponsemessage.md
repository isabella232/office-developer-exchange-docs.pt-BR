---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: O elemento FindMailboxStatisticsByKeywordsResponseMessage especifica a mensagem de resposta para uma solicitação FindMailboxStatisticsByKeywords.
ms.openlocfilehash: 704eebbf82db2871ab36be8e5b30c88c6959baa5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525973"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a><span data-ttu-id="54dc5-103">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54dc5-103">FindMailboxStatisticsByKeywordsResponseMessage</span></span>

<span data-ttu-id="54dc5-104">O elemento **FindMailboxStatisticsByKeywordsResponseMessage** especifica a mensagem de resposta para uma solicitação **FindMailboxStatisticsByKeywords** .</span><span class="sxs-lookup"><span data-stu-id="54dc5-104">The **FindMailboxStatisticsByKeywordsResponseMessage** element specifies the response message for a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 <span data-ttu-id="54dc5-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="54dc5-105">**FindMailboxStatisticsByKeywordsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54dc5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="54dc5-106">Attributes and elements</span></span>

<span data-ttu-id="54dc5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54dc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54dc5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="54dc5-108">Attributes</span></span>

|<span data-ttu-id="54dc5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="54dc5-109">**Attribute**</span></span>|<span data-ttu-id="54dc5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54dc5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54dc5-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="54dc5-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="54dc5-112">Especifica a classe de resposta.</span><span class="sxs-lookup"><span data-stu-id="54dc5-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="54dc5-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="54dc5-113">ResponseClass</span></span>

|<span data-ttu-id="54dc5-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="54dc5-114">**Value**</span></span>|<span data-ttu-id="54dc5-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54dc5-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54dc5-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="54dc5-116">Success</span></span>  <br/> |<span data-ttu-id="54dc5-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="54dc5-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="54dc5-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="54dc5-118">Warning</span></span>  <br/> |<span data-ttu-id="54dc5-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="54dc5-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="54dc5-120">Erro</span><span class="sxs-lookup"><span data-stu-id="54dc5-120">Error</span></span>  <br/> |<span data-ttu-id="54dc5-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="54dc5-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="54dc5-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54dc5-122">Child elements</span></span>

|<span data-ttu-id="54dc5-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54dc5-123">**Element**</span></span>|<span data-ttu-id="54dc5-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54dc5-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54dc5-125">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="54dc5-125">MailboxStatisticsSearchResult</span></span>](mailboxstatisticssearchresult.md) <br/> |<span data-ttu-id="54dc5-126">Especifica o resultado de uma pesquisa de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="54dc5-126">Specifies the result of a mailbox search.</span></span>  <br/> |
|[<span data-ttu-id="54dc5-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="54dc5-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="54dc5-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="54dc5-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="54dc5-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54dc5-129">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="54dc5-130">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="54dc5-130">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="54dc5-131">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="54dc5-131">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="54dc5-132">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="54dc5-132">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="54dc5-133">MessageXml</span><span class="sxs-lookup"><span data-stu-id="54dc5-133">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="54dc5-134">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="54dc5-134">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54dc5-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54dc5-135">Parent elements</span></span>

|<span data-ttu-id="54dc5-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54dc5-136">**Element**</span></span>|<span data-ttu-id="54dc5-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54dc5-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54dc5-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="54dc5-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="54dc5-139">Especifica uma matriz de mensagens de resposta.</span><span class="sxs-lookup"><span data-stu-id="54dc5-139">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54dc5-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="54dc5-140">Remarks</span></span>

<span data-ttu-id="54dc5-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="54dc5-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="54dc5-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54dc5-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54dc5-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="54dc5-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54dc5-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="54dc5-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54dc5-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54dc5-145">Schema Name</span></span>  <br/> |<span data-ttu-id="54dc5-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="54dc5-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="54dc5-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54dc5-147">Validation File</span></span>  <br/> |<span data-ttu-id="54dc5-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="54dc5-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54dc5-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="54dc5-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="54dc5-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="54dc5-150">See also</span></span>



- [<span data-ttu-id="54dc5-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="54dc5-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

