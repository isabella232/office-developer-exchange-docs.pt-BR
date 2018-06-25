---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: O elemento SendItemResponseMessage contém o status e o resultado de uma única solicitação de operação SendItem.
ms.openlocfilehash: 70355aa2b46303bfceafa2cfe89f1c84896f3158
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825344"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="9c36c-103">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9c36c-103">SendItemResponseMessage</span></span>

<span data-ttu-id="9c36c-104">O elemento **SendItemResponseMessage** contém o status e o resultado de uma única [operação SendItem](senditem-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c36c-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="9c36c-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9c36c-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c36c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9c36c-106">Attributes and elements</span></span>

<span data-ttu-id="9c36c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9c36c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c36c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9c36c-108">Attributes</span></span>

|<span data-ttu-id="9c36c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="9c36c-109">**Attribute**</span></span>|<span data-ttu-id="9c36c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c36c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c36c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9c36c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9c36c-112">Descreve o status de uma resposta de [operação SendItem](senditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="9c36c-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9c36c-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="9c36c-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="9c36c-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="9c36c-114">-  Success</span></span>  <br/><span data-ttu-id="9c36c-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="9c36c-115">-  Warning</span></span>  <br/><span data-ttu-id="9c36c-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="9c36c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9c36c-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="9c36c-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9c36c-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9c36c-118">**Value**</span></span>|<span data-ttu-id="9c36c-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c36c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9c36c-120">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="9c36c-120">**Success**</span></span> <br/> |<span data-ttu-id="9c36c-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="9c36c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9c36c-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9c36c-122">**Warning**</span></span> <br/> | <span data-ttu-id="9c36c-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="9c36c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9c36c-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="9c36c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9c36c-125">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="9c36c-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9c36c-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="9c36c-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9c36c-127">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="9c36c-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9c36c-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="9c36c-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="9c36c-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="9c36c-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9c36c-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="9c36c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9c36c-131">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="9c36c-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="9c36c-132">**Erro**</span><span class="sxs-lookup"><span data-stu-id="9c36c-132">**Error**</span></span> <br/> | <span data-ttu-id="9c36c-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="9c36c-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9c36c-134">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="9c36c-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="9c36c-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9c36c-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9c36c-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="9c36c-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="9c36c-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="9c36c-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="9c36c-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="9c36c-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="9c36c-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="9c36c-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9c36c-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="9c36c-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="9c36c-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="9c36c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9c36c-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9c36c-142">Child elements</span></span>

|<span data-ttu-id="9c36c-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9c36c-143">**Element**</span></span>|<span data-ttu-id="9c36c-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c36c-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c36c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9c36c-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9c36c-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c36c-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9c36c-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9c36c-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9c36c-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c36c-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9c36c-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9c36c-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9c36c-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="9c36c-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9c36c-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="9c36c-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9c36c-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9c36c-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9c36c-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="9c36c-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c36c-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9c36c-154">Parent elements</span></span>

|<span data-ttu-id="9c36c-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9c36c-155">**Element**</span></span>|<span data-ttu-id="9c36c-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9c36c-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c36c-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9c36c-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9c36c-158">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c36c-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c36c-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c36c-159">Remarks</span></span>

<span data-ttu-id="9c36c-160">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server com a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9c36c-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c36c-161">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9c36c-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c36c-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c36c-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9c36c-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9c36c-163">Schema Name</span></span>  <br/> |<span data-ttu-id="9c36c-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9c36c-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9c36c-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9c36c-165">Validation File</span></span>  <br/> |<span data-ttu-id="9c36c-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9c36c-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c36c-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9c36c-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c36c-168">False</span><span class="sxs-lookup"><span data-stu-id="9c36c-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c36c-169">Ver também</span><span class="sxs-lookup"><span data-stu-id="9c36c-169">See also</span></span>

- [<span data-ttu-id="9c36c-170">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="9c36c-170">SendItem operation</span></span>](senditem-operation.md)
- [<span data-ttu-id="9c36c-171">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9c36c-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

