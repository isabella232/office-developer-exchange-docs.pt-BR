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
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825191"
---
# <a name="responsemessage"></a><span data-ttu-id="6e025-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6e025-103">ResponseMessage</span></span>

<span data-ttu-id="6e025-104">O elemento **ResponseMessage** fornece informações descritivas sobre o status de resposta para uma única entidade dentro de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e025-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="6e025-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e025-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6e025-106">Attributes and elements</span></span>

<span data-ttu-id="6e025-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e025-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e025-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e025-108">Attributes</span></span>

|<span data-ttu-id="6e025-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="6e025-109">**Attribute**</span></span>|<span data-ttu-id="6e025-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e025-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e025-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6e025-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6e025-112">Representa o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e025-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="6e025-113">Os seguintes valores são válidos para este atributo:</span><span class="sxs-lookup"><span data-stu-id="6e025-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="6e025-114">-Êxito</span><span class="sxs-lookup"><span data-stu-id="6e025-114">-  Success</span></span>  <br/><span data-ttu-id="6e025-115">-Aviso</span><span class="sxs-lookup"><span data-stu-id="6e025-115">-  Warning</span></span>  <br/><span data-ttu-id="6e025-116">-Erro</span><span class="sxs-lookup"><span data-stu-id="6e025-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="6e025-117">Valores de atributo ResponseClass</span><span class="sxs-lookup"><span data-stu-id="6e025-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="6e025-118">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6e025-118">**Value**</span></span>|<span data-ttu-id="6e025-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e025-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e025-120">Êxito</span><span class="sxs-lookup"><span data-stu-id="6e025-120">Success</span></span>  <br/> |<span data-ttu-id="6e025-121">Descreve uma solicitação que seja cumprida.</span><span class="sxs-lookup"><span data-stu-id="6e025-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6e025-122">Aviso</span><span class="sxs-lookup"><span data-stu-id="6e025-122">Warning</span></span>  <br/> | <span data-ttu-id="6e025-123">Descreve uma solicitação que não foi processada.</span><span class="sxs-lookup"><span data-stu-id="6e025-123">Describes a request that was not processed.</span></span> <span data-ttu-id="6e025-124">Um aviso pode ser retornado se ocorreu um erro quando um item na solicitação estava processando e itens subsequentes não pôde ser processados.</span><span class="sxs-lookup"><span data-stu-id="6e025-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="6e025-125">A seguir estão algumas causas possíveis avisos:</span><span class="sxs-lookup"><span data-stu-id="6e025-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="6e025-126">-O armazenamento do Exchange está offline durante o lote.</span><span class="sxs-lookup"><span data-stu-id="6e025-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6e025-127">-O serviço de diretório do Active Directory está offline.</span><span class="sxs-lookup"><span data-stu-id="6e025-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="6e025-128">-Caixas de correio são movidas.</span><span class="sxs-lookup"><span data-stu-id="6e025-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="6e025-129">-O banco de dados de mensagens (MDB) está offline.</span><span class="sxs-lookup"><span data-stu-id="6e025-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6e025-130">-Uma senha expirou.</span><span class="sxs-lookup"><span data-stu-id="6e025-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="6e025-131">-Uma cota for excedida.</span><span class="sxs-lookup"><span data-stu-id="6e025-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="6e025-132">Erro</span><span class="sxs-lookup"><span data-stu-id="6e025-132">Error</span></span>  <br/> | <span data-ttu-id="6e025-133">Descreve uma solicitação que não puder ser atendida.</span><span class="sxs-lookup"><span data-stu-id="6e025-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="6e025-134">A seguir estão algumas causas possíveis erros:</span><span class="sxs-lookup"><span data-stu-id="6e025-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="6e025-135">-Inválido atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6e025-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6e025-136">-Atributos ou elementos fora do intervalo</span><span class="sxs-lookup"><span data-stu-id="6e025-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="6e025-137">-Marca desconhecida</span><span class="sxs-lookup"><span data-stu-id="6e025-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="6e025-138">-Atributo ou elemento não é válido no contexto</span><span class="sxs-lookup"><span data-stu-id="6e025-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="6e025-139">-Tentativa de acesso não autorizado de qualquer cliente</span><span class="sxs-lookup"><span data-stu-id="6e025-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6e025-140">-Falha server-side em resposta a uma chamada de cliente válida</span><span class="sxs-lookup"><span data-stu-id="6e025-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="6e025-141">Informações sobre o erro podem ser encontradas nos elementos [ResponseCode](responsecode.md) e [MessageText](messagetext.md) .</span><span class="sxs-lookup"><span data-stu-id="6e025-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6e025-142">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e025-142">Child elements</span></span>

|<span data-ttu-id="6e025-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e025-143">**Element**</span></span>|<span data-ttu-id="6e025-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e025-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e025-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="6e025-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6e025-146">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e025-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6e025-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6e025-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6e025-148">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e025-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6e025-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6e025-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6e025-150">No momento não utilizados e está reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="6e025-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6e025-151">Ele contém um valor de 0.</span><span class="sxs-lookup"><span data-stu-id="6e025-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6e025-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6e025-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6e025-153">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="6e025-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e025-154">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e025-154">Parent elements</span></span>

|<span data-ttu-id="6e025-155">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e025-155">**Element**</span></span>|<span data-ttu-id="6e025-156">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e025-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e025-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="6e025-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="6e025-158">Contém as informações de disponibilidade para um usuário de caixa de correio única.</span><span class="sxs-lookup"><span data-stu-id="6e025-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="6e025-159">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6e025-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="6e025-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="6e025-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="6e025-161">Contém dados de informações e sugestão de resposta for solicitado sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="6e025-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="6e025-162">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6e025-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="6e025-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="6e025-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="6e025-164">Contém os resultados de resposta e as configurações de ausência temporária para um usuário.</span><span class="sxs-lookup"><span data-stu-id="6e025-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="6e025-165">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6e025-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="6e025-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="6e025-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="6e025-167">Contém o resultado de uma mensagem de [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) tentada.</span><span class="sxs-lookup"><span data-stu-id="6e025-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="6e025-168">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6e025-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e025-169">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e025-169">Remarks</span></span>

<span data-ttu-id="6e025-170">O tipo de **ResponseMessageType** é comum a todas as respostas de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e025-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="6e025-171">O tipo de **ResponseMessageType** é estendido pelos seguintes tipos complexos:</span><span class="sxs-lookup"><span data-stu-id="6e025-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="6e025-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="6e025-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6e025-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="6e025-187">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6e025-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="6e025-188">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="6e025-188">Version differences</span></span>

<span data-ttu-id="6e025-189">Os tipos de **ApplyConversationActionResponseMessage** e **DeleteItemResponseMessageType** foram introduzidos no Exchange compilação 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="6e025-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6e025-190">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6e025-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e025-191">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e025-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e025-192">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e025-192">Schema Name</span></span>  <br/> |<span data-ttu-id="6e025-193">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6e025-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e025-194">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e025-194">Validation File</span></span>  <br/> |<span data-ttu-id="6e025-195">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e025-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e025-196">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6e025-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e025-197">False</span><span class="sxs-lookup"><span data-stu-id="6e025-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e025-198">Ver também</span><span class="sxs-lookup"><span data-stu-id="6e025-198">See also</span></span>

- [<span data-ttu-id="6e025-199">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6e025-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6e025-200">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6e025-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="6e025-201">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6e025-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="6e025-202">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6e025-202">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

