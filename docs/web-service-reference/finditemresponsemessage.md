---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: O elemento FindItemResponseMessage contém o status e o resultado de uma única solicitação de operação FindItem.
ms.openlocfilehash: 0a4bfb3ba8d85b0bff0d03f043be865ce7276229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752288"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="0a472-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a472-103">FindItemResponseMessage</span></span>

<span data-ttu-id="0a472-104">O elemento **FindItemResponseMessage** contém o status e o resultado de uma única [operação FindItem](finditem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a472-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0a472-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="0a472-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="0a472-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a472-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0a472-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a472-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="0a472-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0a472-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a472-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0a472-109">Attributes and elements</span></span>

<span data-ttu-id="0a472-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0a472-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a472-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="0a472-111">Attributes</span></span>

|<span data-ttu-id="0a472-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0a472-112">**Attribute**</span></span>|<span data-ttu-id="0a472-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a472-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a472-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0a472-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0a472-115">Descreve o status de uma resposta de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0a472-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="0a472-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="0a472-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="0a472-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="0a472-117">-  Success</span></span>  <br/><span data-ttu-id="0a472-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="0a472-118">-  Warning</span></span>  <br/><span data-ttu-id="0a472-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="0a472-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0a472-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="0a472-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0a472-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="0a472-121">**Value**</span></span>|<span data-ttu-id="0a472-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a472-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a472-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="0a472-123">**Success**</span></span> <br/> |<span data-ttu-id="0a472-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="0a472-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0a472-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0a472-125">**Warning**</span></span> <br/> | <span data-ttu-id="0a472-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="0a472-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0a472-127">Um aviso pode ser retornado se ocorreu um erro enquanto o processamento de um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="0a472-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0a472-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="0a472-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="0a472-129">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="0a472-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="0a472-130">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0a472-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="0a472-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="0a472-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0a472-132">-O banco de dados de mensagens (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="0a472-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="0a472-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="0a472-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0a472-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="0a472-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="0a472-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="0a472-135">**Error**</span></span> <br/> | <span data-ttu-id="0a472-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="0a472-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0a472-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="0a472-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0a472-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0a472-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0a472-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="0a472-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="0a472-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="0a472-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="0a472-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="0a472-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="0a472-142">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="0a472-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0a472-143">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="0a472-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="0a472-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="0a472-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0a472-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0a472-145">Child elements</span></span>

|<span data-ttu-id="0a472-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a472-146">**Element**</span></span>|<span data-ttu-id="0a472-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a472-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a472-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0a472-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0a472-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a472-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0a472-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0a472-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0a472-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a472-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0a472-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0a472-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0a472-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="0a472-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0a472-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="0a472-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0a472-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0a472-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0a472-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="0a472-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0a472-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="0a472-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="0a472-158">Contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0a472-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a472-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0a472-159">Parent elements</span></span>

|<span data-ttu-id="0a472-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a472-160">**Element**</span></span>|<span data-ttu-id="0a472-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a472-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a472-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0a472-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0a472-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a472-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a472-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="0a472-164">Remarks</span></span>

<span data-ttu-id="0a472-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0a472-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a472-166">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0a472-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a472-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a472-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a472-168">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0a472-168">Schema name</span></span>  <br/> |<span data-ttu-id="0a472-169">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0a472-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0a472-170">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0a472-170">Validation file</span></span>  <br/> |<span data-ttu-id="0a472-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0a472-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a472-172">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0a472-172">Can be empty</span></span>  <br/> |<span data-ttu-id="0a472-173">False</span><span class="sxs-lookup"><span data-stu-id="0a472-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a472-174">Ver também</span><span class="sxs-lookup"><span data-stu-id="0a472-174">See also</span></span>

- [<span data-ttu-id="0a472-175">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="0a472-175">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="0a472-176">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="0a472-176">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

