---
title: CopyItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: O elemento CopyItemResponseMessage contém o status e o resultado de uma única solicitação de operação CopyItem.
ms.openlocfilehash: 6c1acaff422fd731ca81a3ab244d76a73f3b5c15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751555"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="41e5c-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="41e5c-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="41e5c-104">O elemento **CopyItemResponseMessage** contém o status e o resultado de uma única [operação CopyItem](copyitem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="41e5c-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="41e5c-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="41e5c-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41e5c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="41e5c-106">Attributes and elements</span></span>

<span data-ttu-id="41e5c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41e5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41e5c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="41e5c-108">Attributes</span></span>

|<span data-ttu-id="41e5c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="41e5c-109">**Attribute**</span></span>|<span data-ttu-id="41e5c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e5c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41e5c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="41e5c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="41e5c-112">Descreve o status de uma resposta [CopyItem operação](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="41e5c-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="41e5c-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="41e5c-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="41e5c-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="41e5c-114">- Success</span></span>  <br/><span data-ttu-id="41e5c-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="41e5c-115">-  Warning</span></span>  <br/><span data-ttu-id="41e5c-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="41e5c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="41e5c-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="41e5c-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="41e5c-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="41e5c-118">**Value**</span></span>|<span data-ttu-id="41e5c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e5c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41e5c-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="41e5c-120">**Success**</span></span> <br/> |<span data-ttu-id="41e5c-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="41e5c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="41e5c-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="41e5c-122">**Warning**</span></span> <br/> | <span data-ttu-id="41e5c-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="41e5c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="41e5c-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="41e5c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="41e5c-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="41e5c-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="41e5c-126">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="41e5c-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="41e5c-127">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="41e5c-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="41e5c-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="41e5c-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="41e5c-129">-O banco de dados de caixa de correio (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="41e5c-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="41e5c-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="41e5c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="41e5c-131">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="41e5c-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="41e5c-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="41e5c-132">**Error**</span></span> <br/> | <span data-ttu-id="41e5c-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="41e5c-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="41e5c-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="41e5c-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="41e5c-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="41e5c-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="41e5c-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="41e5c-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="41e5c-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="41e5c-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="41e5c-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="41e5c-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="41e5c-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="41e5c-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="41e5c-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="41e5c-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="41e5c-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="41e5c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="41e5c-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41e5c-142">Child elements</span></span>

|<span data-ttu-id="41e5c-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41e5c-143">**Element**</span></span>|<span data-ttu-id="41e5c-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e5c-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41e5c-145">- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="41e5c-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="41e5c-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="41e5c-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="41e5c-147">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="41e5c-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="41e5c-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="41e5c-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="41e5c-149">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="41e5c-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="41e5c-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="41e5c-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="41e5c-151">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="41e5c-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="41e5c-152">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="41e5c-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="41e5c-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="41e5c-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="41e5c-154">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="41e5c-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="41e5c-155">Items</span><span class="sxs-lookup"><span data-stu-id="41e5c-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="41e5c-156">Contém uma matriz de itens copiados</span><span class="sxs-lookup"><span data-stu-id="41e5c-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41e5c-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41e5c-157">Parent elements</span></span>

|<span data-ttu-id="41e5c-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41e5c-158">**Element**</span></span>|<span data-ttu-id="41e5c-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41e5c-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41e5c-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="41e5c-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="41e5c-161">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="41e5c-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="41e5c-162">Comentários</span><span class="sxs-lookup"><span data-stu-id="41e5c-162">Remarks</span></span>

<span data-ttu-id="41e5c-163">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="41e5c-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41e5c-164">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="41e5c-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41e5c-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="41e5c-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="41e5c-166">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41e5c-166">Schema name</span></span>  <br/> |<span data-ttu-id="41e5c-167">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="41e5c-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="41e5c-168">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41e5c-168">Validation file</span></span>  <br/> |<span data-ttu-id="41e5c-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="41e5c-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41e5c-170">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="41e5c-170">Can be empty</span></span>  <br/> |<span data-ttu-id="41e5c-171">False</span><span class="sxs-lookup"><span data-stu-id="41e5c-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41e5c-172">Ver também</span><span class="sxs-lookup"><span data-stu-id="41e5c-172">See also</span></span>

- [<span data-ttu-id="41e5c-173">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="41e5c-173">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="41e5c-174">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="41e5c-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

