---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: O elemento FindPeopleResponse especifica a resposta a uma solicitação FindPeople.
ms.openlocfilehash: b969ac3f7bc2bbd3fc77bf753a15696c3b6d8216
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466399"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="97493-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="97493-103">FindPeopleResponse</span></span>

<span data-ttu-id="97493-104">O elemento **FindPeopleResponse** especifica a resposta a uma solicitação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="97493-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 <span data-ttu-id="97493-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="97493-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97493-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="97493-106">Attributes and elements</span></span>

<span data-ttu-id="97493-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97493-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97493-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97493-108">Attributes</span></span>

|<span data-ttu-id="97493-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="97493-109">**Attribute**</span></span>|<span data-ttu-id="97493-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97493-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97493-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="97493-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="97493-112">Especifica a classe de resposta.</span><span class="sxs-lookup"><span data-stu-id="97493-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="97493-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="97493-113">ResponseClass</span></span>

|<span data-ttu-id="97493-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="97493-114">**Value**</span></span>|<span data-ttu-id="97493-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97493-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="97493-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="97493-116">Success</span></span>  <br/> |<span data-ttu-id="97493-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="97493-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="97493-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="97493-118">Warning</span></span>  <br/> |<span data-ttu-id="97493-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="97493-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="97493-120">Erro</span><span class="sxs-lookup"><span data-stu-id="97493-120">Error</span></span>  <br/> |<span data-ttu-id="97493-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="97493-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="97493-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97493-122">Child elements</span></span>

|<span data-ttu-id="97493-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97493-123">**Element**</span></span>|<span data-ttu-id="97493-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97493-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97493-125">Pessoas</span><span class="sxs-lookup"><span data-stu-id="97493-125">People</span></span>](people.md) <br/> |<span data-ttu-id="97493-126">Especifica uma matriz de dados persona retornados como resultado de uma solicitação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="97493-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="97493-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="97493-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="97493-128">Especifica o número total de pessoas armazenadas em um servidor retornado por uma solicitação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="97493-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="97493-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="97493-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="97493-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="97493-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="97493-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="97493-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="97493-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="97493-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="97493-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="97493-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="97493-134">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="97493-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="97493-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="97493-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="97493-136">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="97493-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97493-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97493-137">Parent elements</span></span>

|<span data-ttu-id="97493-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97493-138">**Element**</span></span>|<span data-ttu-id="97493-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97493-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97493-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="97493-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="97493-141">Especifica uma matriz de mensagens de resposta.</span><span class="sxs-lookup"><span data-stu-id="97493-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97493-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="97493-142">Remarks</span></span>

<span data-ttu-id="97493-143">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97493-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97493-144">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="97493-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97493-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="97493-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97493-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="97493-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97493-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97493-147">Schema Name</span></span>  <br/> |<span data-ttu-id="97493-148">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="97493-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="97493-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97493-149">Validation File</span></span>  <br/> |<span data-ttu-id="97493-150">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="97493-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97493-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="97493-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="97493-152">Também consulte</span><span class="sxs-lookup"><span data-stu-id="97493-152">See also</span></span>



- [<span data-ttu-id="97493-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="97493-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

