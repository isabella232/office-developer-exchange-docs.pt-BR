---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: O elemento SyncFolderHierarchyResponseMessage contém o status e o resultado de uma única solicitação de operação SyncFolderHierarchy.
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837685"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="611ab-103">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="611ab-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="611ab-104">O elemento **SyncFolderHierarchyResponseMessage** contém o status e o resultado de uma única [operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="611ab-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="611ab-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="611ab-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="611ab-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="611ab-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="611ab-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="611ab-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 <span data-ttu-id="611ab-108">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="611ab-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="611ab-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="611ab-109">Attributes and elements</span></span>

<span data-ttu-id="611ab-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="611ab-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="611ab-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="611ab-111">Attributes</span></span>

|<span data-ttu-id="611ab-112">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="611ab-112">**Attribute**</span></span>|<span data-ttu-id="611ab-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="611ab-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="611ab-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="611ab-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="611ab-115">Descreve o status de uma resposta [SyncFolderHierarchy operação](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="611ab-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="611ab-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="611ab-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="611ab-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="611ab-117">-  Success</span></span>  <br/><span data-ttu-id="611ab-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="611ab-118">-  Warning</span></span>  <br/><span data-ttu-id="611ab-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="611ab-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="611ab-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="611ab-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="611ab-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="611ab-121">**Value**</span></span>|<span data-ttu-id="611ab-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="611ab-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="611ab-123">**Sucesso**</span><span class="sxs-lookup"><span data-stu-id="611ab-123">**Success**</span></span> <br/> |<span data-ttu-id="611ab-124">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="611ab-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="611ab-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="611ab-125">**Warning**</span></span> <br/> | <span data-ttu-id="611ab-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="611ab-126">Describes a request that was not processed.</span></span> <span data-ttu-id="611ab-127">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="611ab-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="611ab-128">Estes são exemplos de fontes de avisos de:</span><span class="sxs-lookup"><span data-stu-id="611ab-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="611ab-129">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="611ab-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="611ab-130">-Active Directory Domain Services (AD DS) está offline.</span><span class="sxs-lookup"><span data-stu-id="611ab-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="611ab-131">-Caixas de correio foram movidos.</span><span class="sxs-lookup"><span data-stu-id="611ab-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="611ab-132">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="611ab-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="611ab-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="611ab-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="611ab-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="611ab-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="611ab-135">**Erro**</span><span class="sxs-lookup"><span data-stu-id="611ab-135">**Error**</span></span> <br/> | <span data-ttu-id="611ab-136">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="611ab-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="611ab-137">Estes são exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="611ab-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="611ab-138">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="611ab-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="611ab-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="611ab-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="611ab-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="611ab-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="611ab-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="611ab-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="611ab-142">-Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="611ab-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="611ab-143">-Uma falha no servidor em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="611ab-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="611ab-144">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="611ab-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="611ab-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="611ab-145">Child elements</span></span>

|<span data-ttu-id="611ab-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="611ab-146">**Element**</span></span>|<span data-ttu-id="611ab-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="611ab-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="611ab-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="611ab-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="611ab-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="611ab-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="611ab-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="611ab-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="611ab-151">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="611ab-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="611ab-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="611ab-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="611ab-153">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="611ab-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="611ab-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="611ab-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="611ab-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="611ab-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="611ab-156">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="611ab-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="611ab-157">Estado de sincronização</span><span class="sxs-lookup"><span data-stu-id="611ab-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="611ab-158">Contém um formulário codificado na base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="611ab-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="611ab-159">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="611ab-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="611ab-160">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="611ab-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="611ab-161">Indica se o último item para sincronizar foi incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="611ab-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="611ab-162">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="611ab-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="611ab-163">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="611ab-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="611ab-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="611ab-164">Parent elements</span></span>

|<span data-ttu-id="611ab-165">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="611ab-165">**Element**</span></span>|<span data-ttu-id="611ab-166">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="611ab-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="611ab-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="611ab-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="611ab-168">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="611ab-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="611ab-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="611ab-169">Remarks</span></span>

<span data-ttu-id="611ab-170">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="611ab-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="611ab-171">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="611ab-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="611ab-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="611ab-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="611ab-173">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="611ab-173">Schema Name</span></span>  <br/> |<span data-ttu-id="611ab-174">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="611ab-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="611ab-175">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="611ab-175">Validation File</span></span>  <br/> |<span data-ttu-id="611ab-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="611ab-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="611ab-177">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="611ab-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="611ab-178">False</span><span class="sxs-lookup"><span data-stu-id="611ab-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="611ab-179">Ver também</span><span class="sxs-lookup"><span data-stu-id="611ab-179">See also</span></span>

- [<span data-ttu-id="611ab-180">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="611ab-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="611ab-181">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="611ab-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

