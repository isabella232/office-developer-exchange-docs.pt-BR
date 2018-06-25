---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: O elemento InstallAppResponse Especifica a resposta a uma solicitação InstallApp.
ms.openlocfilehash: 8e8da720b3a38e979b3d83810bb798350822146c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823942"
---
# <a name="installappresponse"></a><span data-ttu-id="7e03a-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7e03a-103">InstallAppResponse</span></span>

<span data-ttu-id="7e03a-104">O elemento **InstallAppResponse** Especifica a resposta a uma solicitação **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7e03a-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="7e03a-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="7e03a-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e03a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e03a-106">Attributes and elements</span></span>

<span data-ttu-id="7e03a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e03a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e03a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e03a-108">Attributes</span></span>

|<span data-ttu-id="7e03a-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7e03a-109">**Attribute**</span></span>|<span data-ttu-id="7e03a-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e03a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e03a-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7e03a-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="7e03a-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e03a-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="7e03a-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7e03a-113">ResponseClass</span></span>

|<span data-ttu-id="7e03a-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7e03a-114">**Value**</span></span>|<span data-ttu-id="7e03a-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e03a-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e03a-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="7e03a-116">Success</span></span>  <br/> |<span data-ttu-id="7e03a-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="7e03a-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="7e03a-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="7e03a-118">Warning</span></span>  <br/> |<span data-ttu-id="7e03a-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="7e03a-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="7e03a-120">Erro</span><span class="sxs-lookup"><span data-stu-id="7e03a-120">Error</span></span>  <br/> |<span data-ttu-id="7e03a-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="7e03a-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e03a-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e03a-122">Child elements</span></span>

|<span data-ttu-id="7e03a-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e03a-123">**Element**</span></span>|<span data-ttu-id="7e03a-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e03a-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e03a-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e03a-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7e03a-126">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="7e03a-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="7e03a-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e03a-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7e03a-128">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e03a-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7e03a-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7e03a-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7e03a-130">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="7e03a-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7e03a-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e03a-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7e03a-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e03a-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e03a-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e03a-133">Parent elements</span></span>

|<span data-ttu-id="7e03a-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e03a-134">**Element**</span></span>|<span data-ttu-id="7e03a-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e03a-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e03a-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7e03a-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7e03a-137">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e03a-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e03a-138">Text value</span><span class="sxs-lookup"><span data-stu-id="7e03a-138">Text value</span></span>

<span data-ttu-id="7e03a-139">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e03a-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e03a-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="7e03a-140">Remarks</span></span>

<span data-ttu-id="7e03a-141">O elemento **GetAppManifestsResponseMessage** é aplicável para clientes que visam o Exchange Online e versões do Microsoft Exchange Server, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="7e03a-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7e03a-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e03a-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e03a-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e03a-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e03a-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e03a-144">Schema Name</span></span>  <br/> |<span data-ttu-id="7e03a-145">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="7e03a-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="7e03a-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e03a-146">Validation File</span></span>  <br/> |<span data-ttu-id="7e03a-147">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e03a-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e03a-148">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7e03a-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7e03a-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="7e03a-149">See also</span></span>



- [<span data-ttu-id="7e03a-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e03a-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

