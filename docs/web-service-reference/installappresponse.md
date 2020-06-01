---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: O elemento InstallAppResponse especifica a resposta a uma solicitação InstallApp.
ms.openlocfilehash: 0f7690e2df7e71c4e478dec191671af24f96294b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465664"
---
# <a name="installappresponse"></a><span data-ttu-id="c0c32-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="c0c32-103">InstallAppResponse</span></span>

<span data-ttu-id="c0c32-104">O elemento **InstallAppResponse** especifica a resposta a uma solicitação **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="c0c32-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="c0c32-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="c0c32-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0c32-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c0c32-106">Attributes and elements</span></span>

<span data-ttu-id="c0c32-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0c32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0c32-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0c32-108">Attributes</span></span>

|<span data-ttu-id="c0c32-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="c0c32-109">**Attribute**</span></span>|<span data-ttu-id="c0c32-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0c32-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0c32-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c0c32-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="c0c32-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0c32-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="c0c32-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c0c32-113">ResponseClass</span></span>

|<span data-ttu-id="c0c32-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c0c32-114">**Value**</span></span>|<span data-ttu-id="c0c32-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0c32-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0c32-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="c0c32-116">Success</span></span>  <br/> |<span data-ttu-id="c0c32-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="c0c32-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="c0c32-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="c0c32-118">Warning</span></span>  <br/> |<span data-ttu-id="c0c32-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="c0c32-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="c0c32-120">Erro</span><span class="sxs-lookup"><span data-stu-id="c0c32-120">Error</span></span>  <br/> |<span data-ttu-id="c0c32-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="c0c32-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c0c32-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0c32-122">Child elements</span></span>

|<span data-ttu-id="c0c32-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0c32-123">**Element**</span></span>|<span data-ttu-id="c0c32-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0c32-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0c32-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c0c32-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c0c32-126">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c0c32-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c0c32-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="c0c32-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c0c32-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0c32-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c0c32-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c0c32-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c0c32-130">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="c0c32-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c0c32-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0c32-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c0c32-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0c32-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0c32-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0c32-133">Parent elements</span></span>

|<span data-ttu-id="c0c32-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0c32-134">**Element**</span></span>|<span data-ttu-id="c0c32-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0c32-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0c32-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0c32-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c0c32-137">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0c32-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0c32-138">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c0c32-138">Text value</span></span>

<span data-ttu-id="c0c32-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c0c32-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0c32-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0c32-140">Remarks</span></span>

<span data-ttu-id="c0c32-141">O elemento **GetAppManifestsResponseMessage** é aplicável para clientes que direcionam o Exchange Online e versões do Microsoft Exchange Server a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c0c32-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="c0c32-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c0c32-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0c32-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0c32-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c0c32-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0c32-144">Schema Name</span></span>  <br/> |<span data-ttu-id="c0c32-145">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c0c32-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="c0c32-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0c32-146">Validation File</span></span>  <br/> |<span data-ttu-id="c0c32-147">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c0c32-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0c32-148">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c0c32-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c0c32-149">Também consulte</span><span class="sxs-lookup"><span data-stu-id="c0c32-149">See also</span></span>



- [<span data-ttu-id="c0c32-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c0c32-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

