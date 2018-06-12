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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752626"
---
# <a name="getsearchablemailboxesresponsemessage"></a><span data-ttu-id="23773-103">GetSearchableMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="23773-103">GetSearchableMailboxesResponseMessage</span></span>

<span data-ttu-id="23773-104">O elemento **GetSearchableMailboxesResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="23773-104">The **GetSearchableMailboxesResponseMessage** element specifies the response message for a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponseMessage ResponseClass=" Success | Warning | Error ">
    <SearchableMailboxes/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetSearchablemailboxesResponseMessage>
```

 <span data-ttu-id="23773-105">**GetSearchableMailboxesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="23773-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23773-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="23773-106">Attributes and elements</span></span>

<span data-ttu-id="23773-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="23773-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23773-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="23773-108">Attributes</span></span>

|<span data-ttu-id="23773-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="23773-109">**Attribute**</span></span>|<span data-ttu-id="23773-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23773-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23773-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="23773-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="23773-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="23773-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="23773-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="23773-113">ResponseClass</span></span>

|<span data-ttu-id="23773-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="23773-114">**Value**</span></span>|<span data-ttu-id="23773-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23773-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23773-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="23773-116">Success</span></span>  <br/> |<span data-ttu-id="23773-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="23773-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="23773-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="23773-118">Warning</span></span>  <br/> |<span data-ttu-id="23773-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="23773-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="23773-120">Erro</span><span class="sxs-lookup"><span data-stu-id="23773-120">Error</span></span>  <br/> |<span data-ttu-id="23773-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="23773-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="23773-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="23773-122">Child elements</span></span>

|<span data-ttu-id="23773-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="23773-123">**Element**</span></span>|<span data-ttu-id="23773-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23773-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23773-125">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="23773-125">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="23773-126">Contém uma matriz das caixas de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="23773-126">Contains an array of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
|[<span data-ttu-id="23773-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="23773-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="23773-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="23773-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="23773-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="23773-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="23773-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="23773-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="23773-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="23773-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="23773-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="23773-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="23773-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="23773-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="23773-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="23773-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23773-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="23773-135">Parent elements</span></span>

|<span data-ttu-id="23773-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="23773-136">**Element**</span></span>|<span data-ttu-id="23773-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23773-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23773-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="23773-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="23773-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23773-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23773-140">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="23773-140">Remarks</span></span>

<span data-ttu-id="23773-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="23773-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23773-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23773-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23773-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="23773-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23773-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="23773-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23773-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="23773-145">Schema Name</span></span>  <br/> |<span data-ttu-id="23773-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="23773-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="23773-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="23773-147">Validation File</span></span>  <br/> |<span data-ttu-id="23773-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="23773-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23773-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="23773-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="23773-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="23773-150">See also</span></span>



- [<span data-ttu-id="23773-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="23773-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

