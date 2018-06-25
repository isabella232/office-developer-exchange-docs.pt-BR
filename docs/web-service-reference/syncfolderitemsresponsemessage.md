---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: O elemento SyncFolderItemsResponseMessage contém o status e o resultado de uma única solicitação de operação SyncFolderItems.
ms.openlocfilehash: 9bb32232143df56ad9de93480e10a5941e68025a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837692"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="5a303-103">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5a303-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="5a303-104">O elemento **SyncFolderItemsResponseMessage** contém o status e o resultado de uma única [operação SyncFolderItems](syncfolderitems-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a303-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5a303-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="5a303-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="5a303-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a303-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5a303-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5a303-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 <span data-ttu-id="5a303-108">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5a303-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a303-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5a303-109">Attributes and elements</span></span>

<span data-ttu-id="5a303-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5a303-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a303-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="5a303-111">Attributes</span></span>

|<span data-ttu-id="5a303-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5a303-112">**Attribute**</span></span>|<span data-ttu-id="5a303-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a303-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5a303-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5a303-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5a303-115">Descreve o status de uma resposta [SyncFolderItems operação](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5a303-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="5a303-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="5a303-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="5a303-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="5a303-117">-  Success</span></span>  <br/><span data-ttu-id="5a303-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="5a303-118">-  Warning</span></span>  <br/><span data-ttu-id="5a303-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="5a303-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="5a303-120">Atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5a303-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="5a303-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5a303-121">**Value**</span></span>|<span data-ttu-id="5a303-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a303-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5a303-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="5a303-123">**Success**</span></span> <br/> |<span data-ttu-id="5a303-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="5a303-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5a303-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5a303-125">**Warning**</span></span> <br/> | <span data-ttu-id="5a303-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="5a303-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5a303-127">Um aviso pode ser retornado se ocorreu um erro durante o processamento de um item na solicitação e itens subsequentes não podem ser processados.</span><span class="sxs-lookup"><span data-stu-id="5a303-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="5a303-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="5a303-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5a303-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="5a303-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5a303-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="5a303-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5a303-131">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="5a303-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="5a303-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="5a303-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5a303-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="5a303-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="5a303-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="5a303-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="5a303-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="5a303-135">**Error**</span></span> <br/> | <span data-ttu-id="5a303-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="5a303-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5a303-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="5a303-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5a303-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5a303-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5a303-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="5a303-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="5a303-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="5a303-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="5a303-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="5a303-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="5a303-142">-Qualquer tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="5a303-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5a303-143">-Qualquer falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="5a303-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="5a303-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5a303-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5a303-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5a303-145">Child elements</span></span>

|<span data-ttu-id="5a303-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a303-146">**Element**</span></span>|<span data-ttu-id="5a303-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a303-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a303-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5a303-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5a303-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a303-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5a303-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a303-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5a303-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a303-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5a303-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5a303-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5a303-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5a303-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5a303-154">Ele contém o valor de 0.</span><span class="sxs-lookup"><span data-stu-id="5a303-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5a303-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5a303-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5a303-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="5a303-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5a303-157">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="5a303-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5a303-158">Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="5a303-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="5a303-159">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5a303-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="5a303-160">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="5a303-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="5a303-161">Indica se o último item para sincronizar foi incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="5a303-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="5a303-162">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="5a303-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="5a303-163">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a303-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5a303-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5a303-164">Parent elements</span></span>

|<span data-ttu-id="5a303-165">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5a303-165">**Element**</span></span>|<span data-ttu-id="5a303-166">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a303-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a303-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a303-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5a303-168">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a303-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a303-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="5a303-169">Remarks</span></span>

<span data-ttu-id="5a303-170">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5a303-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a303-171">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5a303-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a303-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a303-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5a303-173">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5a303-173">Schema Name</span></span>  <br/> |<span data-ttu-id="5a303-174">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5a303-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5a303-175">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5a303-175">Validation File</span></span>  <br/> |<span data-ttu-id="5a303-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5a303-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5a303-177">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5a303-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a303-178">False</span><span class="sxs-lookup"><span data-stu-id="5a303-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a303-179">Ver também</span><span class="sxs-lookup"><span data-stu-id="5a303-179">See also</span></span>

- [<span data-ttu-id="5a303-180">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5a303-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="5a303-181">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5a303-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

