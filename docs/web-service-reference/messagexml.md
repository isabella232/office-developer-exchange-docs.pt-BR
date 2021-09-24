---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: O elemento MessageXml fornece informações adicionais de resposta a erros.
ms.openlocfilehash: 714f055956cee6686acccd98881a12fb976e6c12
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540759"
---
# <a name="messagexml"></a>MessageXml

O **elemento MessageXml** fornece informações adicionais de resposta a erros. 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **xs:any**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fornece informações descritivas sobre o status da resposta. <br/> <br/>  Veja a seguir algumas das possíveis expressões XPath para este elemento: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação unsubscribe.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateFolder.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetFolder.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação UpdateFolder.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação MoveFolder.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CopyFolder.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateManagedFolder.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação FindFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateItem.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetItem.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação UpdateItem.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação MoveItem.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CopyItem.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateAttachment.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetAttachment.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação FindItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação ResolveNames.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação ExpandDL.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação Descrever.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação SyncFolderItems.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação ConvertId.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação AddDelegate.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação GetServerTimeZones.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação GetSharingFolder.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação GetSharingFolder.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação GetSharingMetadata.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma solicitação GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação RefreshSharingFolder.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação RefreshSharingFolder.  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contém o status e os resultados de uma **resposta FindConversation.**  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de **uma solicitação EmptyFolder.**  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contém um status e resultado de uma **solicitação UpdateInboxRules.**  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém um status e um resultado de uma **solicitação UploadItemsResponse.**  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contém uma resposta a uma **solicitação GetInboxRules.**  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contém uma resposta a uma **solicitação GetServiceConfiguration.**  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém configurações de serviço.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento não é necessário e não está incluído em todas as respostas. Ele está incluído para mensagens de erro. Em solicitações que envolvem pastas ou itens, o elemento **MessageXML** conterá um ou mais elementos que contêm as URIs para as propriedades que causaram o erro. Um exemplo disso é o [elemento FieldURI.](fielduri.md) 
  
O **elemento MessageXML** é do tipo **xs:any**, o que significa que qualquer XML bem formado é um conteúdo válido para esse elemento.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

