---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: O elemento FindPeopleResponse Especifica a resposta a uma solicitação FindPeople.
ms.openlocfilehash: 4f2c2f6069a515d5153ea488b35182d8b35f029f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752301"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="298de-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="298de-103">FindPeopleResponse</span></span>

<span data-ttu-id="298de-104">O elemento **FindPeopleResponse** Especifica a resposta a uma solicitação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="298de-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="298de-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="298de-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="298de-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="298de-106">Attributes and elements</span></span>

<span data-ttu-id="298de-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="298de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="298de-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="298de-108">Attributes</span></span>

|<span data-ttu-id="298de-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="298de-109">**Attribute**</span></span>|<span data-ttu-id="298de-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="298de-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="298de-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="298de-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="298de-112">Especifica a classe de resposta.</span><span class="sxs-lookup"><span data-stu-id="298de-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="298de-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="298de-113">ResponseClass</span></span>

|<span data-ttu-id="298de-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="298de-114">**Value**</span></span>|<span data-ttu-id="298de-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="298de-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="298de-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="298de-116">Success</span></span>  <br/> |<span data-ttu-id="298de-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="298de-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="298de-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="298de-118">Warning</span></span>  <br/> |<span data-ttu-id="298de-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="298de-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="298de-120">Erro</span><span class="sxs-lookup"><span data-stu-id="298de-120">Error</span></span>  <br/> |<span data-ttu-id="298de-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="298de-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="298de-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="298de-122">Child elements</span></span>

|<span data-ttu-id="298de-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="298de-123">**Element**</span></span>|<span data-ttu-id="298de-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="298de-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="298de-125">Pessoas</span><span class="sxs-lookup"><span data-stu-id="298de-125">People</span></span>](people.md) <br/> |<span data-ttu-id="298de-126">Especifica uma matriz de dados de pessoa retornados como o resultado de uma solicitação de **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="298de-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="298de-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="298de-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="298de-128">Especifica o número total de personagens armazenados em um servidor que são retornados por uma solicitação **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="298de-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="298de-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="298de-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="298de-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="298de-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="298de-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="298de-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="298de-132">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="298de-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="298de-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="298de-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="298de-134">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="298de-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="298de-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="298de-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="298de-136">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="298de-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="298de-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="298de-137">Parent elements</span></span>

|<span data-ttu-id="298de-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="298de-138">**Element**</span></span>|<span data-ttu-id="298de-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="298de-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="298de-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="298de-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="298de-141">Especifica uma matriz de mensagens de resposta.</span><span class="sxs-lookup"><span data-stu-id="298de-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="298de-142">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="298de-142">Remarks</span></span>

<span data-ttu-id="298de-143">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="298de-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="298de-144">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="298de-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="298de-145">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="298de-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="298de-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="298de-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="298de-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="298de-147">Schema Name</span></span>  <br/> |<span data-ttu-id="298de-148">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="298de-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="298de-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="298de-149">Validation File</span></span>  <br/> |<span data-ttu-id="298de-150">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="298de-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="298de-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="298de-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="298de-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="298de-152">See also</span></span>



- [<span data-ttu-id="298de-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="298de-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

