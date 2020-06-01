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
ms.openlocfilehash: 377aee12d8cc7d6b4aff8d6fc2a6cb67b3bcd10b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464690"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="65a72-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65a72-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="65a72-104">O elemento **ApplyConversationActionResponseMessage** contém o status e os resultados de uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="65a72-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="65a72-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="65a72-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="65a72-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="65a72-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="65a72-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65a72-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="65a72-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="65a72-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65a72-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="65a72-109">Attributes and elements</span></span>

<span data-ttu-id="65a72-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="65a72-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65a72-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="65a72-111">Attributes</span></span>

|<span data-ttu-id="65a72-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="65a72-112">**Attribute**</span></span>|<span data-ttu-id="65a72-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65a72-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65a72-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="65a72-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="65a72-115">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a72-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="65a72-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="65a72-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="65a72-117">Êxito</span><span class="sxs-lookup"><span data-stu-id="65a72-117">Success</span></span></li><li><span data-ttu-id="65a72-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="65a72-118">Warning</span></span></li><li><span data-ttu-id="65a72-119">Erro</span><span class="sxs-lookup"><span data-stu-id="65a72-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="65a72-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="65a72-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="65a72-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="65a72-121">**Value**</span></span>|<span data-ttu-id="65a72-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65a72-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65a72-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="65a72-123">**Success**</span></span> <br/> |<span data-ttu-id="65a72-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="65a72-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="65a72-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="65a72-125">**Warning**</span></span> <br/> | <span data-ttu-id="65a72-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="65a72-126">Describes a request that was not processed.</span></span> <span data-ttu-id="65a72-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="65a72-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="65a72-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="65a72-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="65a72-129">O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="65a72-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="65a72-130">Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="65a72-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="65a72-131">As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="65a72-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="65a72-132">O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="65a72-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="65a72-133">Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="65a72-133">A password is expired.</span></span></li><li><span data-ttu-id="65a72-134">Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="65a72-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="65a72-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="65a72-135">**Error**</span></span> <br/> | <span data-ttu-id="65a72-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="65a72-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="65a72-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="65a72-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="65a72-138">Elementos ou atributos inválidos</span><span class="sxs-lookup"><span data-stu-id="65a72-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="65a72-139">Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="65a72-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="65a72-140">Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="65a72-140">An unknown tag</span></span>  </li><li><span data-ttu-id="65a72-141">Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="65a72-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="65a72-142">Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="65a72-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="65a72-143">Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="65a72-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="65a72-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="65a72-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="65a72-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="65a72-145">Child elements</span></span>

|<span data-ttu-id="65a72-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="65a72-146">**Element**</span></span>|<span data-ttu-id="65a72-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65a72-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65a72-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="65a72-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="65a72-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="65a72-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="65a72-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="65a72-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="65a72-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="65a72-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="65a72-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="65a72-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="65a72-153">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="65a72-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="65a72-154">Este elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="65a72-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="65a72-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="65a72-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="65a72-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="65a72-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65a72-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="65a72-157">Parent elements</span></span>

|<span data-ttu-id="65a72-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="65a72-158">**Element**</span></span>|<span data-ttu-id="65a72-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="65a72-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65a72-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="65a72-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="65a72-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="65a72-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65a72-162">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="65a72-162">Text value</span></span>

<span data-ttu-id="65a72-163">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="65a72-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65a72-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="65a72-164">Remarks</span></span>

<span data-ttu-id="65a72-165">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="65a72-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="65a72-166">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="65a72-166">Version differences</span></span>

<span data-ttu-id="65a72-167">Nas versões do Exchange que começam com a compilação 15.00.0986.00, o elemento **ApplyConversationActionResponseMessage** é do tipo **ApplyConversationActionResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="65a72-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="65a72-168">Nas versões anteriores, o elemento é do tipo **ResponseMessageType**.</span><span class="sxs-lookup"><span data-stu-id="65a72-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65a72-169">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="65a72-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65a72-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="65a72-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65a72-171">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="65a72-171">Schema Name</span></span>  <br/> |<span data-ttu-id="65a72-172">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="65a72-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="65a72-173">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="65a72-173">Validation File</span></span>  <br/> |<span data-ttu-id="65a72-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="65a72-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65a72-175">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="65a72-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="65a72-176">False</span><span class="sxs-lookup"><span data-stu-id="65a72-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65a72-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="65a72-177">See also</span></span>

- [<span data-ttu-id="65a72-178">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="65a72-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="65a72-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="65a72-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

