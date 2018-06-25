---
title: MoveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: O elemento MoveItemResponseMessage contém o status e o resultado de uma única solicitação de operação MoveItem.
ms.openlocfilehash: af1c10391d9b5b761ab87983eea6321d61231152
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824493"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="21329-103">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21329-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="21329-104">O elemento **MoveItemResponseMessage** contém o status e o resultado de uma única [operação MoveItem](moveitem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="21329-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="21329-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="21329-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21329-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="21329-106">Attributes and elements</span></span>

<span data-ttu-id="21329-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="21329-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21329-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="21329-108">Attributes</span></span>

|<span data-ttu-id="21329-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="21329-109">**Attribute**</span></span>|<span data-ttu-id="21329-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21329-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21329-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="21329-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="21329-112">Descreve o status de uma resposta [MoveItem operação](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="21329-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="21329-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="21329-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="21329-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="21329-114">-  Success</span></span>  <br/><span data-ttu-id="21329-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="21329-115">-  Warning</span></span>  <br/><span data-ttu-id="21329-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="21329-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="21329-117">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="21329-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="21329-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="21329-118">**Value**</span></span>|<span data-ttu-id="21329-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21329-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21329-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="21329-120">**Success**</span></span> <br/> |<span data-ttu-id="21329-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="21329-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="21329-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="21329-122">**Warning**</span></span> <br/> | <span data-ttu-id="21329-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="21329-123">Describes a request that was not processed.</span></span> <span data-ttu-id="21329-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="21329-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="21329-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="21329-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="21329-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="21329-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="21329-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="21329-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="21329-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="21329-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="21329-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="21329-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="21329-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="21329-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="21329-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="21329-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="21329-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="21329-132">**Error**</span></span> <br/> | <span data-ttu-id="21329-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="21329-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="21329-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="21329-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="21329-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="21329-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="21329-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="21329-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="21329-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="21329-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="21329-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="21329-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="21329-139">-Qualquer acesso não autorizado tentado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="21329-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="21329-140">-Qualquer falha no servidor em resposta a uma chamada de cliente válida.</span><span class="sxs-lookup"><span data-stu-id="21329-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="21329-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="21329-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="21329-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="21329-142">Child elements</span></span>

|<span data-ttu-id="21329-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="21329-143">**Element**</span></span>|<span data-ttu-id="21329-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21329-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21329-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="21329-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="21329-146">Uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="21329-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="21329-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21329-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="21329-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="21329-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="21329-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="21329-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="21329-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="21329-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="21329-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="21329-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="21329-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="21329-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="21329-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="21329-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="21329-154">Items</span><span class="sxs-lookup"><span data-stu-id="21329-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="21329-155">Contém uma matriz de itens movidos.</span><span class="sxs-lookup"><span data-stu-id="21329-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21329-156">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="21329-156">Parent elements</span></span>

|<span data-ttu-id="21329-157">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="21329-157">**Element**</span></span>|<span data-ttu-id="21329-158">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21329-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21329-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21329-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="21329-160">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="21329-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="21329-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="21329-161">Remarks</span></span>

<span data-ttu-id="21329-162">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="21329-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21329-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="21329-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21329-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="21329-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21329-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="21329-165">Schema Name</span></span>  <br/> |<span data-ttu-id="21329-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="21329-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21329-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="21329-167">Validation File</span></span>  <br/> |<span data-ttu-id="21329-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21329-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21329-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="21329-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="21329-170">False</span><span class="sxs-lookup"><span data-stu-id="21329-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21329-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="21329-171">See also</span></span>

- [<span data-ttu-id="21329-172">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="21329-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="21329-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="21329-173">MoveItem</span></span>](moveitem.md)

