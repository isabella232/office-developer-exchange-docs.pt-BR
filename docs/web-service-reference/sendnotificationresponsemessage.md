---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: O elemento SendNotificationResponseMessage contém o status e o resultado de uma única solicitação de operação SendNotification.
ms.openlocfilehash: 49677b6d61f525b469679ec3fdcb8aadcca7239d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825348"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="47f9b-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="47f9b-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="47f9b-104">O elemento **SendNotificationResponseMessage** contém o status e o resultado de uma única solicitação de operação **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="47f9b-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="47f9b-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="47f9b-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47f9b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47f9b-106">Attributes and elements</span></span>

<span data-ttu-id="47f9b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47f9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47f9b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="47f9b-108">Attributes</span></span>

|<span data-ttu-id="47f9b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="47f9b-109">**Attribute**</span></span>|<span data-ttu-id="47f9b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f9b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="47f9b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="47f9b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="47f9b-112">Descreve o status de uma resposta de operação **SendNotification** .</span><span class="sxs-lookup"><span data-stu-id="47f9b-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="47f9b-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="47f9b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="47f9b-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="47f9b-114">-  Success</span></span>  <br/><span data-ttu-id="47f9b-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="47f9b-115">-  Warning</span></span>  <br/><span data-ttu-id="47f9b-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="47f9b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="47f9b-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="47f9b-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="47f9b-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="47f9b-118">**Value**</span></span>|<span data-ttu-id="47f9b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f9b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="47f9b-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="47f9b-120">**Success**</span></span> <br/> |<span data-ttu-id="47f9b-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="47f9b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="47f9b-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="47f9b-122">**Warning**</span></span> <br/> | <span data-ttu-id="47f9b-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="47f9b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="47f9b-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="47f9b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="47f9b-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="47f9b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="47f9b-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="47f9b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="47f9b-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="47f9b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="47f9b-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="47f9b-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="47f9b-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="47f9b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="47f9b-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="47f9b-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="47f9b-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="47f9b-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="47f9b-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="47f9b-132">**Error**</span></span> <br/> | <span data-ttu-id="47f9b-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="47f9b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="47f9b-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="47f9b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="47f9b-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="47f9b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="47f9b-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="47f9b-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="47f9b-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="47f9b-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="47f9b-138">-Atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="47f9b-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="47f9b-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="47f9b-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="47f9b-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="47f9b-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="47f9b-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="47f9b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="47f9b-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47f9b-142">Child elements</span></span>

|<span data-ttu-id="47f9b-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47f9b-143">**Element**</span></span>|<span data-ttu-id="47f9b-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f9b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f9b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="47f9b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="47f9b-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="47f9b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="47f9b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="47f9b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="47f9b-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="47f9b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="47f9b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="47f9b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="47f9b-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="47f9b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="47f9b-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="47f9b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="47f9b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="47f9b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="47f9b-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="47f9b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="47f9b-154">Notificação</span><span class="sxs-lookup"><span data-stu-id="47f9b-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="47f9b-155">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="47f9b-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47f9b-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47f9b-156">Parent elements</span></span>

|<span data-ttu-id="47f9b-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47f9b-157">**Element**</span></span>|<span data-ttu-id="47f9b-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f9b-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f9b-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="47f9b-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="47f9b-160">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="47f9b-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47f9b-161">Text value</span><span class="sxs-lookup"><span data-stu-id="47f9b-161">Text value</span></span>

<span data-ttu-id="47f9b-162">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47f9b-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47f9b-163">Comentários</span><span class="sxs-lookup"><span data-stu-id="47f9b-163">Remarks</span></span>

<span data-ttu-id="47f9b-164">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="47f9b-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47f9b-165">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47f9b-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47f9b-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="47f9b-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="47f9b-167">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47f9b-167">Schema Name</span></span>  <br/> |<span data-ttu-id="47f9b-168">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="47f9b-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="47f9b-169">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47f9b-169">Validation File</span></span>  <br/> |<span data-ttu-id="47f9b-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="47f9b-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47f9b-171">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47f9b-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="47f9b-172">False</span><span class="sxs-lookup"><span data-stu-id="47f9b-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47f9b-173">Ver também</span><span class="sxs-lookup"><span data-stu-id="47f9b-173">See also</span></span>

- [<span data-ttu-id="47f9b-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="47f9b-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="47f9b-175">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="47f9b-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="47f9b-176">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="47f9b-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

