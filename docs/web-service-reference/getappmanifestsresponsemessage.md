---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: O elemento GetAppManifestsResponseMessage Especifica a mensagem de resposta para uma solicitação de GetAppManifests.
ms.openlocfilehash: 05eeef7f7194c1dc05be93ed13ebff93d5013e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752400"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="0ea6f-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ea6f-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="0ea6f-104">O elemento **GetAppManifestsResponseMessage** Especifica a mensagem de resposta para uma solicitação de **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="0ea6f-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="0ea6f-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ea6f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0ea6f-106">Attributes and elements</span></span>

<span data-ttu-id="0ea6f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ea6f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0ea6f-108">Attributes</span></span>

|<span data-ttu-id="0ea6f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-109">**Attribute**</span></span>|<span data-ttu-id="0ea6f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ea6f-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0ea6f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="0ea6f-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="0ea6f-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0ea6f-113">ResponseClass</span></span>

|<span data-ttu-id="0ea6f-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-114">**Value**</span></span>|<span data-ttu-id="0ea6f-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ea6f-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="0ea6f-116">Success</span></span>  <br/> |<span data-ttu-id="0ea6f-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="0ea6f-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="0ea6f-118">Warning</span></span>  <br/> |<span data-ttu-id="0ea6f-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="0ea6f-120">Erro</span><span class="sxs-lookup"><span data-stu-id="0ea6f-120">Error</span></span>  <br/> |<span data-ttu-id="0ea6f-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0ea6f-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0ea6f-122">Child elements</span></span>

|<span data-ttu-id="0ea6f-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-123">**Element**</span></span>|<span data-ttu-id="0ea6f-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ea6f-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ea6f-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0ea6f-126">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="0ea6f-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ea6f-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0ea6f-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0ea6f-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0ea6f-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0ea6f-130">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0ea6f-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ea6f-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0ea6f-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ea6f-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0ea6f-133">Parent elements</span></span>

|<span data-ttu-id="0ea6f-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-134">**Element**</span></span>|<span data-ttu-id="0ea6f-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ea6f-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ea6f-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ea6f-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0ea6f-137">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ea6f-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ea6f-138">Remarks</span></span>

<span data-ttu-id="0ea6f-139">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0ea6f-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ea6f-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ea6f-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0ea6f-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ea6f-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ea6f-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ea6f-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0ea6f-143">Schema Name</span></span>  <br/> |<span data-ttu-id="0ea6f-144">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="0ea6f-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="0ea6f-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0ea6f-145">Validation File</span></span>  <br/> |<span data-ttu-id="0ea6f-146">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ea6f-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ea6f-147">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0ea6f-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0ea6f-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="0ea6f-148">See also</span></span>



- [<span data-ttu-id="0ea6f-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0ea6f-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

