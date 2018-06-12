---
title: SubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponseMessage
api_type:
- schema
ms.assetid: d121d38a-a61a-4f9c-a477-fc6d7f9af77e
description: O elemento SubscribeResponseMessage contém o status e o resultado de uma única solicitação de operação de assinatura.
ms.openlocfilehash: 97c7bd9f12511ff226e75f53278c13481679c8a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="fd922-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fd922-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="fd922-104">O elemento **SubscribeResponseMessage** contém o status e o resultado de uma única solicitação [Subscribe operação](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fd922-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="fd922-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="fd922-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="fd922-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fd922-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="fd922-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fd922-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
```xml
<SubscribeResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SubscriptionId/>
   <Watermark/>
</SubscribeResponseMessage>
```

 <span data-ttu-id="fd922-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fd922-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd922-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fd922-109">Attributes and elements</span></span>

<span data-ttu-id="fd922-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fd922-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd922-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="fd922-111">Attributes</span></span>

|<span data-ttu-id="fd922-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="fd922-112">**Attribute**</span></span>|<span data-ttu-id="fd922-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd922-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd922-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="fd922-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="fd922-115">Descreve o status de uma [operação Subscribe](subscribe-operation.md) de resposta.</span><span class="sxs-lookup"><span data-stu-id="fd922-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="fd922-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="fd922-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="fd922-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="fd922-117">-  Success</span></span>  <br/><span data-ttu-id="fd922-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="fd922-118">-  Warning</span></span>  <br/><span data-ttu-id="fd922-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="fd922-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="fd922-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fd922-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="fd922-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="fd922-121">**Value**</span></span>|<span data-ttu-id="fd922-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd922-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fd922-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="fd922-123">**Success**</span></span> <br/> |<span data-ttu-id="fd922-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="fd922-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="fd922-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="fd922-125">**Warning**</span></span> <br/> | <span data-ttu-id="fd922-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="fd922-126">Describes a request that was not processed.</span></span> <span data-ttu-id="fd922-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="fd922-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="fd922-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="fd922-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="fd922-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="fd922-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="fd922-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="fd922-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="fd922-131">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="fd922-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="fd922-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="fd922-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="fd922-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="fd922-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="fd922-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="fd922-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="fd922-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="fd922-135">**Error**</span></span> <br/> | <span data-ttu-id="fd922-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="fd922-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="fd922-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="fd922-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="fd922-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fd922-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="fd922-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="fd922-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="fd922-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="fd922-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="fd922-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="fd922-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="fd922-142">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="fd922-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="fd922-143">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="fd922-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="fd922-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="fd922-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fd922-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fd922-145">Child elements</span></span>

|<span data-ttu-id="fd922-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd922-146">**Element**</span></span>|<span data-ttu-id="fd922-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd922-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd922-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="fd922-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fd922-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd922-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fd922-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fd922-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fd922-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd922-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="fd922-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fd922-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fd922-153">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="fd922-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="fd922-154">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="fd922-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="fd922-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fd922-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fd922-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="fd922-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fd922-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="fd922-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="fd922-158">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="fd922-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="fd922-159">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="fd922-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="fd922-160">Representa um indicador de evento na fila de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fd922-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fd922-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fd922-161">Parent elements</span></span>

|<span data-ttu-id="fd922-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd922-162">**Element**</span></span>|<span data-ttu-id="fd922-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd922-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd922-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fd922-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fd922-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd922-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fd922-166">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="fd922-166">Remarks</span></span>

<span data-ttu-id="fd922-167">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="fd922-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd922-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fd922-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd922-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd922-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd922-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fd922-170">Schema Name</span></span>  <br/> |<span data-ttu-id="fd922-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fd922-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd922-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fd922-172">Validation File</span></span>  <br/> |<span data-ttu-id="fd922-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fd922-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd922-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fd922-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd922-175">False</span><span class="sxs-lookup"><span data-stu-id="fd922-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd922-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="fd922-176">See also</span></span>

- [<span data-ttu-id="fd922-177">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="fd922-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="fd922-178">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="fd922-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="fd922-179">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="fd922-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

