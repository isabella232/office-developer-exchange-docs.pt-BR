---
title: GetSearchableMailboxesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f45865fd-4626-4d80-84f6-7989339fdd85
description: O elemento GetSearchableMailboxesResponseMessage Especifica a mensagem de resposta para uma solicitação de GetSearchableMailboxes.
ms.openlocfilehash: 2a4d1fe357656fe29d8572e7f32a4bc2e4a6131e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752626"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="50ca9-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="50ca9-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="50ca9-104">O elemento **GetSearchableMailboxesResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="50ca9-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="50ca9-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="50ca9-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50ca9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="50ca9-106">Attributes and elements</span></span>

<span data-ttu-id="50ca9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="50ca9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50ca9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="50ca9-108">Attributes</span></span>

|<span data-ttu-id="50ca9-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="50ca9-109">**Attribute**</span></span>|<span data-ttu-id="50ca9-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50ca9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50ca9-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="50ca9-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="50ca9-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="50ca9-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="50ca9-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="50ca9-113">ResponseClass</span></span>

|<span data-ttu-id="50ca9-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="50ca9-114">**Value**</span></span>|<span data-ttu-id="50ca9-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50ca9-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50ca9-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="50ca9-116">Success</span></span>  <br/> |<span data-ttu-id="50ca9-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="50ca9-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="50ca9-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="50ca9-118">Warning</span></span>  <br/> |<span data-ttu-id="50ca9-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="50ca9-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="50ca9-120">Erro</span><span class="sxs-lookup"><span data-stu-id="50ca9-120">Error</span></span>  <br/> |<span data-ttu-id="50ca9-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="50ca9-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="50ca9-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="50ca9-122">Child elements</span></span>

|<span data-ttu-id="50ca9-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50ca9-123">**Element**</span></span>|<span data-ttu-id="50ca9-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50ca9-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50ca9-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="50ca9-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="50ca9-126">Contém uma matriz das caixas de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="50ca9-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="50ca9-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="50ca9-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="50ca9-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="50ca9-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="50ca9-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="50ca9-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="50ca9-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="50ca9-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="50ca9-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="50ca9-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="50ca9-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="50ca9-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="50ca9-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50ca9-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="50ca9-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ca9-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50ca9-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="50ca9-135">Parent elements</span></span>

|<span data-ttu-id="50ca9-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50ca9-136">**Element**</span></span>|<span data-ttu-id="50ca9-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50ca9-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50ca9-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50ca9-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="50ca9-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="50ca9-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50ca9-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="50ca9-140">Remarks</span></span>

<span data-ttu-id="50ca9-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="50ca9-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="50ca9-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="50ca9-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50ca9-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="50ca9-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50ca9-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="50ca9-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50ca9-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="50ca9-145">Schema Name</span></span>  <br/> |<span data-ttu-id="50ca9-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="50ca9-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="50ca9-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="50ca9-147">Validation File</span></span>  <br/> |<span data-ttu-id="50ca9-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="50ca9-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50ca9-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="50ca9-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="50ca9-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="50ca9-150">See also</span></span>



- [<span data-ttu-id="50ca9-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50ca9-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

