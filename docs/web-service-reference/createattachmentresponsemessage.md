---
title: CreateAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: O elemento CreateAttachmentResponseMessage contém o status e o resultado de uma única solicitação de operação CreateAttachment.
ms.openlocfilehash: 14d8d1936b3cfd52bdb816343c86606cb8ccf76f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458919"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="f779f-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f779f-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="f779f-104">O elemento **CreateAttachmentResponseMessage** contém o status e o resultado de uma única solicitação de [operação CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f779f-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="f779f-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="f779f-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="f779f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f779f-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="f779f-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f779f-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="f779f-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f779f-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f779f-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f779f-109">Attributes and elements</span></span>

<span data-ttu-id="f779f-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f779f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f779f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="f779f-111">Attributes</span></span>

|<span data-ttu-id="f779f-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="f779f-112">**Attribute**</span></span>|<span data-ttu-id="f779f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f779f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f779f-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f779f-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f779f-115">Descreve o status de uma resposta de [operação de CreateAttachment](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f779f-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="f779f-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="f779f-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="f779f-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="f779f-117">-  Success</span></span>  <br/><span data-ttu-id="f779f-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="f779f-118">-  Warning</span></span>  <br/><span data-ttu-id="f779f-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="f779f-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f779f-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="f779f-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="f779f-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f779f-121">**Value**</span></span>|<span data-ttu-id="f779f-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f779f-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f779f-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="f779f-123">**Success**</span></span> <br/> |<span data-ttu-id="f779f-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="f779f-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f779f-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="f779f-125">**Warning**</span></span> <br/> | <span data-ttu-id="f779f-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="f779f-126">Describes a request that was not processed.</span></span> <span data-ttu-id="f779f-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="f779f-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="f779f-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="f779f-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="f779f-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="f779f-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f779f-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="f779f-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f779f-131">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="f779f-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="f779f-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="f779f-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f779f-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="f779f-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="f779f-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="f779f-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="f779f-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="f779f-135">**Error**</span></span> <br/> | <span data-ttu-id="f779f-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="f779f-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="f779f-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="f779f-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f779f-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="f779f-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f779f-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="f779f-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="f779f-140">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="f779f-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="f779f-141">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="f779f-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="f779f-142">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="f779f-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f779f-143">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="f779f-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="f779f-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="f779f-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f779f-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f779f-145">Child elements</span></span>

|<span data-ttu-id="f779f-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f779f-146">**Element**</span></span>|<span data-ttu-id="f779f-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f779f-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f779f-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="f779f-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f779f-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="f779f-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f779f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f779f-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f779f-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="f779f-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f779f-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f779f-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f779f-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="f779f-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="f779f-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="f779f-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f779f-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f779f-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f779f-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="f779f-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f779f-157">Anexos</span><span class="sxs-lookup"><span data-stu-id="f779f-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f779f-158">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f779f-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f779f-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f779f-159">Parent elements</span></span>

|<span data-ttu-id="f779f-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f779f-160">**Element**</span></span>|<span data-ttu-id="f779f-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f779f-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f779f-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f779f-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f779f-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f779f-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f779f-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="f779f-164">Remarks</span></span>

<span data-ttu-id="f779f-165">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f779f-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f779f-166">Se vários anexos estiverem anexados a um item em uma única viagem de ida e volta, o atributo **RootItemChangeKey** na última mensagem de resposta será aquele que representa a nova chave de alteração do item que tem os anexos.</span><span class="sxs-lookup"><span data-stu-id="f779f-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f779f-167">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f779f-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f779f-168">Namespace</span><span class="sxs-lookup"><span data-stu-id="f779f-168">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f779f-169">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f779f-169">Schema Name</span></span>  <br/> |<span data-ttu-id="f779f-170">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f779f-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f779f-171">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f779f-171">Validation File</span></span>  <br/> |<span data-ttu-id="f779f-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f779f-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f779f-173">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f779f-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="f779f-174">False</span><span class="sxs-lookup"><span data-stu-id="f779f-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f779f-175">Confira também</span><span class="sxs-lookup"><span data-stu-id="f779f-175">See also</span></span>

- [<span data-ttu-id="f779f-176">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="f779f-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="f779f-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="f779f-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="f779f-178">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="f779f-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="f779f-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f779f-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

