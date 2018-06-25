---
title: UploadItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: O elemento UploadItemsResponseMessage contém o status e os resultados de uma solicitação para carregar um item de caixa de correio única.
ms.openlocfilehash: 9a1a33011aa1e240ab7e15794e2e89401238ffda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837958"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="c61a8-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c61a8-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="c61a8-104">O elemento **UploadItemsResponseMessage** contém o status e os resultados de uma solicitação para carregar um item de caixa de correio única.</span><span class="sxs-lookup"><span data-stu-id="c61a8-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="c61a8-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="c61a8-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="c61a8-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c61a8-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="c61a8-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c61a8-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="c61a8-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c61a8-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c61a8-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c61a8-109">Attributes and elements</span></span>

<span data-ttu-id="c61a8-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c61a8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c61a8-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="c61a8-111">Attributes</span></span>

|<span data-ttu-id="c61a8-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="c61a8-112">**Attribute**</span></span>|<span data-ttu-id="c61a8-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c61a8-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c61a8-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c61a8-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c61a8-115">Descreve o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c61a8-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="c61a8-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="c61a8-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="c61a8-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="c61a8-117">-  Success</span></span>  <br/><span data-ttu-id="c61a8-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="c61a8-118">-  Warning</span></span>  <br/><span data-ttu-id="c61a8-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="c61a8-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c61a8-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c61a8-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="c61a8-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c61a8-121">**Value**</span></span>|<span data-ttu-id="c61a8-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c61a8-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c61a8-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="c61a8-123">**Success**</span></span> <br/> |<span data-ttu-id="c61a8-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="c61a8-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c61a8-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c61a8-125">**Warning**</span></span> <br/> | <span data-ttu-id="c61a8-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="c61a8-126">Describes a request that was not processed.</span></span> <span data-ttu-id="c61a8-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="c61a8-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="c61a8-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="c61a8-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="c61a8-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="c61a8-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c61a8-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="c61a8-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="c61a8-131">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="c61a8-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="c61a8-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="c61a8-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c61a8-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="c61a8-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="c61a8-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="c61a8-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="c61a8-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="c61a8-135">**Error**</span></span> <br/> | <span data-ttu-id="c61a8-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="c61a8-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c61a8-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="c61a8-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c61a8-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c61a8-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c61a8-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="c61a8-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="c61a8-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="c61a8-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="c61a8-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="c61a8-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="c61a8-142">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="c61a8-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c61a8-143">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="c61a8-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="c61a8-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="c61a8-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c61a8-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c61a8-145">Child elements</span></span>

|<span data-ttu-id="c61a8-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c61a8-146">**Element**</span></span>|<span data-ttu-id="c61a8-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c61a8-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c61a8-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c61a8-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c61a8-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c61a8-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c61a8-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c61a8-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c61a8-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c61a8-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c61a8-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c61a8-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c61a8-153">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c61a8-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="c61a8-154">Esse elemento contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="c61a8-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c61a8-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c61a8-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c61a8-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="c61a8-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c61a8-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="c61a8-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c61a8-158">Contém o identificador de item de um item carregado.</span><span class="sxs-lookup"><span data-stu-id="c61a8-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c61a8-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c61a8-159">Parent elements</span></span>

|<span data-ttu-id="c61a8-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c61a8-160">**Element**</span></span>|<span data-ttu-id="c61a8-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c61a8-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c61a8-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c61a8-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c61a8-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c61a8-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c61a8-164">Text value</span><span class="sxs-lookup"><span data-stu-id="c61a8-164">Text value</span></span>

<span data-ttu-id="c61a8-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c61a8-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c61a8-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="c61a8-166">Remarks</span></span>

<span data-ttu-id="c61a8-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c61a8-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c61a8-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c61a8-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c61a8-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="c61a8-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c61a8-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c61a8-170">Schema Name</span></span>  <br/> |<span data-ttu-id="c61a8-171">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="c61a8-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="c61a8-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c61a8-172">Validation File</span></span>  <br/> |<span data-ttu-id="c61a8-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c61a8-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c61a8-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c61a8-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="c61a8-175">False</span><span class="sxs-lookup"><span data-stu-id="c61a8-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c61a8-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="c61a8-176">See also</span></span>

- [<span data-ttu-id="c61a8-177">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="c61a8-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="c61a8-178">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="c61a8-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="c61a8-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c61a8-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

