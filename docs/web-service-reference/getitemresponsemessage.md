---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: O elemento GetItemResponseMessage contém o status e o resultado de uma única solicitação de operação GetItem.
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752552"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="0fbd9-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd9-103">GetItemResponseMessage</span></span>

<span data-ttu-id="0fbd9-104">O elemento **GetItemResponseMessage** contém o status e o resultado de uma única [operação GetItem](getitem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0fbd9-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="0fbd9-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="0fbd9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0fbd9-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0fbd9-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0fbd9-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="0fbd9-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0fbd9-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0fbd9-109">Attributes and elements</span></span>

<span data-ttu-id="0fbd9-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fbd9-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="0fbd9-111">Attributes</span></span>

|<span data-ttu-id="0fbd9-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-112">**Attribute**</span></span>|<span data-ttu-id="0fbd9-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0fbd9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0fbd9-115">Descreve o status de uma resposta [GetItem operação](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbd9-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0fbd9-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="0fbd9-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="0fbd9-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="0fbd9-117">- Success</span></span><br/><span data-ttu-id="0fbd9-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="0fbd9-118">- Warning</span></span><br/><span data-ttu-id="0fbd9-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="0fbd9-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0fbd9-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0fbd9-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0fbd9-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-121">**Value**</span></span>|<span data-ttu-id="0fbd9-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0fbd9-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-123">**Success**</span></span> <br/> |<span data-ttu-id="0fbd9-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0fbd9-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-125">**Warning**</span></span> <br/> | <span data-ttu-id="0fbd9-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0fbd9-127">Um aviso pode ser retornado se ocorreu um erro quando um item em que a solicitação foi processado e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="0fbd9-128">Estes são exemplos de fontes para avisos:</span><span class="sxs-lookup"><span data-stu-id="0fbd9-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="0fbd9-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="0fbd9-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="0fbd9-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="0fbd9-132">-MDB está offline.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-132">- MDB is offline.</span></span><br/><span data-ttu-id="0fbd9-133">-Senha expirou.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-133">- Password is expired.</span></span>  <br/><span data-ttu-id="0fbd9-134">-Quota for excedido.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="0fbd9-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-135">**Error**</span></span> <br/> | <span data-ttu-id="0fbd9-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="0fbd9-137">Estes são exemplos de fontes para erros:</span><span class="sxs-lookup"><span data-stu-id="0fbd9-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="0fbd9-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0fbd9-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="0fbd9-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="0fbd9-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="0fbd9-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="0fbd9-140">- Unknown tag</span></span><br/><span data-ttu-id="0fbd9-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="0fbd9-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="0fbd9-142">-Acesso não autorizado tentado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="0fbd9-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="0fbd9-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="0fbd9-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="0fbd9-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0fbd9-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="0fbd9-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0fbd9-145">Child elements</span></span>

|<span data-ttu-id="0fbd9-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-146">**Element**</span></span>|<span data-ttu-id="0fbd9-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fbd9-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0fbd9-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0fbd9-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0fbd9-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0fbd9-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0fbd9-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0fbd9-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0fbd9-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0fbd9-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0fbd9-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0fbd9-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0fbd9-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0fbd9-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0fbd9-157">Items</span><span class="sxs-lookup"><span data-stu-id="0fbd9-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="0fbd9-158">Contém uma matriz de itens retornados.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fbd9-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0fbd9-159">Parent elements</span></span>

|<span data-ttu-id="0fbd9-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-160">**Element**</span></span>|<span data-ttu-id="0fbd9-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0fbd9-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fbd9-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0fbd9-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0fbd9-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0fbd9-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="0fbd9-164">Remarks</span></span>

<span data-ttu-id="0fbd9-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0fbd9-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fbd9-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0fbd9-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fbd9-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="0fbd9-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0fbd9-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0fbd9-168">Schema Name</span></span>  <br/> |<span data-ttu-id="0fbd9-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0fbd9-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0fbd9-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0fbd9-170">Validation File</span></span>  <br/> |<span data-ttu-id="0fbd9-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0fbd9-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0fbd9-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0fbd9-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fbd9-173">False</span><span class="sxs-lookup"><span data-stu-id="0fbd9-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fbd9-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="0fbd9-174">See also</span></span>

- [<span data-ttu-id="0fbd9-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="0fbd9-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="0fbd9-176">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="0fbd9-176">GetItem operation</span></span>](getitem-operation.md)

