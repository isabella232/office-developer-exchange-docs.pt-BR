---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: O elemento GetConversationItemsResponseMessage especifica a mensagem de resposta para uma solicitação GetConversationItems.
ms.openlocfilehash: b38bca60bb51c24a7635391c4e23e5426366cd72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461069"
---
# <a name="getconversationitemsresponsemessage"></a><span data-ttu-id="0b75c-103">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b75c-103">GetConversationItemsResponseMessage</span></span>

<span data-ttu-id="0b75c-104">O elemento **GetConversationItemsResponseMessage** especifica a mensagem de resposta para uma solicitação **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="0b75c-104">The **GetConversationItemsResponseMessage** element specifies the response message for a **GetConversationItems** request.</span></span> 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 <span data-ttu-id="0b75c-105">**GetConversationItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0b75c-105">**GetConversationItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b75c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0b75c-106">Attributes and elements</span></span>

<span data-ttu-id="0b75c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b75c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b75c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b75c-108">Attributes</span></span>

|<span data-ttu-id="0b75c-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="0b75c-109">**Attribute**</span></span>|<span data-ttu-id="0b75c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b75c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b75c-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0b75c-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="0b75c-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b75c-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="0b75c-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0b75c-113">ResponseClass</span></span>

|<span data-ttu-id="0b75c-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0b75c-114">**Value**</span></span>|<span data-ttu-id="0b75c-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b75c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b75c-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="0b75c-116">Success</span></span>  <br/> |<span data-ttu-id="0b75c-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="0b75c-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="0b75c-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="0b75c-118">Warning</span></span>  <br/> |<span data-ttu-id="0b75c-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="0b75c-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="0b75c-120">Erro</span><span class="sxs-lookup"><span data-stu-id="0b75c-120">Error</span></span>  <br/> |<span data-ttu-id="0b75c-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="0b75c-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b75c-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b75c-122">Child elements</span></span>

|<span data-ttu-id="0b75c-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b75c-123">**Element**</span></span>|<span data-ttu-id="0b75c-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b75c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b75c-125">Conversa (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="0b75c-125">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="0b75c-126">Representa uma única conversa retornada em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="0b75c-126">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
|[<span data-ttu-id="0b75c-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0b75c-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0b75c-128">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0b75c-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="0b75c-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="0b75c-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0b75c-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b75c-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0b75c-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0b75c-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0b75c-132">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="0b75c-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0b75c-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0b75c-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0b75c-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b75c-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b75c-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b75c-135">Parent elements</span></span>

|<span data-ttu-id="0b75c-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b75c-136">**Element**</span></span>|<span data-ttu-id="0b75c-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b75c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b75c-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b75c-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0b75c-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="0b75c-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b75c-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b75c-140">Remarks</span></span>

<span data-ttu-id="0b75c-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0b75c-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0b75c-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b75c-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b75c-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0b75c-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b75c-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b75c-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b75c-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b75c-145">Schema Name</span></span>  <br/> |<span data-ttu-id="0b75c-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0b75c-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="0b75c-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b75c-147">Validation File</span></span>  <br/> |<span data-ttu-id="0b75c-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0b75c-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b75c-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0b75c-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0b75c-150">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0b75c-150">See also</span></span>



- [<span data-ttu-id="0b75c-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b75c-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

