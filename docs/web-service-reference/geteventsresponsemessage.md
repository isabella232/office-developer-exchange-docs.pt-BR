---
title: GetEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEventsResponseMessage
api_type:
- schema
ms.assetid: d433977f-b86a-499e-b9c3-f405ac229358
description: O elemento GetEventsResponseMessage contém o status e o resultado de uma única solicitação de operação GetEvents.
ms.openlocfilehash: 90e79194182f61ba7298ef67b1070b1aa239073d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752483"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="23468-103">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="23468-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="23468-104">O elemento **GetEventsResponseMessage** contém o status e o resultado de uma única [operação GetEvents](getevents-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="23468-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="23468-105">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="23468-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23468-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="23468-106">Attributes and elements</span></span>

<span data-ttu-id="23468-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="23468-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23468-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="23468-108">Attributes</span></span>

|<span data-ttu-id="23468-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="23468-109">**Attribute**</span></span>|<span data-ttu-id="23468-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23468-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23468-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="23468-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="23468-112">Descreve o status de uma resposta [GetEvents operação](getevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="23468-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="23468-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="23468-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="23468-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="23468-114">-  Success</span></span>  <br/><span data-ttu-id="23468-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="23468-115">-  Warning</span></span>  <br/><span data-ttu-id="23468-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="23468-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="23468-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="23468-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="23468-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="23468-118">**Value**</span></span>|<span data-ttu-id="23468-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23468-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="23468-120">Êxito</span><span class="sxs-lookup"><span data-stu-id="23468-120">Success</span></span>  <br/> |<span data-ttu-id="23468-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="23468-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="23468-122">Aviso</span><span class="sxs-lookup"><span data-stu-id="23468-122">Warning</span></span>  <br/> | <span data-ttu-id="23468-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="23468-123">Describes a request that was not processed.</span></span> <span data-ttu-id="23468-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="23468-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="23468-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="23468-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="23468-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="23468-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="23468-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="23468-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="23468-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="23468-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="23468-129">-O banco de dados de caixa de correio (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="23468-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="23468-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="23468-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="23468-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="23468-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="23468-132">Erro</span><span class="sxs-lookup"><span data-stu-id="23468-132">Error</span></span>  <br/> | <span data-ttu-id="23468-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="23468-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="23468-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="23468-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="23468-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="23468-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="23468-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="23468-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="23468-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="23468-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="23468-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="23468-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="23468-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="23468-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="23468-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="23468-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="23468-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="23468-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="23468-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="23468-142">Child elements</span></span>

|<span data-ttu-id="23468-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="23468-143">**Element**</span></span>|<span data-ttu-id="23468-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23468-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23468-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="23468-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="23468-146">Fornece a descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="23468-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="23468-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="23468-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="23468-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="23468-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="23468-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="23468-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="23468-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="23468-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="23468-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="23468-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="23468-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="23468-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="23468-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="23468-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="23468-154">Notificação</span><span class="sxs-lookup"><span data-stu-id="23468-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="23468-155">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="23468-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23468-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="23468-156">Parent elements</span></span>

|<span data-ttu-id="23468-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="23468-157">**Element**</span></span>|<span data-ttu-id="23468-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="23468-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23468-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="23468-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="23468-160">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="23468-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="23468-161">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="23468-161">Remarks</span></span>

<span data-ttu-id="23468-162">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="23468-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23468-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="23468-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23468-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="23468-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23468-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="23468-165">Schema Name</span></span>  <br/> |<span data-ttu-id="23468-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="23468-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="23468-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="23468-167">Validation File</span></span>  <br/> |<span data-ttu-id="23468-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="23468-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23468-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="23468-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="23468-170">False</span><span class="sxs-lookup"><span data-stu-id="23468-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23468-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="23468-171">See also</span></span>

- [<span data-ttu-id="23468-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="23468-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="23468-173">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="23468-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="23468-174">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="23468-174">GetEvents operation</span></span>](getevents-operation.md)

