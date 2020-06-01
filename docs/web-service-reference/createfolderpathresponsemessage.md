---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: O elemento CreateFolderPathResponseMessage especifica a mensagem de resposta para uma solicitação createfolderpath.
ms.openlocfilehash: 3c0c4e98b568a6398dcd0e71a6e6931a3f47e3da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458884"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="a704f-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a704f-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="a704f-104">O elemento **CreateFolderPathResponseMessage** especifica a mensagem de resposta para uma solicitação **createfolderpath** .</span><span class="sxs-lookup"><span data-stu-id="a704f-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="a704f-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a704f-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a704f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a704f-106">Attributes and elements</span></span>

<span data-ttu-id="a704f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a704f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a704f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a704f-108">Attributes</span></span>

|<span data-ttu-id="a704f-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a704f-109">**Attribute**</span></span>|<span data-ttu-id="a704f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a704f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a704f-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a704f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="a704f-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="a704f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="a704f-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a704f-113">ResponseClass</span></span>

|<span data-ttu-id="a704f-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a704f-114">**Value**</span></span>|<span data-ttu-id="a704f-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a704f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a704f-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="a704f-116">Success</span></span>  <br/> |<span data-ttu-id="a704f-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="a704f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="a704f-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="a704f-118">Warning</span></span>  <br/> |<span data-ttu-id="a704f-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="a704f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="a704f-120">Erro</span><span class="sxs-lookup"><span data-stu-id="a704f-120">Error</span></span>  <br/> |<span data-ttu-id="a704f-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="a704f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a704f-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a704f-122">Child elements</span></span>

|<span data-ttu-id="a704f-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a704f-123">**Element**</span></span>|<span data-ttu-id="a704f-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a704f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a704f-125">Pastas</span><span class="sxs-lookup"><span data-stu-id="a704f-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a704f-126">Contém uma matriz de pastas que são usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="a704f-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="a704f-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a704f-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a704f-128">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="a704f-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="a704f-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="a704f-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a704f-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="a704f-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a704f-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a704f-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a704f-132">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="a704f-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a704f-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a704f-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a704f-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a704f-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a704f-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a704f-135">Parent elements</span></span>

|<span data-ttu-id="a704f-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a704f-136">**Element**</span></span>|<span data-ttu-id="a704f-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a704f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a704f-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a704f-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a704f-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a704f-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a704f-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="a704f-140">Remarks</span></span>

<span data-ttu-id="a704f-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a704f-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a704f-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a704f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a704f-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a704f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a704f-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="a704f-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a704f-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a704f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="a704f-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a704f-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="a704f-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a704f-147">Validation File</span></span>  <br/> |<span data-ttu-id="a704f-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a704f-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a704f-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a704f-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a704f-150">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a704f-150">See also</span></span>

- [<span data-ttu-id="a704f-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a704f-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

