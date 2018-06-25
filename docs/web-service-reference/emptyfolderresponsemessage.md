---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: O elemento EmptyFolderResponseMessage contém o status e o resultado de uma única solicitação EmptyFolder.
ms.openlocfilehash: ebdaac28cdd16a55811276ef0d11c03b00d3897a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752039"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="991e9-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="991e9-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="991e9-104">O elemento **EmptyFolderResponseMessage** contém o status e o resultado de uma única solicitação [EmptyFolder](emptyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="991e9-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="991e9-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="991e9-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="991e9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="991e9-106">Attributes and elements</span></span>

<span data-ttu-id="991e9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="991e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="991e9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="991e9-108">Attributes</span></span>

|<span data-ttu-id="991e9-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="991e9-109">**Attribute**</span></span>|<span data-ttu-id="991e9-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="991e9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="991e9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="991e9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="991e9-112">Descreve o status de uma resposta de [operação EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="991e9-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="991e9-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="991e9-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="991e9-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="991e9-114">-  Success</span></span>  <br/><span data-ttu-id="991e9-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="991e9-115">-  Warning</span></span>  <br/><span data-ttu-id="991e9-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="991e9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="991e9-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="991e9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="991e9-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="991e9-118">**Value**</span></span>|<span data-ttu-id="991e9-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="991e9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="991e9-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="991e9-120">**Success**</span></span> <br/> |<span data-ttu-id="991e9-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="991e9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="991e9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="991e9-122">**Warning**</span></span> <br/> | <span data-ttu-id="991e9-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="991e9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="991e9-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="991e9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="991e9-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="991e9-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="991e9-126">-O armazenamento do Exchange fica offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="991e9-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="991e9-127">-Active Directory Domain Services (AD DS) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="991e9-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="991e9-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="991e9-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="991e9-129">-O banco de dados de mensagens (MDB) ficará offline.</span><span class="sxs-lookup"><span data-stu-id="991e9-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="991e9-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="991e9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="991e9-131">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="991e9-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="991e9-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="991e9-132">**Error**</span></span> <br/> | <span data-ttu-id="991e9-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="991e9-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="991e9-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="991e9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="991e9-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="991e9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="991e9-136">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="991e9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="991e9-137">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="991e9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="991e9-138">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="991e9-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="991e9-139">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="991e9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="991e9-140">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="991e9-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="991e9-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="991e9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="991e9-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="991e9-142">Child elements</span></span>

|<span data-ttu-id="991e9-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="991e9-143">**Element**</span></span>|<span data-ttu-id="991e9-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="991e9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991e9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="991e9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="991e9-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="991e9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="991e9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="991e9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="991e9-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="991e9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="991e9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="991e9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="991e9-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="991e9-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="991e9-151">Ele contém o valor de 0.</span><span class="sxs-lookup"><span data-stu-id="991e9-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="991e9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="991e9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="991e9-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="991e9-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="991e9-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="991e9-154">Parent elements</span></span>

|<span data-ttu-id="991e9-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="991e9-155">**Element**</span></span>|<span data-ttu-id="991e9-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="991e9-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991e9-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="991e9-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="991e9-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="991e9-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="991e9-159">Text value</span><span class="sxs-lookup"><span data-stu-id="991e9-159">Text value</span></span>

<span data-ttu-id="991e9-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="991e9-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="991e9-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="991e9-161">Remarks</span></span>

<span data-ttu-id="991e9-162">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="991e9-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="991e9-163">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="991e9-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="991e9-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="991e9-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="991e9-165">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="991e9-165">Schema Name</span></span>  <br/> |<span data-ttu-id="991e9-166">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="991e9-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="991e9-167">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="991e9-167">Validation File</span></span>  <br/> |<span data-ttu-id="991e9-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="991e9-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="991e9-169">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="991e9-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="991e9-170">False</span><span class="sxs-lookup"><span data-stu-id="991e9-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="991e9-171">Ver também</span><span class="sxs-lookup"><span data-stu-id="991e9-171">See also</span></span>

- [<span data-ttu-id="991e9-172">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="991e9-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="991e9-173">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="991e9-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="991e9-174">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="991e9-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

