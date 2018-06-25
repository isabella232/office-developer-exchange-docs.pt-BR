---
title: ResponseMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 2071bed8-ea66-4627-aa4f-a1d9a025cf3d
description: O elemento ResponseMessages contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.
ms.openlocfilehash: dc56476447cceac4eca56c171b148ac1ed177cb3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825203"
---
# <a name="responsemessages"></a>ResponseMessages

O elemento **ResponseMessages** contém as mensagens de resposta para uma solicitação de serviços Web do Exchange. 
  
```XML
<ResponseMessages>
   <CreateItemResponseMessage/>
</ResponseMessages>
```

```xml
<ResponseMessages>
   <DeleteItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <EmptyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetAttachmentResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UploadItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExportItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <FindItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <MoveItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CopyItemResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ResolveNamesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ExpandDLResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetServerTimeZonesResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetStreamingEventsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UnsubscribeResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SendNotificationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderHierarchyResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <SyncFolderItemsResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateManagedFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ConvertIdResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingMetadataResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <RefreshSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetSharingFolderResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <CreateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <DeleteUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <UpdateUserConfigurationResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomListsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRoomsResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetRemindersResponse/>
</ResponseMessages
```

```xml 
<ResponseMessages>
   <PerformReminderActionResponse/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <ApplyConversationActionResponseMessage/>
</ResponseMessages>
```

```xml 
<ResponseMessages>
   <GetPasswordExpirationDateResponse />
</ResponseMessages>
```


**ArrayOfResponseMessagesType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CopyFolder.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CopyItem.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateAttachment.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateFolder.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateItem.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteAttachment.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteFolder.  <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação DeleteItem.  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação [EmptyFolder](emptyfolder.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação ExpandDL.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação FindFolder.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação FindItem.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetAttachment.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém o status e os resultados de uma única solicitação UploadItems.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contém o status e os resultados de uma única solicitação ExportItems.  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetEvents.  <br/> |
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetStreamingEvents.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetFolder.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetItem.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação MoveFolder.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação MoveItem.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de ResolveNames.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendItem.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendNotification.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação Subscribe.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de SyncFolderItems.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de cancelamento da assinatura.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação UpdateFolder.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação UpdateItem.  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de ConvertId.  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de GetSharingMetadata.  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de RefreshSharingFolder.  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de GetSharingFolder.  <br/> |
|[CreateUserConfigurationResponseMessage](createuserconfigurationresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de CreateUserConfiguration.  <br/> |
|[DeleteUserConfigurationResponseMessage](deleteuserconfigurationresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponseMessage](updateuserconfigurationresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de UpdateUserConfiguration.  <br/> |
|[GetRoomListsResponse](getroomlistsresponse.md) <br/> |Contém o status e os resultados de uma solicitação de GetRoomLists.  <br/> |
|[GetRoomsResponse](getroomsresponse.md) <br/> |Contém o status e os resultados de uma solicitação de GetRooms.  <br/> |
|[GetRemindersResponse](getremindersresponse.md) <br/> |Contém o status e os resultados de uma solicitação de GetReminders.  <br/> |
|[PerformReminderActionResponse](performreminderactionresponse.md) <br/> |Contém o status e os resultados de uma solicitação de PerformReminderAction.  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetServerTimeZones.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyFolderResponse](copyfolderresponse.md) <br/> |Define uma resposta a uma solicitação de CopyFolder.  <br/> |
|[CopyItemResponse](copyitemresponse.md) <br/> |Define uma resposta a uma solicitação de CopyItem.  <br/> |
|[CreateAttachmentResponse](createattachmentresponse.md) <br/> |Define uma resposta a uma solicitação de CreateAttachment.  <br/> |
|[CreateFolderResponse](createfolderresponse.md) <br/> |Define uma resposta a uma solicitação de CreateFolder.  <br/> |
|[CreateItemResponse](createitemresponse.md) <br/> |Define uma resposta a uma solicitação de CreateItem.  <br/> |
|[CreateManagedFolderResponse](createmanagedfolderresponse.md) <br/> |Define uma resposta a uma solicitação de CreateManagedFolder.  <br/> |
|[DeleteAttachmentResponse](deleteattachmentresponse.md) <br/> |Define uma resposta a uma solicitação de DeleteAttachment.  <br/> |
|[DeleteFolderResponse](deletefolderresponse.md) <br/> |Define uma resposta a uma solicitação de DeleteFolder.  <br/> |
|[DeleteItemResponse](deleteitemresponse.md) <br/> |Define uma resposta a uma solicitação de DeleteItem.  <br/> |
|[EmptyFolderResponse](emptyfolderresponse.md) <br/> |Define uma resposta a uma solicitação EmptyFolder.  <br/> |
|[ExpandDLResponse](expanddlresponse.md) <br/> |Define uma resposta a uma solicitação de ExpandDL.  <br/> |
|[ExportItemsResponse](exportitemsresponse.md) <br/> |Representa a resposta a uma única solicitação ExportItems.  <br/> |
|[FindFolderResponse](findfolderresponse.md) <br/> |Define uma resposta a uma solicitação de FindFolder.  <br/> |
|[FindItemResponse](finditemresponse.md) <br/> |Define uma resposta a uma solicitação de FindItem.  <br/> |
|[GetAttachmentResponse](getattachmentresponse.md) <br/> |Define uma resposta a uma solicitação de GetAttachment.  <br/> |
|[GetEventsResponse](geteventsresponse.md) <br/> |Define uma resposta a uma solicitação de GetEvents.  <br/> |
|[GetStreamingEventsResponse](getstreamingeventsresponse.md) <br/> |Define uma resposta a uma solicitação GetStreamingEvents.  <br/> |
|[GetFolderResponse](getfolderresponse.md) <br/> |Define uma resposta a uma solicitação de GetFolder.  <br/> |
|[GetItemResponse](getitemresponse.md) <br/> |Define uma resposta a uma solicitação de GetItem.  <br/> |
|[MoveFolderResponse](movefolderresponse.md) <br/> |Define uma resposta a uma solicitação de MoveFolder.  <br/> |
|[MoveItemResponse](moveitemresponse.md) <br/> |Define uma resposta a uma solicitação de MoveItem.  <br/> |
|[ResolveNamesResponse](resolvenamesresponse.md) <br/> |Define uma resposta a uma solicitação de ResolveNames.  <br/> |
|[SendItemResponse](senditemresponse.md) <br/> |Define uma resposta a uma solicitação de SendItem.  <br/> |
|[SendNotificationResult](sendnotificationresult.md) <br/> |Define uma resposta a uma solicitação SendNotification.  <br/> |
|[SubscribeResponse](subscriberesponse.md) <br/> |Define uma resposta a uma solicitação Subscribe.  <br/> |
|[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) <br/> |Define uma resposta a uma solicitação de SyncFolderHierarchy.  <br/> |
|[SyncFolderItemsResponse](syncfolderitemsresponse.md) <br/> |Define uma resposta a uma solicitação de SyncFolderItems.  <br/> |
|[UnsubscribeResponse](unsubscriberesponse.md) <br/> |Define uma resposta a uma solicitação de cancelamento da assinatura.  <br/> |
|[UpdateFolderResponse](updatefolderresponse.md) <br/> |Define uma resposta a uma solicitação de UpdateFolder.  <br/> |
|[UpdateItemResponse](updateitemresponse.md) <br/> |Define uma resposta a uma solicitação de UpdateItem.  <br/> |
|[ConvertIdResponse](convertidresponse.md) <br/> |Contém uma resposta a uma solicitação ConvertId.  <br/> |
|[GetServerTimeZonesResponse](getservertimezonesresponse.md) <br/> |Define uma resposta a uma solicitação GetServerTimeZones.  <br/> |
|[CreateUserConfigurationResponse](createuserconfigurationresponse.md) <br/> |Define uma resposta a uma solicitação CreateUserConfiuration.  <br/> |
|[DeleteUserConfigurationResponse](deleteuserconfigurationresponse.md) <br/> |Define uma resposta a uma solicitação DeleteUserConfiguration.  <br/> |
|[GetUserConfigurationResponse](getuserconfigurationresponse.md) <br/> |Define uma resposta a uma solicitação GetUserConfiguration.  <br/> |
|[UpdateUserConfigurationResponse](updateuserconfigurationresponse.md) <br/> |Define uma resposta a uma solicitação UpdateUserConfiguration.  <br/> |
|[ApplyConversationActionResponse](applyconversationactionresponse.md) <br/> |Define uma resposta a uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md) <br/> |Define uma resposta a uma solicitação de operação [GetPasswordExpirationDate operação](getpasswordexpirationdate-operation.md) .  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ExportItems](exportitems-operation.md) 
- [Operação UploadItems](uploaditems-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

