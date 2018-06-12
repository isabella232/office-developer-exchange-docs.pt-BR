---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: O elemento GetStreamingEventsResponseMessage contém o status e o resultado de uma única solicitação de operação GetStreamingEvents.
ms.openlocfilehash: 5fcc7ddde41b49a5d8b304da0732f4472c61a76a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823682"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="408aa-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="408aa-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="408aa-104">O elemento **GetStreamingEventsResponseMessage** contém o status e o resultado de uma única solicitação de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="408aa-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 <span data-ttu-id="408aa-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="408aa-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="408aa-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="408aa-106">Attributes and elements</span></span>

<span data-ttu-id="408aa-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="408aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="408aa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="408aa-108">Attributes</span></span>

|<span data-ttu-id="408aa-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="408aa-109">**Attribute**</span></span>|<span data-ttu-id="408aa-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408aa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="408aa-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="408aa-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="408aa-112">Descreve o status de uma resposta de [operação GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="408aa-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="408aa-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="408aa-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="408aa-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="408aa-114">-  Success</span></span>  <br/><span data-ttu-id="408aa-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="408aa-115">-  Warning</span></span>  <br/><span data-ttu-id="408aa-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="408aa-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="408aa-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="408aa-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="408aa-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="408aa-118">**Value**</span></span>|<span data-ttu-id="408aa-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408aa-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="408aa-120">Êxito</span><span class="sxs-lookup"><span data-stu-id="408aa-120">Success</span></span>  <br/> |<span data-ttu-id="408aa-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="408aa-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="408aa-122">Aviso</span><span class="sxs-lookup"><span data-stu-id="408aa-122">Warning</span></span>  <br/> | <span data-ttu-id="408aa-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="408aa-123">Describes a request that was not processed.</span></span> <span data-ttu-id="408aa-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="408aa-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="408aa-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="408aa-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="408aa-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="408aa-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="408aa-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="408aa-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="408aa-128">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="408aa-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="408aa-129">-O banco de dados de caixa de correio (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="408aa-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="408aa-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="408aa-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="408aa-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="408aa-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="408aa-132">Erro</span><span class="sxs-lookup"><span data-stu-id="408aa-132">Error</span></span>  <br/> | <span data-ttu-id="408aa-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="408aa-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="408aa-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="408aa-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="408aa-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="408aa-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="408aa-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="408aa-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="408aa-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="408aa-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="408aa-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="408aa-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="408aa-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="408aa-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="408aa-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="408aa-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="408aa-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="408aa-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="408aa-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="408aa-142">Child elements</span></span>

|<span data-ttu-id="408aa-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="408aa-143">**Element**</span></span>|<span data-ttu-id="408aa-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408aa-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="408aa-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="408aa-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="408aa-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="408aa-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="408aa-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="408aa-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="408aa-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="408aa-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="408aa-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="408aa-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="408aa-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="408aa-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="408aa-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="408aa-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="408aa-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="408aa-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="408aa-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="408aa-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="408aa-154">Notificações</span><span class="sxs-lookup"><span data-stu-id="408aa-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="408aa-155">Contém uma lista de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="408aa-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="408aa-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="408aa-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="408aa-157">Contém uma lista de assinatura IDs são inválidos.</span><span class="sxs-lookup"><span data-stu-id="408aa-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="408aa-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="408aa-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="408aa-159">Fornece uma descrição de texto do status de uma assinatura de streaming.</span><span class="sxs-lookup"><span data-stu-id="408aa-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="408aa-160">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="408aa-160">Parent elements</span></span>

|<span data-ttu-id="408aa-161">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="408aa-161">**Element**</span></span>|<span data-ttu-id="408aa-162">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="408aa-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="408aa-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="408aa-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="408aa-164">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="408aa-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="408aa-165">Text value</span><span class="sxs-lookup"><span data-stu-id="408aa-165">Text value</span></span>

<span data-ttu-id="408aa-166">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="408aa-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="408aa-167">Comentários</span><span class="sxs-lookup"><span data-stu-id="408aa-167">Remarks</span></span>

<span data-ttu-id="408aa-168">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="408aa-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="408aa-169">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="408aa-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="408aa-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="408aa-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="408aa-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="408aa-171">Schema Name</span></span>  <br/> |<span data-ttu-id="408aa-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="408aa-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="408aa-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="408aa-173">Validation File</span></span>  <br/> |<span data-ttu-id="408aa-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="408aa-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="408aa-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="408aa-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="408aa-176">False</span><span class="sxs-lookup"><span data-stu-id="408aa-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="408aa-177">Ver também</span><span class="sxs-lookup"><span data-stu-id="408aa-177">See also</span></span>

- [<span data-ttu-id="408aa-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="408aa-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="408aa-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="408aa-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="408aa-180">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="408aa-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

