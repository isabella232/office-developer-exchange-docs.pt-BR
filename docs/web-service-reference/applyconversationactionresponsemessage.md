---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: O elemento ApplyConversationActionResponseMessage contém o status e os resultados de uma solicitação de operação ApplyConversationAction.
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751182"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="14c30-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14c30-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="14c30-104">O elemento **ApplyConversationActionResponseMessage** contém o status e os resultados de uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="14c30-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="14c30-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="14c30-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="14c30-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14c30-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="14c30-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14c30-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="14c30-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="14c30-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14c30-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="14c30-109">Attributes and elements</span></span>

<span data-ttu-id="14c30-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="14c30-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14c30-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="14c30-111">Attributes</span></span>

|<span data-ttu-id="14c30-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="14c30-112">**Attribute**</span></span>|<span data-ttu-id="14c30-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14c30-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="14c30-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="14c30-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="14c30-115">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="14c30-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="14c30-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="14c30-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="14c30-117">Êxito</span><span class="sxs-lookup"><span data-stu-id="14c30-117">Success</span></span></li><li><span data-ttu-id="14c30-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="14c30-118">Warning</span></span></li><li><span data-ttu-id="14c30-119">Erro</span><span class="sxs-lookup"><span data-stu-id="14c30-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="14c30-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="14c30-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="14c30-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="14c30-121">**Value**</span></span>|<span data-ttu-id="14c30-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14c30-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="14c30-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="14c30-123">**Success**</span></span> <br/> |<span data-ttu-id="14c30-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="14c30-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="14c30-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="14c30-125">**Warning**</span></span> <br/> | <span data-ttu-id="14c30-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="14c30-126">Describes a request that was not processed.</span></span> <span data-ttu-id="14c30-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="14c30-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="14c30-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="14c30-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="14c30-129">O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="14c30-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="14c30-130">Serviços de domínio Active Directory (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="14c30-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="14c30-131">Caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="14c30-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="14c30-132">O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="14c30-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="14c30-133">Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="14c30-133">A password is expired.</span></span></li><li><span data-ttu-id="14c30-134">Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="14c30-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="14c30-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="14c30-135">**Error**</span></span> <br/> | <span data-ttu-id="14c30-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="14c30-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="14c30-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="14c30-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="14c30-138">Elementos ou atributos inválidos</span><span class="sxs-lookup"><span data-stu-id="14c30-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="14c30-139">Atributos e elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="14c30-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="14c30-140">Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="14c30-140">An unknown tag</span></span>  </li><li><span data-ttu-id="14c30-141">Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="14c30-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="14c30-142">Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="14c30-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="14c30-143">Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="14c30-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="14c30-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="14c30-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="14c30-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="14c30-145">Child elements</span></span>

|<span data-ttu-id="14c30-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14c30-146">**Element**</span></span>|<span data-ttu-id="14c30-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14c30-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14c30-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="14c30-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="14c30-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="14c30-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="14c30-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="14c30-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="14c30-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="14c30-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="14c30-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="14c30-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="14c30-153">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="14c30-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="14c30-154">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="14c30-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="14c30-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="14c30-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="14c30-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="14c30-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14c30-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="14c30-157">Parent elements</span></span>

|<span data-ttu-id="14c30-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="14c30-158">**Element**</span></span>|<span data-ttu-id="14c30-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="14c30-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14c30-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14c30-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="14c30-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="14c30-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14c30-162">Text value</span><span class="sxs-lookup"><span data-stu-id="14c30-162">Text value</span></span>

<span data-ttu-id="14c30-163">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="14c30-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14c30-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="14c30-164">Remarks</span></span>

<span data-ttu-id="14c30-165">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="14c30-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="14c30-166">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="14c30-166">Version differences</span></span>

<span data-ttu-id="14c30-167">Nas versões do Exchange, começando com compilação 15.00.0986.00, o elemento **ApplyConversationActionResponseMessage** é do tipo **ApplyConversationActionResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="14c30-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="14c30-168">Nas versões anteriores, o elemento é do tipo **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="14c30-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14c30-169">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="14c30-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14c30-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="14c30-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14c30-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="14c30-171">Schema Name</span></span>  <br/> |<span data-ttu-id="14c30-172">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="14c30-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="14c30-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="14c30-173">Validation File</span></span>  <br/> |<span data-ttu-id="14c30-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="14c30-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14c30-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="14c30-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="14c30-176">False</span><span class="sxs-lookup"><span data-stu-id="14c30-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14c30-177">Ver também</span><span class="sxs-lookup"><span data-stu-id="14c30-177">See also</span></span>

- [<span data-ttu-id="14c30-178">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="14c30-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="14c30-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="14c30-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

