---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: O elemento GetClientAccessTokenResponseMessage Especifica a mensagem de resposta para uma solicitação de GetClientAccessToken.
ms.openlocfilehash: 16fe684dd48f77156ed88d02a6ae7b8f3312cd87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752424"
---
# <a name="getclientaccesstokenresponsemessage"></a><span data-ttu-id="7c5be-103">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7c5be-103">GetClientAccessTokenResponseMessage</span></span>

<span data-ttu-id="7c5be-104">O elemento **GetClientAccessTokenResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="7c5be-104">The **GetClientAccessTokenResponseMessage** element specifies the response message for a **GetClientAccessToken** request.</span></span> 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 <span data-ttu-id="7c5be-105">**GetClientAccessTokenResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7c5be-105">**GetClientAccessTokenResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c5be-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7c5be-106">Attributes and elements</span></span>

<span data-ttu-id="7c5be-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7c5be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c5be-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7c5be-108">Attributes</span></span>

|<span data-ttu-id="7c5be-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7c5be-109">**Attribute**</span></span>|<span data-ttu-id="7c5be-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c5be-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c5be-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7c5be-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="7c5be-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c5be-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="7c5be-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7c5be-113">ResponseClass</span></span>

|<span data-ttu-id="7c5be-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7c5be-114">**Value**</span></span>|<span data-ttu-id="7c5be-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c5be-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c5be-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="7c5be-116">Success</span></span>  <br/> |<span data-ttu-id="7c5be-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="7c5be-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="7c5be-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="7c5be-118">Warning</span></span>  <br/> |<span data-ttu-id="7c5be-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="7c5be-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="7c5be-120">Erro</span><span class="sxs-lookup"><span data-stu-id="7c5be-120">Error</span></span>  <br/> |<span data-ttu-id="7c5be-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="7c5be-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7c5be-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7c5be-122">Child elements</span></span>

|<span data-ttu-id="7c5be-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c5be-123">**Element**</span></span>|<span data-ttu-id="7c5be-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c5be-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c5be-125">Token (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="7c5be-125">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md) <br/> |<span data-ttu-id="7c5be-126">Especifica um token de acesso do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c5be-126">Specifies a client access token.</span></span>  <br/> |
|[<span data-ttu-id="7c5be-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7c5be-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7c5be-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="7c5be-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="7c5be-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="7c5be-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7c5be-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c5be-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7c5be-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7c5be-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7c5be-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="7c5be-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7c5be-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7c5be-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7c5be-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c5be-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c5be-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7c5be-135">Parent elements</span></span>

|<span data-ttu-id="7c5be-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7c5be-136">**Element**</span></span>|<span data-ttu-id="7c5be-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7c5be-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c5be-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7c5be-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7c5be-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="7c5be-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c5be-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="7c5be-140">Remarks</span></span>

<span data-ttu-id="7c5be-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7c5be-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c5be-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c5be-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c5be-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7c5be-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c5be-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c5be-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c5be-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7c5be-145">Schema Name</span></span>  <br/> |<span data-ttu-id="7c5be-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="7c5be-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="7c5be-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7c5be-147">Validation File</span></span>  <br/> |<span data-ttu-id="7c5be-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c5be-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c5be-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7c5be-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7c5be-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="7c5be-150">See also</span></span>



- [<span data-ttu-id="7c5be-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7c5be-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

