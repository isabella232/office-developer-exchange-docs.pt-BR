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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751576"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="a440c-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a440c-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="a440c-104">O elemento **CreateAttachmentResponseMessage** contém o status e o resultado de uma única [operação CreateAttachment](createattachment-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="a440c-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a440c-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="a440c-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="a440c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a440c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a440c-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a440c-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="a440c-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a440c-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a440c-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a440c-109">Attributes and elements</span></span>

<span data-ttu-id="a440c-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a440c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a440c-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="a440c-111">Attributes</span></span>

|<span data-ttu-id="a440c-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a440c-112">**Attribute**</span></span>|<span data-ttu-id="a440c-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a440c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a440c-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a440c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a440c-115">Descreve o status de uma resposta [CreateAttachment operação](createattachment-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a440c-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a440c-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="a440c-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="a440c-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="a440c-117">-  Success</span></span>  <br/><span data-ttu-id="a440c-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="a440c-118">-  Warning</span></span>  <br/><span data-ttu-id="a440c-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="a440c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a440c-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="a440c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a440c-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a440c-121">**Value**</span></span>|<span data-ttu-id="a440c-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a440c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a440c-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="a440c-123">**Success**</span></span> <br/> |<span data-ttu-id="a440c-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="a440c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a440c-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="a440c-125">**Warning**</span></span> <br/> | <span data-ttu-id="a440c-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="a440c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="a440c-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="a440c-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="a440c-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="a440c-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="a440c-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="a440c-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="a440c-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="a440c-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="a440c-131">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="a440c-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="a440c-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="a440c-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="a440c-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="a440c-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="a440c-134">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="a440c-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="a440c-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="a440c-135">**Error**</span></span> <br/> | <span data-ttu-id="a440c-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="a440c-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="a440c-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="a440c-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="a440c-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a440c-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="a440c-139">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="a440c-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="a440c-140">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="a440c-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="a440c-141">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="a440c-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="a440c-142">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="a440c-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="a440c-143">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="a440c-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="a440c-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="a440c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a440c-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a440c-145">Child elements</span></span>

|<span data-ttu-id="a440c-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a440c-146">**Element**</span></span>|<span data-ttu-id="a440c-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a440c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a440c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="a440c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a440c-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="a440c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a440c-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a440c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a440c-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a440c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a440c-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a440c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a440c-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="a440c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a440c-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="a440c-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a440c-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a440c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a440c-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="a440c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a440c-157">Anexos</span><span class="sxs-lookup"><span data-stu-id="a440c-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a440c-158">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440c-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a440c-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a440c-159">Parent elements</span></span>

|<span data-ttu-id="a440c-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a440c-160">**Element**</span></span>|<span data-ttu-id="a440c-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a440c-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a440c-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a440c-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a440c-163">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a440c-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a440c-164">Comentários</span><span class="sxs-lookup"><span data-stu-id="a440c-164">Remarks</span></span>

<span data-ttu-id="a440c-165">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a440c-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="a440c-166">Se vários anexos anexados a um item em uma única viagem de ida e, o atributo **RootItemChangeKey** na última mensagem de resposta é aquela que representa a nova chave de alteração do item que tenha os anexos.</span><span class="sxs-lookup"><span data-stu-id="a440c-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a440c-167">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a440c-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a440c-168">Namespace</span><span class="sxs-lookup"><span data-stu-id="a440c-168">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a440c-169">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a440c-169">Schema Name</span></span>  <br/> |<span data-ttu-id="a440c-170">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a440c-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a440c-171">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a440c-171">Validation File</span></span>  <br/> |<span data-ttu-id="a440c-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a440c-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a440c-173">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a440c-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="a440c-174">False</span><span class="sxs-lookup"><span data-stu-id="a440c-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a440c-175">Ver também</span><span class="sxs-lookup"><span data-stu-id="a440c-175">See also</span></span>

- [<span data-ttu-id="a440c-176">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="a440c-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="a440c-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="a440c-177">CreateAttachment</span></span>](createattachment.md)
- [<span data-ttu-id="a440c-178">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="a440c-178">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="a440c-179">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a440c-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

