---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: O elemento MessageXml fornece informações de resposta de erro adicionais.
ms.openlocfilehash: 8b6d201fe35c99a65f920ed7f60c33a2271fbd2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824470"
---
# <a name="messagexml"></a>MessageXml

O elemento **MessageXml** fornece informações de resposta de erro adicionais. 
  
- [ResponseMessage](responsemessage.md)  
- [MessageXml](messagexml.md)
  
```XML
<MessageXml/>
```

 **x: nenhum**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fornece informações descritivas sobre o status de resposta. <br/> <br/>  A seguir estão algumas das expressões XPath possíveis para esse elemento: <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteItem.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendItem.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteAttachment.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de cancelamento da assinatura.  <br/> |
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
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de ResolveNames.  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação ExpandDL.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação Subscribe.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de SyncFolderItems.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de ConvertId.  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de AddDelegate.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de GetServerTimeZones.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de GetSharingFolder.  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação GetSharingFolder.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de GetSharingMetadata.  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma solicitação GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de RefreshSharingFolder.  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação RefreshSharingFolder.  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contém o status e os resultados de uma resposta **FindConversation** .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de **EmptyFolder** .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contém um resultado de uma solicitação de **UpdateInboxRules** e status.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém um resultado de uma solicitação de **UploadItemsResponse** e status.  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contém uma resposta a uma solicitação **GetInboxRules** .  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contém uma resposta a uma solicitação **GetServiceConfiguration** .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém as definições de configuração de serviço.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Este elemento não é necessário e não está incluído em todas as respostas. Ele é incluído para mensagens de erro. Solicitações que envolvem pastas ou itens, o elemento **MessageXML** conterá um ou mais elementos que contêm os URIs para as propriedades que causou o erro. Um exemplo disso é o elemento [FieldURI](fielduri.md) . 
  
O elemento **MessageXML** é do tipo **x: qualquer**, que significa que qualquer XML bem formado é conteúdo válido para este elemento.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

