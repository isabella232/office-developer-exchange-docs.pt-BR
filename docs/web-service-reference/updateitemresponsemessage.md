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
description: O elemento UpdateItemResponseMessage contém o status e o resultado de uma única solicitação de operação UpdateItem.
ms.openlocfilehash: c971657813784e68a01539899e8fabea67847325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837922"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="4d00f-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d00f-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="4d00f-104">O elemento **UpdateItemResponseMessage** contém o status e o resultado de uma única [operação UpdateItem](updateitem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d00f-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="4d00f-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="4d00f-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="4d00f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d00f-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4d00f-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4d00f-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
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

 <span data-ttu-id="4d00f-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4d00f-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d00f-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4d00f-109">Attributes and elements</span></span>

<span data-ttu-id="4d00f-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4d00f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d00f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="4d00f-111">Attributes</span></span>

|<span data-ttu-id="4d00f-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="4d00f-112">**Attribute**</span></span>|<span data-ttu-id="4d00f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d00f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d00f-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4d00f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4d00f-115">Descreve o status de uma resposta [UpdateItem operação](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4d00f-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="4d00f-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="4d00f-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4d00f-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="4d00f-117">-  Success</span></span>  <br/><span data-ttu-id="4d00f-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="4d00f-118">-  Warning</span></span>  <br/><span data-ttu-id="4d00f-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="4d00f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4d00f-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="4d00f-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4d00f-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="4d00f-121">**Value**</span></span>|<span data-ttu-id="4d00f-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d00f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d00f-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="4d00f-123">**Success**</span></span> <br/> |<span data-ttu-id="4d00f-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="4d00f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4d00f-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4d00f-125">**Warning**</span></span> <br/> | <span data-ttu-id="4d00f-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="4d00f-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4d00f-127">Um aviso pode ser retornado se ocorreu um erro quando um item em que a solicitação foi processado e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="4d00f-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4d00f-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="4d00f-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4d00f-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="4d00f-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4d00f-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="4d00f-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4d00f-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="4d00f-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4d00f-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="4d00f-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4d00f-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="4d00f-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="4d00f-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="4d00f-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4d00f-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="4d00f-135">**Error**</span></span> <br/> | <span data-ttu-id="4d00f-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="4d00f-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4d00f-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="4d00f-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4d00f-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4d00f-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4d00f-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="4d00f-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="4d00f-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="4d00f-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="4d00f-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="4d00f-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="4d00f-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="4d00f-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4d00f-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="4d00f-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="4d00f-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="4d00f-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4d00f-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4d00f-145">Child elements</span></span>

|<span data-ttu-id="4d00f-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4d00f-146">**Element**</span></span>|<span data-ttu-id="4d00f-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d00f-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d00f-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4d00f-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4d00f-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d00f-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4d00f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4d00f-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4d00f-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d00f-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4d00f-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4d00f-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4d00f-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="4d00f-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4d00f-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="4d00f-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4d00f-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4d00f-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4d00f-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="4d00f-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4d00f-157">Items</span><span class="sxs-lookup"><span data-stu-id="4d00f-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="4d00f-158">Contém uma matriz de itens atualizados.</span><span class="sxs-lookup"><span data-stu-id="4d00f-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="4d00f-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="4d00f-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="4d00f-160">Contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4d00f-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d00f-161">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4d00f-161">Parent elements</span></span>

|<span data-ttu-id="4d00f-162">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4d00f-162">**Element**</span></span>|<span data-ttu-id="4d00f-163">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4d00f-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d00f-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4d00f-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4d00f-165">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d00f-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d00f-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="4d00f-166">Remarks</span></span>

<span data-ttu-id="4d00f-167">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4d00f-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d00f-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4d00f-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d00f-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="4d00f-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d00f-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4d00f-170">Schema Name</span></span>  <br/> |<span data-ttu-id="4d00f-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="4d00f-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4d00f-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4d00f-172">Validation File</span></span>  <br/> |<span data-ttu-id="4d00f-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d00f-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d00f-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4d00f-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d00f-175">False</span><span class="sxs-lookup"><span data-stu-id="4d00f-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d00f-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="4d00f-176">See also</span></span>

- [<span data-ttu-id="4d00f-177">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4d00f-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="4d00f-178">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="4d00f-178">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="4d00f-179">Atualizar as tarefas</span><span class="sxs-lookup"><span data-stu-id="4d00f-179">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

