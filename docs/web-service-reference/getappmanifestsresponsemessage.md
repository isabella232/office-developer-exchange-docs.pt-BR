---
title: GetAppManifestsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 815908f1-4223-42d8-92dc-f8bdfc6b5df8
description: O elemento GetAppManifestsResponseMessage especifica a mensagem de resposta para uma solicitação GetAppManifests.
ms.openlocfilehash: 26a521d8647a010fe956596eaf63d4df4756edb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459529"
---
# <a name="getappmanifestsresponsemessage"></a><span data-ttu-id="ce272-103">GetAppManifestsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce272-103">GetAppManifestsResponseMessage</span></span>

<span data-ttu-id="ce272-104">O elemento **GetAppManifestsResponseMessage** especifica a mensagem de resposta para uma solicitação **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="ce272-104">The **GetAppManifestsResponseMessage** element specifies the response message for a **GetAppManifests** request.</span></span> 
  
```XML
<GetAppManifestsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppManifestsResponseMessage>
```

 <span data-ttu-id="ce272-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ce272-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce272-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ce272-106">Attributes and elements</span></span>

<span data-ttu-id="ce272-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ce272-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce272-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ce272-108">Attributes</span></span>

|<span data-ttu-id="ce272-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ce272-109">**Attribute**</span></span>|<span data-ttu-id="ce272-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce272-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce272-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ce272-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="ce272-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce272-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="ce272-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="ce272-113">ResponseClass</span></span>

|<span data-ttu-id="ce272-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="ce272-114">**Value**</span></span>|<span data-ttu-id="ce272-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce272-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce272-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="ce272-116">Success</span></span>  <br/> |<span data-ttu-id="ce272-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="ce272-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="ce272-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="ce272-118">Warning</span></span>  <br/> |<span data-ttu-id="ce272-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="ce272-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="ce272-120">Erro</span><span class="sxs-lookup"><span data-stu-id="ce272-120">Error</span></span>  <br/> |<span data-ttu-id="ce272-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="ce272-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ce272-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ce272-122">Child elements</span></span>

|<span data-ttu-id="ce272-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce272-123">**Element**</span></span>|<span data-ttu-id="ce272-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce272-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce272-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ce272-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ce272-126">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="ce272-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="ce272-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="ce272-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ce272-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce272-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ce272-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ce272-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ce272-130">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="ce272-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ce272-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce272-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ce272-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce272-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce272-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ce272-133">Parent elements</span></span>

|<span data-ttu-id="ce272-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce272-134">**Element**</span></span>|<span data-ttu-id="ce272-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce272-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce272-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce272-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ce272-137">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce272-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce272-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce272-138">Remarks</span></span>

<span data-ttu-id="ce272-139">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ce272-139">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ce272-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce272-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce272-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ce272-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce272-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce272-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce272-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ce272-143">Schema Name</span></span>  <br/> |<span data-ttu-id="ce272-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ce272-144">Message schema</span></span>  <br/> |
|<span data-ttu-id="ce272-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ce272-145">Validation File</span></span>  <br/> |<span data-ttu-id="ce272-146">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ce272-146">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce272-147">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ce272-147">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ce272-148">Também consulte</span><span class="sxs-lookup"><span data-stu-id="ce272-148">See also</span></span>



- [<span data-ttu-id="ce272-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce272-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

