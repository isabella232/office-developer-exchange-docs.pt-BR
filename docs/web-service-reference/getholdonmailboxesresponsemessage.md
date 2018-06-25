---
title: GetHoldOnMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7d0d90-d418-4ce9-8cea-afe8f14728c3
description: O elemento GetHoldOnMailboxesResponseMessage Especifica a mensagem de resposta para uma solicitação de GetHoldOnMailboxes.
ms.openlocfilehash: e1c43f75bfa62b20de9248546e71c92ae5998ed9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752518"
---
# <a name="getholdonmailboxesresponsemessage"></a><span data-ttu-id="19a02-103">GetHoldOnMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="19a02-103">GetHoldOnMailboxesResponseMessage</span></span>

<span data-ttu-id="19a02-104">O elemento **GetHoldOnMailboxesResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="19a02-104">The **GetHoldOnMailboxesResponseMessage** element specifies the response message for a **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxHoldResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetHoldOnMailboxesResponseMessage>
```

 <span data-ttu-id="19a02-105">**GetHoldOnMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="19a02-105">**GetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19a02-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="19a02-106">Attributes and elements</span></span>

<span data-ttu-id="19a02-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="19a02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19a02-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="19a02-108">Attributes</span></span>

|<span data-ttu-id="19a02-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="19a02-109">**Attribute**</span></span>|<span data-ttu-id="19a02-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19a02-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19a02-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="19a02-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="19a02-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a02-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="19a02-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="19a02-113">ResponseClass</span></span>

|<span data-ttu-id="19a02-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="19a02-114">**Value**</span></span>|<span data-ttu-id="19a02-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19a02-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="19a02-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="19a02-116">Success</span></span>  <br/> |<span data-ttu-id="19a02-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="19a02-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="19a02-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="19a02-118">Warning</span></span>  <br/> |<span data-ttu-id="19a02-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="19a02-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="19a02-120">Erro</span><span class="sxs-lookup"><span data-stu-id="19a02-120">Error</span></span>  <br/> |<span data-ttu-id="19a02-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="19a02-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="19a02-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="19a02-122">Child elements</span></span>

|<span data-ttu-id="19a02-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19a02-123">**Element**</span></span>|<span data-ttu-id="19a02-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19a02-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19a02-125">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="19a02-125">MailboxHoldResult</span></span>](mailboxholdresult.md) <br/> |<span data-ttu-id="19a02-126">Contém o resultado da solicitação **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="19a02-126">Contains the result of the **GetHoldOnMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="19a02-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="19a02-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="19a02-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="19a02-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="19a02-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="19a02-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="19a02-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a02-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="19a02-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="19a02-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="19a02-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="19a02-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="19a02-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="19a02-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="19a02-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a02-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19a02-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="19a02-135">Parent elements</span></span>

|<span data-ttu-id="19a02-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="19a02-136">**Element**</span></span>|<span data-ttu-id="19a02-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="19a02-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19a02-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="19a02-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="19a02-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="19a02-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="19a02-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="19a02-140">Remarks</span></span>

<span data-ttu-id="19a02-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="19a02-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="19a02-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="19a02-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19a02-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="19a02-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19a02-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="19a02-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19a02-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="19a02-145">Schema Name</span></span>  <br/> |<span data-ttu-id="19a02-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="19a02-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="19a02-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="19a02-147">Validation File</span></span>  <br/> |<span data-ttu-id="19a02-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19a02-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19a02-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="19a02-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="19a02-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="19a02-150">See also</span></span>



- [<span data-ttu-id="19a02-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="19a02-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

