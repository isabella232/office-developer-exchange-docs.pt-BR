---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: O elemento GetConversationItemsResponseMessage Especifica a mensagem de resposta para uma solicitação de GetConversationItems.
ms.openlocfilehash: 997319193311ef9267d8f6ff14c70bfe40e2634b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752443"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="66383-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="66383-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="66383-104">O elemento **GetConversationItemsResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="66383-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="66383-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="66383-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66383-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="66383-106">Attributes and elements</span></span>

<span data-ttu-id="66383-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="66383-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66383-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="66383-108">Attributes</span></span>

|<span data-ttu-id="66383-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="66383-109">**Attribute**</span></span>|<span data-ttu-id="66383-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66383-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66383-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="66383-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="66383-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="66383-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="66383-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="66383-113">ResponseClass</span></span>

|<span data-ttu-id="66383-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="66383-114">**Value**</span></span>|<span data-ttu-id="66383-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66383-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66383-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="66383-116">Success</span></span>  <br/> |<span data-ttu-id="66383-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="66383-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="66383-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="66383-118">Warning</span></span>  <br/> |<span data-ttu-id="66383-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="66383-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="66383-120">Erro</span><span class="sxs-lookup"><span data-stu-id="66383-120">Error</span></span>  <br/> |<span data-ttu-id="66383-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="66383-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66383-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="66383-122">Child elements</span></span>

|<span data-ttu-id="66383-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66383-123">**Element**</span></span>|<span data-ttu-id="66383-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66383-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66383-125">Conversa (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="66383-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="66383-126">Representa uma única conversa retornada em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="66383-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="66383-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="66383-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="66383-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="66383-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="66383-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="66383-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="66383-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="66383-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="66383-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="66383-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="66383-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="66383-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="66383-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="66383-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="66383-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="66383-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66383-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="66383-135">Parent elements</span></span>

|<span data-ttu-id="66383-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66383-136">**Element**</span></span>|<span data-ttu-id="66383-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66383-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66383-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="66383-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="66383-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="66383-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66383-140">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="66383-140">Remarks</span></span>

<span data-ttu-id="66383-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="66383-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66383-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="66383-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66383-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="66383-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66383-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="66383-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66383-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="66383-145">Schema Name</span></span>  <br/> |<span data-ttu-id="66383-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="66383-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="66383-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="66383-147">Validation File</span></span>  <br/> |<span data-ttu-id="66383-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="66383-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66383-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="66383-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="66383-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="66383-150">See also</span></span>



- [<span data-ttu-id="66383-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66383-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

