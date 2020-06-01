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
description: O elemento SyncFolderHierarchyResponseMessage contém o status e o resultado de uma única solicitação de operação de SyncFolderHierarchy.
ms.openlocfilehash: fda0a37178f89ba0fd5ef860f8b009f335a11391
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465342"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="5203b-103">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5203b-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="5203b-104">O elemento **SyncFolderHierarchyResponseMessage** contém o status e o resultado de uma única solicitação de [operação de SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5203b-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5203b-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="5203b-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="5203b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5203b-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5203b-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5203b-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
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

 <span data-ttu-id="5203b-108">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5203b-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5203b-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5203b-109">Attributes and elements</span></span>

<span data-ttu-id="5203b-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5203b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5203b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="5203b-111">Attributes</span></span>

|<span data-ttu-id="5203b-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="5203b-112">**Attribute**</span></span>|<span data-ttu-id="5203b-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5203b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5203b-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5203b-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5203b-115">Descreve o status de uma resposta de [operação do SyncFolderHierarchy](syncfolderhierarchy-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="5203b-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="5203b-116">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="5203b-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="5203b-117">-Êxito</span><span class="sxs-lookup"><span data-stu-id="5203b-117">-  Success</span></span>  <br/><span data-ttu-id="5203b-118">-Aviso</span><span class="sxs-lookup"><span data-stu-id="5203b-118">-  Warning</span></span>  <br/><span data-ttu-id="5203b-119">-Erro</span><span class="sxs-lookup"><span data-stu-id="5203b-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5203b-120">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5203b-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="5203b-121">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5203b-121">**Value**</span></span>|<span data-ttu-id="5203b-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5203b-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5203b-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="5203b-123">**Success**</span></span> <br/> |<span data-ttu-id="5203b-124">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="5203b-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5203b-125">**Aviso**</span><span class="sxs-lookup"><span data-stu-id="5203b-125">**Warning**</span></span> <br/> | <span data-ttu-id="5203b-126">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="5203b-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5203b-127">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="5203b-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5203b-128">A seguir estão exemplos de fontes de avisos:</span><span class="sxs-lookup"><span data-stu-id="5203b-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5203b-129">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="5203b-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5203b-130">– Os serviços de domínio do Active Directory (AD DS) estão offline.</span><span class="sxs-lookup"><span data-stu-id="5203b-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5203b-131">-As caixas de correio foram movidas.</span><span class="sxs-lookup"><span data-stu-id="5203b-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="5203b-132">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="5203b-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5203b-133">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="5203b-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="5203b-134">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="5203b-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="5203b-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="5203b-135">**Error**</span></span> <br/> | <span data-ttu-id="5203b-136">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="5203b-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5203b-137">A seguir estão exemplos de fontes de erros:</span><span class="sxs-lookup"><span data-stu-id="5203b-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5203b-138">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="5203b-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5203b-139">-Atributos ou elementos que estão fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="5203b-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="5203b-140">-Uma marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="5203b-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="5203b-141">-Um atributo ou elemento que não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="5203b-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="5203b-142">– Uma tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="5203b-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5203b-143">-Uma falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="5203b-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5203b-144">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="5203b-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5203b-145">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5203b-145">Child elements</span></span>

|<span data-ttu-id="5203b-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5203b-146">**Element**</span></span>|<span data-ttu-id="5203b-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5203b-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5203b-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5203b-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5203b-149">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5203b-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5203b-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5203b-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5203b-151">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="5203b-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5203b-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5203b-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5203b-153">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5203b-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5203b-154">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="5203b-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5203b-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5203b-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5203b-156">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="5203b-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5203b-157">SyncState</span><span class="sxs-lookup"><span data-stu-id="5203b-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5203b-158">Contém uma forma codificada em base64 dos dados de sincronização que são atualizados após cada solicitação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="5203b-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="5203b-159">Isso é usado para identificar o estado de sincronização.</span><span class="sxs-lookup"><span data-stu-id="5203b-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="5203b-160">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="5203b-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="5203b-161">Indica se o último item a ser sincronizado foi incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="5203b-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="5203b-162">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="5203b-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="5203b-163">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5203b-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5203b-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5203b-164">Parent elements</span></span>

|<span data-ttu-id="5203b-165">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5203b-165">**Element**</span></span>|<span data-ttu-id="5203b-166">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5203b-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5203b-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5203b-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5203b-168">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5203b-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5203b-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="5203b-169">Remarks</span></span>

<span data-ttu-id="5203b-170">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5203b-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5203b-171">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5203b-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5203b-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="5203b-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5203b-173">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5203b-173">Schema Name</span></span>  <br/> |<span data-ttu-id="5203b-174">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5203b-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5203b-175">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5203b-175">Validation File</span></span>  <br/> |<span data-ttu-id="5203b-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5203b-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5203b-177">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5203b-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="5203b-178">False</span><span class="sxs-lookup"><span data-stu-id="5203b-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5203b-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="5203b-179">See also</span></span>

- [<span data-ttu-id="5203b-180">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="5203b-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="5203b-181">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5203b-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

