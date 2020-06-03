---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: O elemento ResponseMessage fornece informações descritivas sobre o status de resposta para uma única entidade dentro de uma solicitação.
ms.openlocfilehash: a7f4240b1e988cb69d67118c6db58db0d7babba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467155"
---
# <a name="responsemessage"></a><span data-ttu-id="13fea-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="13fea-103">ResponseMessage</span></span>

<span data-ttu-id="13fea-104">O elemento **ResponseMessage** fornece informações descritivas sobre o status de resposta para uma única entidade dentro de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="13fea-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="13fea-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13fea-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="13fea-106">Attributes and elements</span></span>

<span data-ttu-id="13fea-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="13fea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13fea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="13fea-108">Attributes</span></span>

|<span data-ttu-id="13fea-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="13fea-109">**Attribute**</span></span>|<span data-ttu-id="13fea-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13fea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13fea-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="13fea-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="13fea-112">Representa o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="13fea-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="13fea-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="13fea-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="13fea-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="13fea-114">-  Success</span></span>  <br/><span data-ttu-id="13fea-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="13fea-115">-  Warning</span></span>  <br/><span data-ttu-id="13fea-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="13fea-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="13fea-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="13fea-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="13fea-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="13fea-118">**Value**</span></span>|<span data-ttu-id="13fea-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13fea-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13fea-120">Êxito</span><span class="sxs-lookup"><span data-stu-id="13fea-120">Success</span></span>  <br/> |<span data-ttu-id="13fea-121">Descreve uma solicitação que é atendida.</span><span class="sxs-lookup"><span data-stu-id="13fea-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="13fea-122">Aviso</span><span class="sxs-lookup"><span data-stu-id="13fea-122">Warning</span></span>  <br/> | <span data-ttu-id="13fea-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="13fea-123">Describes a request that was not processed.</span></span> <span data-ttu-id="13fea-124">Um aviso pode ser retornado se um erro ocorreu enquanto um item na solicitação estava sendo processado e não foi possível processar os itens subsequentes.</span><span class="sxs-lookup"><span data-stu-id="13fea-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="13fea-125">Veja a seguir algumas possíveis causas para os avisos:</span><span class="sxs-lookup"><span data-stu-id="13fea-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="13fea-126">– O repositório do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="13fea-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="13fea-127">– O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="13fea-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="13fea-128">-As caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="13fea-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="13fea-129">– O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="13fea-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="13fea-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="13fea-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="13fea-131">-Uma cota foi excedida.</span><span class="sxs-lookup"><span data-stu-id="13fea-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="13fea-132">Erro</span><span class="sxs-lookup"><span data-stu-id="13fea-132">Error</span></span>  <br/> | <span data-ttu-id="13fea-133">Descreve uma solicitação que não pode ser atendida.</span><span class="sxs-lookup"><span data-stu-id="13fea-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="13fea-134">Veja a seguir algumas possíveis causas de erros:</span><span class="sxs-lookup"><span data-stu-id="13fea-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="13fea-135">-Atributos ou elementos inválidos</span><span class="sxs-lookup"><span data-stu-id="13fea-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="13fea-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="13fea-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="13fea-137">– Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="13fea-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="13fea-138">-Atributo ou elemento não válido no contexto</span><span class="sxs-lookup"><span data-stu-id="13fea-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="13fea-139">– Tentativa de acesso não autorizado por qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="13fea-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="13fea-140">-Falha do servidor em resposta a uma chamada válida do lado do cliente</span><span class="sxs-lookup"><span data-stu-id="13fea-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="13fea-141">As informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="13fea-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="13fea-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="13fea-142">Child elements</span></span>

|<span data-ttu-id="13fea-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13fea-143">**Element**</span></span>|<span data-ttu-id="13fea-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13fea-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13fea-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="13fea-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="13fea-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="13fea-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="13fea-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="13fea-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="13fea-148">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="13fea-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="13fea-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="13fea-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="13fea-150">Não utilizado no momento e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="13fea-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="13fea-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="13fea-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="13fea-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="13fea-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="13fea-153">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="13fea-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13fea-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="13fea-154">Parent elements</span></span>

|<span data-ttu-id="13fea-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13fea-155">**Element**</span></span>|<span data-ttu-id="13fea-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13fea-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13fea-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="13fea-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="13fea-158">Contém as informações de disponibilidade de um único usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="13fea-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="13fea-159">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="13fea-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="13fea-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="13fea-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="13fea-161">Contém informações de resposta e dados de sugestão para sugestões de reunião solicitadas.</span><span class="sxs-lookup"><span data-stu-id="13fea-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="13fea-162">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="13fea-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="13fea-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="13fea-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="13fea-164">Contém os resultados da resposta e as configurações de ausência temporária de um usuário.</span><span class="sxs-lookup"><span data-stu-id="13fea-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="13fea-165">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="13fea-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="13fea-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="13fea-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="13fea-167">Contém o resultado de uma mensagem tentada [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="13fea-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="13fea-168">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="13fea-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13fea-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="13fea-169">Remarks</span></span>

<span data-ttu-id="13fea-170">O tipo **ResponseMessageType** é comum a todas as respostas de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="13fea-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="13fea-171">O tipo **ResponseMessageType** é estendido pelos seguintes tipos complexos:</span><span class="sxs-lookup"><span data-stu-id="13fea-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="13fea-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="13fea-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fea-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="13fea-187">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="13fea-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="13fea-188">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="13fea-188">Version differences</span></span>

<span data-ttu-id="13fea-189">Os tipos **ApplyConversationActionResponseMessage** e **DeleteItemResponseMessageType** foram introduzidos no 15.00.0986.00 de compilação do Exchange.</span><span class="sxs-lookup"><span data-stu-id="13fea-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="13fea-190">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="13fea-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13fea-191">Namespace</span><span class="sxs-lookup"><span data-stu-id="13fea-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="13fea-192">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="13fea-192">Schema Name</span></span>  <br/> |<span data-ttu-id="13fea-193">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="13fea-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="13fea-194">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="13fea-194">Validation File</span></span>  <br/> |<span data-ttu-id="13fea-195">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="13fea-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="13fea-196">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="13fea-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="13fea-197">False</span><span class="sxs-lookup"><span data-stu-id="13fea-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13fea-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="13fea-198">See also</span></span>

- [<span data-ttu-id="13fea-199">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="13fea-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="13fea-200">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="13fea-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="13fea-201">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="13fea-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="13fea-202">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="13fea-202">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

