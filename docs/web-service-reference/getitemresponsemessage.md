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
description: O elemento GetItemResponseMessage contém o status e o resultado de uma única solicitação de operação de GetItem.
ms.openlocfilehash: bd25a82641259e1546bad6eef5c2f6f8f03e98cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458667"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="9f05c-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f05c-103">GetItemResponseMessage</span></span>

<span data-ttu-id="9f05c-104">O elemento **GetItemResponseMessage** contém o status e o resultado de uma única solicitação de [operação de GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f05c-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="9f05c-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="9f05c-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="9f05c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f05c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="9f05c-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9f05c-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="9f05c-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9f05c-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f05c-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9f05c-109">Attributes and elements</span></span>

<span data-ttu-id="9f05c-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9f05c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f05c-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="9f05c-111">Attributes</span></span>

|<span data-ttu-id="9f05c-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="9f05c-112">**Attribute**</span></span>|<span data-ttu-id="9f05c-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f05c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f05c-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9f05c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9f05c-115">Descreve o status de uma resposta de [operação do GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9f05c-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9f05c-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="9f05c-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="9f05c-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="9f05c-117">- Success</span></span><br/><span data-ttu-id="9f05c-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="9f05c-118">- Warning</span></span><br/><span data-ttu-id="9f05c-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="9f05c-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9f05c-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9f05c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="9f05c-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9f05c-121">**Value**</span></span>|<span data-ttu-id="9f05c-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f05c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f05c-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="9f05c-123">**Success**</span></span> <br/> |<span data-ttu-id="9f05c-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="9f05c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9f05c-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="9f05c-125">**Warning**</span></span> <br/> | <span data-ttu-id="9f05c-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="9f05c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="9f05c-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação foi processado e itens subsequentes não puderam ser processados.</span><span class="sxs-lookup"><span data-stu-id="9f05c-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="9f05c-128">Estes são exemplos de fontes para avisos:</span><span class="sxs-lookup"><span data-stu-id="9f05c-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="9f05c-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="9f05c-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="9f05c-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="9f05c-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="9f05c-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="9f05c-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="9f05c-132">-O MDB está offline.</span><span class="sxs-lookup"><span data-stu-id="9f05c-132">- MDB is offline.</span></span><br/><span data-ttu-id="9f05c-133">-A senha expirou.</span><span class="sxs-lookup"><span data-stu-id="9f05c-133">- Password is expired.</span></span>  <br/><span data-ttu-id="9f05c-134">-A cota é excedida.</span><span class="sxs-lookup"><span data-stu-id="9f05c-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="9f05c-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="9f05c-135">**Error**</span></span> <br/> | <span data-ttu-id="9f05c-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="9f05c-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="9f05c-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="9f05c-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="9f05c-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="9f05c-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="9f05c-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="9f05c-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="9f05c-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="9f05c-140">- Unknown tag</span></span><br/><span data-ttu-id="9f05c-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="9f05c-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="9f05c-142">– Acesso não autorizado tentado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="9f05c-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="9f05c-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="9f05c-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="9f05c-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9f05c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="9f05c-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9f05c-145">Child elements</span></span>

|<span data-ttu-id="9f05c-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f05c-146">**Element**</span></span>|<span data-ttu-id="9f05c-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f05c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f05c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="9f05c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9f05c-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f05c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9f05c-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9f05c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9f05c-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="9f05c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9f05c-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9f05c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9f05c-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9f05c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9f05c-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9f05c-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9f05c-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9f05c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9f05c-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="9f05c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9f05c-157">Itens</span><span class="sxs-lookup"><span data-stu-id="9f05c-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="9f05c-158">Contém uma matriz de itens retornados.</span><span class="sxs-lookup"><span data-stu-id="9f05c-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f05c-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9f05c-159">Parent elements</span></span>

|<span data-ttu-id="9f05c-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9f05c-160">**Element**</span></span>|<span data-ttu-id="9f05c-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9f05c-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f05c-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9f05c-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9f05c-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f05c-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f05c-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="9f05c-164">Remarks</span></span>

<span data-ttu-id="9f05c-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9f05c-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f05c-166">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9f05c-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f05c-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f05c-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f05c-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9f05c-168">Schema Name</span></span>  <br/> |<span data-ttu-id="9f05c-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9f05c-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f05c-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9f05c-170">Validation File</span></span>  <br/> |<span data-ttu-id="9f05c-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9f05c-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f05c-172">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9f05c-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f05c-173">False</span><span class="sxs-lookup"><span data-stu-id="9f05c-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f05c-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="9f05c-174">See also</span></span>

- [<span data-ttu-id="9f05c-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="9f05c-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="9f05c-176">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="9f05c-176">GetItem operation</span></span>](getitem-operation.md)

