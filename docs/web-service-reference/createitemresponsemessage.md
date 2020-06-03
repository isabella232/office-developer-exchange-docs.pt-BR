---
title: CreateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponseMessage
api_type:
- schema
ms.assetid: 595d36c2-f87a-4d50-8e8b-f58d7641564b
description: O elemento CreateItemResponseMessage contém o status e o resultado de uma solicitação de operação CreateItem única.
ms.openlocfilehash: 6304d2c7a3c9253c03c07eb37e9a57226e794a24
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457848"
---
# <a name="createitemresponsemessage"></a><span data-ttu-id="fc486-103">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fc486-103">CreateItemResponseMessage</span></span>

<span data-ttu-id="fc486-104">O elemento **CreateItemResponseMessage** contém o status e o resultado de uma solicitação de [operação CreateItem](createitem-operation.md) única.</span><span class="sxs-lookup"><span data-stu-id="fc486-104">The **CreateItemResponseMessage** element contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="fc486-105">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="fc486-105">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="fc486-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fc486-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="fc486-107">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fc486-107">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
  
```xml
<CreateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CreateItemResponseMessage>
```

 <span data-ttu-id="fc486-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fc486-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc486-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc486-109">Attributes and elements</span></span>

<span data-ttu-id="fc486-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc486-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc486-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc486-111">Attributes</span></span>

|<span data-ttu-id="fc486-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="fc486-112">**Attribute**</span></span>|<span data-ttu-id="fc486-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc486-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fc486-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="fc486-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="fc486-115">Descreve o status de uma resposta de [operação CreateItem](createitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="fc486-115">Describes the status of a [CreateItem operation](createitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="fc486-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="fc486-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="fc486-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="fc486-117">-  Success</span></span>  <br/><span data-ttu-id="fc486-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="fc486-118">-  Warning</span></span>  <br/><span data-ttu-id="fc486-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="fc486-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="fc486-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fc486-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="fc486-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="fc486-121">**Value**</span></span>|<span data-ttu-id="fc486-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc486-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fc486-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="fc486-123">**Success**</span></span> <br/> |<span data-ttu-id="fc486-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="fc486-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="fc486-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="fc486-125">**Warning**</span></span> <br/> | <span data-ttu-id="fc486-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="fc486-126">Describes a request that was not processed.</span></span> <span data-ttu-id="fc486-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="fc486-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="fc486-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="fc486-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="fc486-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="fc486-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="fc486-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="fc486-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="fc486-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="fc486-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="fc486-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="fc486-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="fc486-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="fc486-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="fc486-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="fc486-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="fc486-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="fc486-135">**Error**</span></span> <br/> | <span data-ttu-id="fc486-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="fc486-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="fc486-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="fc486-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="fc486-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="fc486-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="fc486-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="fc486-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="fc486-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="fc486-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="fc486-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="fc486-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="fc486-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="fc486-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="fc486-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="fc486-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="fc486-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="fc486-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fc486-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc486-145">Child elements</span></span>

|<span data-ttu-id="fc486-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc486-146">**Element**</span></span>|<span data-ttu-id="fc486-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc486-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc486-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="fc486-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fc486-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc486-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fc486-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fc486-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fc486-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="fc486-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="fc486-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fc486-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fc486-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="fc486-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="fc486-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="fc486-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="fc486-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fc486-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fc486-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="fc486-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fc486-157">Itens</span><span class="sxs-lookup"><span data-stu-id="fc486-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="fc486-158">Contém uma matriz de itens criados.</span><span class="sxs-lookup"><span data-stu-id="fc486-158">Contains an array of created items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc486-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc486-159">Parent elements</span></span>

|<span data-ttu-id="fc486-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc486-160">**Element**</span></span>|<span data-ttu-id="fc486-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc486-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc486-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fc486-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fc486-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc486-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc486-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc486-164">Remarks</span></span>

<span data-ttu-id="fc486-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="fc486-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc486-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc486-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc486-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc486-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc486-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc486-168">Schema Name</span></span>  <br/> |<span data-ttu-id="fc486-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fc486-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc486-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc486-170">Validation File</span></span>  <br/> |<span data-ttu-id="fc486-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fc486-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc486-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc486-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc486-173">False</span><span class="sxs-lookup"><span data-stu-id="fc486-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc486-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc486-174">See also</span></span>

- [<span data-ttu-id="fc486-175">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="fc486-175">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="fc486-176">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="fc486-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="fc486-177">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fc486-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

