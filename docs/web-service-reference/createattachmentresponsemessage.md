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
ms.openlocfilehash: a6d3adde07dedb7a2533d6e9c7fc6ff0497792bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751576"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="5aef6-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5aef6-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="5aef6-104">O elemento **CreateAttachmentResponseMessage** contém o status e o resultado de uma única [operação CreateAttachment](createattachment-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aef6-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5aef6-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="5aef6-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="5aef6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5aef6-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5aef6-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5aef6-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="5aef6-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5aef6-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5aef6-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5aef6-109">Attributes and elements</span></span>

<span data-ttu-id="5aef6-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5aef6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5aef6-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="5aef6-111">Attributes</span></span>

|<span data-ttu-id="5aef6-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5aef6-112">**Attribute**</span></span>|<span data-ttu-id="5aef6-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5aef6-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5aef6-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5aef6-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5aef6-115">Descreve o status de uma resposta [CreateAttachment operação](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5aef6-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="5aef6-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="5aef6-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="5aef6-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="5aef6-117">-  Success</span></span>  <br/><span data-ttu-id="5aef6-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="5aef6-118">-  Warning</span></span>  <br/><span data-ttu-id="5aef6-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="5aef6-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5aef6-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5aef6-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="5aef6-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5aef6-121">**Value**</span></span>|<span data-ttu-id="5aef6-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5aef6-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5aef6-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="5aef6-123">**Success**</span></span> <br/> |<span data-ttu-id="5aef6-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="5aef6-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5aef6-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5aef6-125">**Warning**</span></span> <br/> | <span data-ttu-id="5aef6-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="5aef6-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5aef6-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="5aef6-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="5aef6-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="5aef6-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="5aef6-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="5aef6-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5aef6-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="5aef6-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5aef6-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="5aef6-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="5aef6-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="5aef6-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5aef6-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="5aef6-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="5aef6-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="5aef6-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="5aef6-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="5aef6-135">**Error**</span></span> <br/> | <span data-ttu-id="5aef6-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="5aef6-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="5aef6-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="5aef6-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5aef6-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5aef6-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5aef6-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="5aef6-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="5aef6-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="5aef6-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="5aef6-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="5aef6-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="5aef6-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="5aef6-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5aef6-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="5aef6-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="5aef6-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5aef6-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5aef6-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5aef6-145">Child elements</span></span>

|<span data-ttu-id="5aef6-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5aef6-146">**Element**</span></span>|<span data-ttu-id="5aef6-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5aef6-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5aef6-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5aef6-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5aef6-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aef6-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5aef6-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5aef6-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5aef6-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aef6-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5aef6-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5aef6-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5aef6-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5aef6-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5aef6-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="5aef6-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5aef6-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5aef6-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5aef6-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="5aef6-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5aef6-157">Anexos</span><span class="sxs-lookup"><span data-stu-id="5aef6-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5aef6-158">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aef6-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5aef6-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5aef6-159">Parent elements</span></span>

|<span data-ttu-id="5aef6-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5aef6-160">**Element**</span></span>|<span data-ttu-id="5aef6-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5aef6-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5aef6-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5aef6-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5aef6-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aef6-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5aef6-164">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="5aef6-164">Remarks</span></span>

<span data-ttu-id="5aef6-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5aef6-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5aef6-166">Se vários anexos anexados a um item em uma única viagem de ida e, o atributo **RootItemChangeKey** na última mensagem de resposta é aquela que representa a nova chave de alteração do item que tenha os anexos.</span><span class="sxs-lookup"><span data-stu-id="5aef6-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5aef6-167">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5aef6-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5aef6-168">Namespace</span><span class="sxs-lookup"><span data-stu-id="5aef6-168">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5aef6-169">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5aef6-169">Schema Name</span></span>  <br/> |<span data-ttu-id="5aef6-170">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5aef6-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5aef6-171">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5aef6-171">Validation File</span></span>  <br/> |<span data-ttu-id="5aef6-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5aef6-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5aef6-173">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5aef6-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="5aef6-174">False</span><span class="sxs-lookup"><span data-stu-id="5aef6-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5aef6-175">Ver também</span><span class="sxs-lookup"><span data-stu-id="5aef6-175">See also</span></span>

- [<span data-ttu-id="5aef6-176">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="5aef6-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="5aef6-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="5aef6-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="5aef6-178">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="5aef6-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="5aef6-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5aef6-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

