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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465370"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="9e783-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9e783-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="9e783-104">O elemento **SubscribeResponseMessage** contém o status e o resultado de uma única solicitação de [operação de assinatura](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9e783-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="9e783-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="9e783-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="9e783-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9e783-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="9e783-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9e783-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="9e783-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9e783-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e783-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9e783-109">Attributes and elements</span></span>

<span data-ttu-id="9e783-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e783-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e783-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e783-111">Attributes</span></span>

|<span data-ttu-id="9e783-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="9e783-112">**Attribute**</span></span>|<span data-ttu-id="9e783-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e783-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e783-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9e783-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9e783-115">Descreve o status de uma resposta de [operação de assinatura](subscribe-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9e783-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9e783-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="9e783-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="9e783-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="9e783-117">-  Success</span></span>  <br/><span data-ttu-id="9e783-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="9e783-118">-  Warning</span></span>  <br/><span data-ttu-id="9e783-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="9e783-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9e783-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9e783-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="9e783-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9e783-121">**Value**</span></span>|<span data-ttu-id="9e783-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e783-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e783-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="9e783-123">**Success**</span></span> <br/> |<span data-ttu-id="9e783-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="9e783-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9e783-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="9e783-125">**Warning**</span></span> <br/> | <span data-ttu-id="9e783-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="9e783-126">Describes a request that was not processed.</span></span> <span data-ttu-id="9e783-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="9e783-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9e783-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="9e783-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9e783-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="9e783-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9e783-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="9e783-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9e783-131">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="9e783-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9e783-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="9e783-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9e783-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="9e783-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="9e783-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="9e783-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9e783-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="9e783-135">**Error**</span></span> <br/> | <span data-ttu-id="9e783-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="9e783-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9e783-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="9e783-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9e783-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="9e783-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9e783-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="9e783-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9e783-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="9e783-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="9e783-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="9e783-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9e783-142">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="9e783-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9e783-143">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="9e783-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9e783-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9e783-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9e783-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e783-145">Child elements</span></span>

|<span data-ttu-id="9e783-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9e783-146">**Element**</span></span>|<span data-ttu-id="9e783-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e783-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e783-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="9e783-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9e783-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e783-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9e783-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9e783-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9e783-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="9e783-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9e783-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9e783-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9e783-153">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9e783-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="9e783-154">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9e783-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9e783-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9e783-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9e783-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="9e783-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9e783-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="9e783-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="9e783-158">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="9e783-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="9e783-159">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="9e783-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9e783-160">Representa um indicador de evento na fila de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9e783-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e783-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e783-161">Parent elements</span></span>

|<span data-ttu-id="9e783-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9e783-162">**Element**</span></span>|<span data-ttu-id="9e783-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9e783-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e783-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9e783-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9e783-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e783-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9e783-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e783-166">Remarks</span></span>

<span data-ttu-id="9e783-167">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9e783-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e783-168">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9e783-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e783-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e783-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e783-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e783-170">Schema Name</span></span>  <br/> |<span data-ttu-id="9e783-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9e783-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e783-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e783-172">Validation File</span></span>  <br/> |<span data-ttu-id="9e783-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e783-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e783-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9e783-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e783-175">False</span><span class="sxs-lookup"><span data-stu-id="9e783-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e783-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="9e783-176">See also</span></span>

- [<span data-ttu-id="9e783-177">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="9e783-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="9e783-178">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="9e783-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="9e783-179">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="9e783-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

