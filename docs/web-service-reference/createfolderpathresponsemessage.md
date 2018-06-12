---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: O elemento CreateFolderPathResponseMessage Especifica a mensagem de resposta para uma solicitação de CreateFolderPath.
ms.openlocfilehash: f8f85cc246bb5d5ecd5cb745267d9d373286cf7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751588"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="c0dda-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c0dda-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="c0dda-104">O elemento **CreateFolderPathResponseMessage** Especifica a mensagem de resposta para uma solicitação de **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="c0dda-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="c0dda-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c0dda-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0dda-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c0dda-106">Attributes and elements</span></span>

<span data-ttu-id="c0dda-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0dda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0dda-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0dda-108">Attributes</span></span>

|<span data-ttu-id="c0dda-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="c0dda-109">**Attribute**</span></span>|<span data-ttu-id="c0dda-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0dda-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0dda-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c0dda-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="c0dda-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0dda-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="c0dda-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c0dda-113">ResponseClass</span></span>

|<span data-ttu-id="c0dda-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c0dda-114">**Value**</span></span>|<span data-ttu-id="c0dda-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0dda-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0dda-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="c0dda-116">Success</span></span>  <br/> |<span data-ttu-id="c0dda-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="c0dda-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="c0dda-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="c0dda-118">Warning</span></span>  <br/> |<span data-ttu-id="c0dda-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="c0dda-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="c0dda-120">Erro</span><span class="sxs-lookup"><span data-stu-id="c0dda-120">Error</span></span>  <br/> |<span data-ttu-id="c0dda-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="c0dda-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c0dda-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0dda-122">Child elements</span></span>

|<span data-ttu-id="c0dda-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0dda-123">**Element**</span></span>|<span data-ttu-id="c0dda-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0dda-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0dda-125">Pastas</span><span class="sxs-lookup"><span data-stu-id="c0dda-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c0dda-126">Contém uma matriz das pastas que são usadas nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="c0dda-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="c0dda-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c0dda-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c0dda-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c0dda-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c0dda-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="c0dda-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c0dda-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0dda-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c0dda-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c0dda-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c0dda-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="c0dda-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c0dda-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0dda-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c0dda-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0dda-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0dda-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0dda-135">Parent elements</span></span>

|<span data-ttu-id="c0dda-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0dda-136">**Element**</span></span>|<span data-ttu-id="c0dda-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0dda-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0dda-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0dda-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c0dda-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0dda-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0dda-140">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c0dda-140">Remarks</span></span>

<span data-ttu-id="c0dda-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c0dda-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c0dda-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0dda-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0dda-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c0dda-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0dda-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0dda-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c0dda-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0dda-145">Schema Name</span></span>  <br/> |<span data-ttu-id="c0dda-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="c0dda-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="c0dda-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0dda-147">Validation File</span></span>  <br/> |<span data-ttu-id="c0dda-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0dda-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0dda-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c0dda-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c0dda-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="c0dda-150">See also</span></span>

- [<span data-ttu-id="c0dda-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c0dda-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

