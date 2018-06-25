---
title: FindConversationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversationResponse
api_type:
- schema
ms.assetid: a689e29d-5f3d-4deb-81ee-8b6cc60f6dea
description: O elemento de FindConversationResponse define uma resposta a uma solicitação de operação FindConversation.
ms.openlocfilehash: 5754ea7540fa6daac8cd725386ca213d5bf05c8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752267"
---
# <a name="findconversationresponse"></a><span data-ttu-id="11b12-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="11b12-103">FindConversationResponse</span></span>

<span data-ttu-id="11b12-104">O elemento de **FindConversationResponse** define uma resposta a uma solicitação de [operação FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="11b12-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="11b12-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="11b12-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="11b12-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="11b12-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11b12-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="11b12-107">Attributes and elements</span></span>

<span data-ttu-id="11b12-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11b12-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11b12-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="11b12-109">Attributes</span></span>

|<span data-ttu-id="11b12-110">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="11b12-110">**Attribute**</span></span>|<span data-ttu-id="11b12-111">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11b12-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11b12-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="11b12-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="11b12-113">Descreve o status de uma resposta de [operação FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="11b12-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="11b12-114">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="11b12-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="11b12-115">-Êxito</span><span class="sxs-lookup"><span data-stu-id="11b12-115">-  Success</span></span>  <br/><span data-ttu-id="11b12-116">-Aviso</span><span class="sxs-lookup"><span data-stu-id="11b12-116">-  Warning</span></span>  <br/><span data-ttu-id="11b12-117">-Erro</span><span class="sxs-lookup"><span data-stu-id="11b12-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="11b12-118">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="11b12-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="11b12-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="11b12-119">**Value**</span></span>|<span data-ttu-id="11b12-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11b12-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="11b12-121">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="11b12-121">**Success**</span></span> <br/> |<span data-ttu-id="11b12-122">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="11b12-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="11b12-123">**Warning**</span><span class="sxs-lookup"><span data-stu-id="11b12-123">**Warning**</span></span> <br/> | <span data-ttu-id="11b12-124">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="11b12-124">Describes a request that was not processed.</span></span> <span data-ttu-id="11b12-125">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="11b12-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="11b12-126">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="11b12-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="11b12-127">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="11b12-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="11b12-128">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="11b12-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="11b12-129">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="11b12-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="11b12-130">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="11b12-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="11b12-131">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="11b12-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="11b12-132">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="11b12-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="11b12-133">**Erro**</span><span class="sxs-lookup"><span data-stu-id="11b12-133">**Error**</span></span> <br/> | <span data-ttu-id="11b12-134">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="11b12-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="11b12-135">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="11b12-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="11b12-136">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="11b12-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="11b12-137">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="11b12-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="11b12-138">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="11b12-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="11b12-139">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="11b12-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="11b12-140">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="11b12-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="11b12-141">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="11b12-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="11b12-142">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="11b12-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="11b12-143">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11b12-143">Child elements</span></span>

|<span data-ttu-id="11b12-144">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11b12-144">**Element**</span></span>|<span data-ttu-id="11b12-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11b12-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11b12-146">Conversas</span><span class="sxs-lookup"><span data-stu-id="11b12-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="11b12-147">Contém uma matriz de conversas.</span><span class="sxs-lookup"><span data-stu-id="11b12-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="11b12-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="11b12-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="11b12-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="11b12-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="11b12-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="11b12-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="11b12-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="11b12-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="11b12-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="11b12-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="11b12-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="11b12-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="11b12-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="11b12-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="11b12-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="11b12-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="11b12-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="11b12-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11b12-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11b12-157">Parent elements</span></span>

<span data-ttu-id="11b12-158">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11b12-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="11b12-159">Text value</span><span class="sxs-lookup"><span data-stu-id="11b12-159">Text value</span></span>

<span data-ttu-id="11b12-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11b12-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11b12-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="11b12-161">Remarks</span></span>

<span data-ttu-id="11b12-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="11b12-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11b12-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="11b12-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11b12-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="11b12-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11b12-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11b12-165">Schema name</span></span>  <br/> |<span data-ttu-id="11b12-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="11b12-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11b12-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11b12-167">Validation file</span></span>  <br/> |<span data-ttu-id="11b12-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="11b12-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11b12-169">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="11b12-169">Can be empty</span></span>  <br/> |<span data-ttu-id="11b12-170">False</span><span class="sxs-lookup"><span data-stu-id="11b12-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11b12-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="11b12-171">See also</span></span>

- [<span data-ttu-id="11b12-172">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="11b12-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="11b12-173">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="11b12-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="11b12-174">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="11b12-174">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

