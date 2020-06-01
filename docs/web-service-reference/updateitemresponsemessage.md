---
title: UpdateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponseMessage
api_type:
- schema
ms.assetid: dc585b05-5afc-4c74-8763-5a54f9a650ec
description: O elemento UpdateItemResponseMessage contém o status e o resultado de uma única solicitação de operação de UpdateItem.
ms.openlocfilehash: ef25dcf26e06f199587cef885d8cbc9e93b52bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457939"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="af206-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="af206-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="af206-104">O elemento **UpdateItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="af206-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="af206-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="af206-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="af206-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="af206-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="af206-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="af206-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
```xml
<UpdateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <ConflictResults/>
</UpdateItemResponseMessage>
```

 <span data-ttu-id="af206-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="af206-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af206-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="af206-109">Attributes and elements</span></span>

<span data-ttu-id="af206-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af206-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af206-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="af206-111">Attributes</span></span>

|<span data-ttu-id="af206-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="af206-112">**Attribute**</span></span>|<span data-ttu-id="af206-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af206-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="af206-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="af206-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="af206-115">Descreve o status de uma resposta de [operação do UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="af206-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="af206-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="af206-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="af206-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="af206-117">-  Success</span></span>  <br/><span data-ttu-id="af206-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="af206-118">-  Warning</span></span>  <br/><span data-ttu-id="af206-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="af206-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="af206-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="af206-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="af206-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="af206-121">**Value**</span></span>|<span data-ttu-id="af206-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af206-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="af206-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="af206-123">**Success**</span></span> <br/> |<span data-ttu-id="af206-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="af206-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="af206-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="af206-125">**Warning**</span></span> <br/> | <span data-ttu-id="af206-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="af206-126">Describes a request that was not processed.</span></span> <span data-ttu-id="af206-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação foi processado e itens subsequentes não puderam ser processados.</span><span class="sxs-lookup"><span data-stu-id="af206-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="af206-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="af206-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="af206-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="af206-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="af206-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="af206-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="af206-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="af206-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="af206-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="af206-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="af206-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="af206-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="af206-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="af206-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="af206-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="af206-135">**Error**</span></span> <br/> | <span data-ttu-id="af206-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="af206-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="af206-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="af206-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="af206-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="af206-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="af206-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="af206-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="af206-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="af206-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="af206-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="af206-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="af206-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="af206-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="af206-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="af206-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="af206-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="af206-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="af206-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af206-145">Child elements</span></span>

|<span data-ttu-id="af206-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af206-146">**Element**</span></span>|<span data-ttu-id="af206-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af206-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af206-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="af206-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="af206-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="af206-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="af206-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="af206-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="af206-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="af206-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="af206-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="af206-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="af206-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="af206-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="af206-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="af206-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="af206-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="af206-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="af206-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="af206-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="af206-157">Itens</span><span class="sxs-lookup"><span data-stu-id="af206-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="af206-158">Contém uma matriz de itens atualizados.</span><span class="sxs-lookup"><span data-stu-id="af206-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="af206-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="af206-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="af206-160">Contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="af206-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af206-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af206-161">Parent elements</span></span>

|<span data-ttu-id="af206-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af206-162">**Element**</span></span>|<span data-ttu-id="af206-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af206-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af206-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="af206-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="af206-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af206-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af206-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="af206-166">Remarks</span></span>

<span data-ttu-id="af206-167">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="af206-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af206-168">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="af206-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af206-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="af206-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af206-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af206-170">Schema Name</span></span>  <br/> |<span data-ttu-id="af206-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="af206-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="af206-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af206-172">Validation File</span></span>  <br/> |<span data-ttu-id="af206-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af206-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af206-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="af206-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="af206-175">False</span><span class="sxs-lookup"><span data-stu-id="af206-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af206-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="af206-176">See also</span></span>

- [<span data-ttu-id="af206-177">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="af206-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="af206-178">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="af206-178">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="af206-179">Atualizando tarefas</span><span class="sxs-lookup"><span data-stu-id="af206-179">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

