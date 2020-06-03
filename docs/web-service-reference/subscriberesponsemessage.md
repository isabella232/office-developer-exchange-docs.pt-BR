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
ms.openlocfilehash: eea7356dbcf1887383d56e40a4f6dcd091535fa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465370"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="9eca7-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9eca7-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="9eca7-104">O elemento **SubscribeResponseMessage** contém o status e o resultado de uma única solicitação de [operação de assinatura](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9eca7-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="9eca7-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="9eca7-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="9eca7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9eca7-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="9eca7-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9eca7-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="9eca7-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9eca7-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9eca7-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9eca7-109">Attributes and elements</span></span>

<span data-ttu-id="9eca7-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9eca7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9eca7-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="9eca7-111">Attributes</span></span>

|<span data-ttu-id="9eca7-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="9eca7-112">**Attribute**</span></span>|<span data-ttu-id="9eca7-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9eca7-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9eca7-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9eca7-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9eca7-115">Descreve o status de uma resposta de [operação de assinatura](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9eca7-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9eca7-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="9eca7-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="9eca7-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="9eca7-117">-  Success</span></span>  <br/><span data-ttu-id="9eca7-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="9eca7-118">-  Warning</span></span>  <br/><span data-ttu-id="9eca7-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="9eca7-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9eca7-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9eca7-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="9eca7-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9eca7-121">**Value**</span></span>|<span data-ttu-id="9eca7-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9eca7-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9eca7-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="9eca7-123">**Success**</span></span> <br/> |<span data-ttu-id="9eca7-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="9eca7-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9eca7-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="9eca7-125">**Warning**</span></span> <br/> | <span data-ttu-id="9eca7-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="9eca7-126">Describes a request that was not processed.</span></span> <span data-ttu-id="9eca7-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="9eca7-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9eca7-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="9eca7-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9eca7-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="9eca7-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9eca7-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="9eca7-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9eca7-131">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="9eca7-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9eca7-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="9eca7-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9eca7-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="9eca7-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="9eca7-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="9eca7-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9eca7-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="9eca7-135">**Error**</span></span> <br/> | <span data-ttu-id="9eca7-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="9eca7-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9eca7-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="9eca7-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9eca7-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="9eca7-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9eca7-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="9eca7-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9eca7-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="9eca7-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="9eca7-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="9eca7-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9eca7-142">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="9eca7-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9eca7-143">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="9eca7-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9eca7-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9eca7-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9eca7-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9eca7-145">Child elements</span></span>

|<span data-ttu-id="9eca7-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9eca7-146">**Element**</span></span>|<span data-ttu-id="9eca7-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9eca7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eca7-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="9eca7-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9eca7-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9eca7-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9eca7-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9eca7-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9eca7-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="9eca7-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9eca7-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9eca7-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9eca7-153">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9eca7-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="9eca7-154">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9eca7-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9eca7-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9eca7-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9eca7-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="9eca7-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9eca7-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="9eca7-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="9eca7-158">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="9eca7-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="9eca7-159">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="9eca7-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9eca7-160">Representa um indicador de evento na fila de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9eca7-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9eca7-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9eca7-161">Parent elements</span></span>

|<span data-ttu-id="9eca7-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9eca7-162">**Element**</span></span>|<span data-ttu-id="9eca7-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9eca7-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9eca7-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9eca7-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9eca7-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9eca7-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9eca7-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="9eca7-166">Remarks</span></span>

<span data-ttu-id="9eca7-167">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9eca7-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9eca7-168">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9eca7-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9eca7-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="9eca7-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9eca7-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9eca7-170">Schema Name</span></span>  <br/> |<span data-ttu-id="9eca7-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9eca7-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9eca7-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9eca7-172">Validation File</span></span>  <br/> |<span data-ttu-id="9eca7-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9eca7-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9eca7-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9eca7-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="9eca7-175">False</span><span class="sxs-lookup"><span data-stu-id="9eca7-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9eca7-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="9eca7-176">See also</span></span>

- [<span data-ttu-id="9eca7-177">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="9eca7-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="9eca7-178">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="9eca7-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="9eca7-179">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="9eca7-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

