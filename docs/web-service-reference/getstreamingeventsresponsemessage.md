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
description: O elemento GetStreamingEventsResponseMessage contém o status e o resultado de uma única solicitação de operação de GetStreamingEvents.
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459143"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="4aa65-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4aa65-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="4aa65-104">O elemento **GetStreamingEventsResponseMessage** contém o status e o resultado de uma única solicitação de [operação de GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4aa65-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="4aa65-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4aa65-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4aa65-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4aa65-106">Attributes and elements</span></span>

<span data-ttu-id="4aa65-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4aa65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4aa65-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4aa65-108">Attributes</span></span>

|<span data-ttu-id="4aa65-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="4aa65-109">**Attribute**</span></span>|<span data-ttu-id="4aa65-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa65-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4aa65-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4aa65-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4aa65-112">Descreve o status de uma resposta de [operação do GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4aa65-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4aa65-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="4aa65-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4aa65-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="4aa65-114">-  Success</span></span>  <br/><span data-ttu-id="4aa65-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="4aa65-115">-  Warning</span></span>  <br/><span data-ttu-id="4aa65-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="4aa65-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="4aa65-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4aa65-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="4aa65-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="4aa65-118">**Value**</span></span>|<span data-ttu-id="4aa65-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa65-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4aa65-120">Êxito</span><span class="sxs-lookup"><span data-stu-id="4aa65-120">Success</span></span>  <br/> |<span data-ttu-id="4aa65-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="4aa65-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4aa65-122">Aviso</span><span class="sxs-lookup"><span data-stu-id="4aa65-122">Warning</span></span>  <br/> | <span data-ttu-id="4aa65-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="4aa65-123">Describes a request that was not processed.</span></span> <span data-ttu-id="4aa65-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="4aa65-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4aa65-125">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="4aa65-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4aa65-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="4aa65-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4aa65-127">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="4aa65-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4aa65-128">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="4aa65-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="4aa65-129">– O banco de dados de caixa de correio (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="4aa65-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4aa65-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="4aa65-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="4aa65-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="4aa65-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="4aa65-132">Erro</span><span class="sxs-lookup"><span data-stu-id="4aa65-132">Error</span></span>  <br/> | <span data-ttu-id="4aa65-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="4aa65-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4aa65-134">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="4aa65-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4aa65-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="4aa65-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4aa65-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="4aa65-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="4aa65-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="4aa65-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="4aa65-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="4aa65-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4aa65-139">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="4aa65-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4aa65-140">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="4aa65-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4aa65-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4aa65-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4aa65-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4aa65-142">Child elements</span></span>

|<span data-ttu-id="4aa65-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4aa65-143">**Element**</span></span>|<span data-ttu-id="4aa65-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa65-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aa65-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="4aa65-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4aa65-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="4aa65-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4aa65-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4aa65-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="4aa65-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4aa65-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4aa65-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="4aa65-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4aa65-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="4aa65-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4aa65-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4aa65-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="4aa65-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-154">Notificações</span><span class="sxs-lookup"><span data-stu-id="4aa65-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="4aa65-155">Contém uma lista de informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="4aa65-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="4aa65-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="4aa65-157">Contém uma lista de IDs de assinatura que são inválidas.</span><span class="sxs-lookup"><span data-stu-id="4aa65-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="4aa65-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="4aa65-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="4aa65-159">Fornece uma descrição de texto do status de uma assinatura de streaming.</span><span class="sxs-lookup"><span data-stu-id="4aa65-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4aa65-160">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4aa65-160">Parent elements</span></span>

|<span data-ttu-id="4aa65-161">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4aa65-161">**Element**</span></span>|<span data-ttu-id="4aa65-162">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4aa65-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aa65-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4aa65-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4aa65-164">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4aa65-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4aa65-165">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="4aa65-165">Text value</span></span>

<span data-ttu-id="4aa65-166">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4aa65-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4aa65-167">Comentários</span><span class="sxs-lookup"><span data-stu-id="4aa65-167">Remarks</span></span>

<span data-ttu-id="4aa65-168">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4aa65-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4aa65-169">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4aa65-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4aa65-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="4aa65-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4aa65-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4aa65-171">Schema Name</span></span>  <br/> |<span data-ttu-id="4aa65-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4aa65-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4aa65-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4aa65-173">Validation File</span></span>  <br/> |<span data-ttu-id="4aa65-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4aa65-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4aa65-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4aa65-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="4aa65-176">False</span><span class="sxs-lookup"><span data-stu-id="4aa65-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4aa65-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="4aa65-177">See also</span></span>

- [<span data-ttu-id="4aa65-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="4aa65-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="4aa65-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="4aa65-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="4aa65-180">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="4aa65-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

