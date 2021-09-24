---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: O elemento ResponseCode fornece informações de status sobre a solicitação.
ms.openlocfilehash: 9d662ee93870c2aabe045d801222deb881d0a28b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512384"
---
# <a name="responsecode"></a>ResponseCode

O **elemento ResponseCode** fornece informações de status sobre a solicitação. 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|Elemento|Descrição|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fornece informações descritivas sobre o status da resposta.<br/><br/>  Veja a seguir as possíveis expressões XPath para este elemento:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação DeleteItem.](deleteitem-operation.md)  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação SendItem.](senditem-operation.md)  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação DeleteFolder.](deletefolder-operation.md)  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação [DeleteAttachment.](deleteattachment-operation.md)  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação [Unsubscribe.](unsubscribe-operation.md)  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateFolder.](createfolder-operation.md)  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação GetFolder.](getfolder-operation.md)  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação UpdateFolder.](updatefolder-operation.md)  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação MoveFolder.](movefolder-operation.md)  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CopyFolder.](copyfolder-operation.md)  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateManagedFolder.](createmanagedfolder-operation.md)  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação FindFolder.](findfolder-operation.md)  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateItem.](createitem-operation.md)  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação GetItem.](getitem-operation.md)  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação UpdateItem.](updateitem-operation.md)  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação MoveItem.](moveitem-operation.md)  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CopyItem.](copyitem-operation.md)  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateAttachment.](createattachment-operation.md)  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação GetAttachment.](getattachment-operation.md)  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação FindItem.](finditem-operation.md)  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação ResolveNames.](resolvenames-operation.md)  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação ExpandDL.](expanddl-operation.md)  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação Assinar.](subscribe-operation.md)  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação GetEvents.](getevents-operation.md)  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação SyncFolderHierarchy.](syncfolderhierarchy-operation.md)  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação SyncFolderItems.](syncfolderitems-operation.md)  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação ConvertId.](convertid-operation.md)  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação AddDelegate.](adddelegate-operation.md)  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação GetDelegate.](getdelegate-operation.md)  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação RemoveDelegate.](removedelegate-operation.md)  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contém o status e o resultado de uma [solicitação de operação UpdateDelegate.](updatedelegate-operation.md)  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação GetServerTimeZones.](getservertimezones-operation.md)  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de operação [GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetSharingFolder.](getsharingfolder-operation.md)  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de operação [GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma [solicitação de operação GetSharingMetadata.](getsharingmetadata-operation.md)  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de operação [RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Define uma resposta a uma [solicitação de operação RefreshSharingFolder.](refreshsharingfolder-operation.md)  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contém o status e os resultados de uma resposta de [operação FindConversation.](findconversation-operation.md)  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contém o status e os resultados de uma [solicitação de operação ApplyConversationAction.](applyconversationaction-operation.md)  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação EmptyFolder.](emptyfolder-operation.md)  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contém um status e resultado de uma [solicitação de operação UpdateInboxRules.](updateinboxrules-operation.md)  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém um status e resultado de uma [solicitação de operação UploadItems.](uploaditems-operation.md)  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contém uma resposta a uma [solicitação de operação GetInboxRules](getinboxrules-operation.md) ****.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contém uma resposta a uma [solicitação de operação GetServiceConfiguration.](getserviceconfiguration-operation.md)  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém configurações de serviço.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto será necessário se esse elemento for usado. A tabela a seguir descreve os valores retornados com esse elemento.
  
|Valor|Descrição|
|:-----|:-----|
|NoError  <br/> |Não ocorreu nenhum erro para a solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Esse erro ocorre quando a conta de chamada não tem os direitos para executar a ação solicitada.  <br/> |
|ErrorAccessModeSpecified  <br/> |Esse erro é apenas para uso interno. Esse erro não é retornado.  <br/> |
|ErrorAccountDisabled  <br/> |Esse erro ocorre quando a conta em questão foi desabilitada.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Esse erro ocorre quando uma lista com representantes adicionados não pode ser salva.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Esse erro ocorre quando o registro de espaço de endereço ou o nome de domínio DNS (Sistema de Nomes de Domínio), para disponibilidade entre florestas não pôde ser encontrado no banco de dados do Active Directory.  <br/> |
|ErrorADOperation  <br/> |Esse erro ocorre quando a operação falhou devido a problemas de comunicação com os Serviços de Domínio do Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Esse erro é retornado quando uma solicitação de operação **ResolveNames** especifica um nome que não é válido.  <br/> |
|ErrorADUnavailable  <br/> |Esse erro ocorre quando o AD DS não está disponível. Tente sua solicitação novamente mais tarde.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Esse erro indica que o **atributo AffectedTaskOccurrences** não foi especificado. Quando o elemento [DeleteItem](deleteitem.md) é usado para excluir pelo menos um item que é uma tarefa e, independentemente de essa tarefa ser recorrente ou não, o atributo **AffectedTaskOccurrences** precisa ser especificado para que **DeleteItem** possa determinar se a ocorrência atual ou a série inteira deve ser excluído.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indica um erro na criação de caminho de pasta de arquivo morto.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indica que a caixa de correio de arquivo morto não foi habilitada.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indica que a descoberta do serviço de caixa de correio de arquivo morto falhou.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Especifica que uma tentativa foi feita para criar um item com mais de 10 anexos aninhados. Esse valor foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |O [elemento CreateAttachment](createattachment.md) retornará esse erro se for feita uma tentativa de criar um anexo com tamanho superior a Int32.MaxValue, em bytes.  <br/> O [elemento GetAttachment](getattachment.md) retornará esse erro se uma tentativa de recuperar um anexo existente com tamanho superior a Int32.MaxValue, em bytes.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Esse erro indica que o Exchange Web Services tentou determinar o local de um computador entre florestas que está executando o Exchange 2010 que tem a função de servidor de Acesso para Cliente instalada usando o serviço descoberta automática, mas a chamada para o serviço de Descoberta Automática falhou.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Esse erro indica que as informações de configuração de disponibilidade para a floresta local estão ausentes do AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Esse erro indica que ocorreu uma exceção durante o processamento de um item e essa exceção provavelmente ocorrerá para os itens a seguir. As solicitações podem incluir vários itens; por exemplo, uma solicitação de operação GetItem pode incluir vários identificadores. Em geral, os itens são processados um por vez. Se ocorrer uma exceção durante o processamento de um item e essa exceção provavelmente ocorrer para os itens a seguir, os itens a seguir não serão processados.  <br/><br/>  Veja a seguir exemplos de erros que interromperão o processamento de itens a seguir:<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Esse erro ocorre quando uma tentativa é feita para mover ou copiar uma ocorrência de um item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Esse erro ocorre quando uma tentativa é feita para atualizar um item de calendário localizado na pasta Itens Excluídos e quando as atualizações de reunião ou cancelamentos devem ser enviadas de acordo com o valor do **atributo SendMeetingInvitationsOrCancellations.** <br/><br/>Veja a seguir os valores possíveis para este atributo:  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>No entanto, essa atualização só é permitida quando o valor desse atributo é definido como SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Esse erro ocorre quando a operação UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem é chamada e a ID especificada não é uma ID de ocorrência de qualquer item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Esse erro ocorre quando a operação **UpdateItem**, **GetItem,** **DeleteItem,** **MoveItem,** **CopyItem** ou **SendItem** é chamada e a ID especificada não é uma ID de qualquer item mestre recorrente.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando a duração de um item de calendário é maior do que o máximo permitido, que atualmente é de 5 anos.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Esse erro ocorre quando uma hora de término do calendário é definida para a mesma hora ou após a hora de início.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Esse erro ocorre quando a pasta especificada para uma operação **FindItem** com um [elemento CalendarView](calendarview.md) não é do tipo de pasta de calendário.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando os valores inválidos de Day, WeekendDay e Weekday são usados para definir o padrão de alteração de tempo.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando os valores inválidos de Day, WeekDay e WeekendDay são usados para especificar a recorrência semanal.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Esse erro ocorre quando o estado de um objeto binário de recorrência de item de calendário (BLOB) no Exchange store é inválido.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Esse erro ocorre quando a recorrência especificada não pode ser criada.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Esse erro ocorre quando um fuso horário inválido é encontrado.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Este erro Indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Esse erro indica que o [elemento AcceptItem](acceptitem.md) é inválido para um item de calendário ou uma solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Esse erro indica que o [elemento DeclineItem](declineitem.md) é inválido para um item de calendário ou uma solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Esse erro indica que o [elemento RemoveItem](removeitem.md) é inválido para um cancelamento de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Esse erro indica que o [elemento TentativelyAcceptItem](tentativelyacceptitem.md) é inválido para um item de calendário ou solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Esse erro indica que a operação (atualmente CancelItem) no item de calendário não é válida para um participante. Somente o organizador da reunião pode cancelar a reunião.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Esse erro indica que [AcceptItem é](acceptitem.md) inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Esse erro indica que [DeclineItem é](declineitem.md) inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Esse erro indica que [RemoveItem é](removeitem.md) inválido para o item de calendário do organizador. Para remover uma reunião do calendário, o organizador deve usar CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Esse erro indica que [TentativelyAcceptItem](tentativelyacceptitem.md) é inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Esse erro indica que uma solicitação de reunião está des date e não pode ser atualizada.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Esse erro indica que o índice de ocorrência não aponta para uma ocorrência dentro da recorrência atual. Por exemplo, se o padrão de recorrência definir um conjunto de três ocorrências de reunião e você tentar acessar a quinta ocorrência, esse código de resposta resultará.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Esse erro indica que qualquer operação em uma ocorrência excluída (endereçada por meio da ID mestra recorrente e do índice de ocorrência) é inválida.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Esse erro é relatado nas operações CreateItem e UpdateItem para itens de calendário ou propriedades de recorrência de tarefa quando o valor da propriedade está fora do intervalo. Por exemplo, especificar a décima quinta semana do mês resultará nesse código de resposta.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Esse erro ocorre quando o intervalo Start to End do [elemento CalendarView](calendarview.md) é mais do que o máximo permitido, atualmente 2 anos.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Esse erro indica que a conta solicitante não é uma conta válida no banco de dados de diretório.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indica que foi feita uma tentativa de arquivar uma pasta de tarefas de contato de calendário.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indica que foi feita uma tentativa de arquivar itens em pastas públicas.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indica que foi feita uma tentativa de arquivar itens na caixa de correio de arquivo morto.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Esse erro ocorre quando um item de calendário está sendo criado e o atributo **SavedItemFolderId** se refere a uma pasta não calendário.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Esse erro ocorre quando um contato está sendo criado e o atributo **SavedItemFolderId** se refere a uma pasta sem contato.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Esse erro indica que um item de postagem não pode ser criado em uma pasta diferente de uma pasta de email, como Calendário, Contato, Tarefas, Anotações e assim por diante.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Esse erro ocorre quando uma tarefa está sendo criada e o atributo **SavedItemFolderId** se refere a uma pasta não tarefa.  <br/> |
|ErrorCannotDeleteObject  <br/> |Esse erro ocorre quando o item ou pasta a ser excluído não pode ser excluído.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |A [operação DeleteItem](deleteitem-operation.md) retorna esse erro quando falha ao excluir a ocorrência atual de uma tarefa recorrente. Isso só poderá acontecer se o atributo **AffectedTaskOccurrences** tiver sido definido como SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indica que foi feita uma tentativa de desabilitar uma extensão de obrigações.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Esse erro deve ser retornado quando o servidor não puder esvaziar uma pasta.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indica que o caminho da pasta de origem não pôde ser recuperado.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Especifica que o servidor não pôde recuperar a URL externa para Outlook Web App Opções.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |A **operação GetAttachment** retornará esse erro se não puder recuperar o corpo de um anexo de arquivo.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões de calendário em uma pasta que não seja de calendário.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões que não são de calendário em uma pasta de calendário.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Esse erro indica que você não pode definir permissões desconhecidas em um conjunto de permissões.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indica que foi feita uma tentativa de especificar a pasta de pesquisa como a pasta de origem.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Esse erro ocorre quando uma solicitação que requer um identificador de item recebe um identificador de pasta.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Esse erro ocorre quando uma solicitação que requer um identificador de pasta recebe um identificador de item.  <br/> |
|ErrorChangeKeyRequired  <br/> |Este código de resposta foi substituído por **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Esse erro é retornado quando a chave de alteração de um item está ausente ou está em fases. <br/><br/>Para operações SendItem, UpdateItem e UpdateFolder, o chamador deve passar uma chave de alteração correta e atual para o item. Observe que esse é o caso de UpdateItem mesmo quando a resolução de conflitos é definida como sempre sobregravada.  <br/> |
|ErrorClientDisconnected  <br/> |Especifica que o cliente foi desconectado.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorClientIntentNotFound  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorConnectionFailed  <br/> |Esse erro ocorre quando Exchange Web Services não podem se conectar à caixa de correio.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Este erro indica que a propriedade inspecionada por um filtro Contains não é um tipo de cadeia de caracteres.  <br/> |
|ErrorContentConversionFailed  <br/> |A **operação GetItem** retorna esse erro quando Exchange Web Services não consegue recuperar o conteúdo MIME do item solicitado. <br/><br/>A **operação CreateItem** retorna esse erro quando Exchange Web Services não consegue criar o item do conteúdo MIME fornecido. Normalmente, isso é uma indicação de que a propriedade item está corrompida ou truncada.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Esse erro ocorre quando uma solicitação de pesquisa é feita usando a opção QueryString e a indexação de conteúdo não está habilitada para a caixa de correio de destino.  <br/> |
|ErrorCorruptData  <br/> |Esse erro ocorre quando os dados estão corrompidos e não podem ser processados.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Esse erro ocorre quando o chamador não tem permissão para criar o item.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Esse erro ocorre quando uma ou mais pastas gerenciadas especificadas na solicitação de operação CreateManagedFolder não foram criadas. Pesquise cada pasta para determinar quais pastas foram criadas e quais pastas não existem.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Esse erro ocorre quando a conta de chamada não tem as permissões necessárias para criar a subpasta.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Esse erro ocorre quando uma tentativa é feita para mover um item ou pasta de uma caixa de correio para outra. Se a caixa de correio de origem e a caixa de correio de destino são diferentes, você receberá esse erro.  <br/> |
|ErrorCrossSiteRequest  <br/> |Esse erro indica que a solicitação não é permitida porque o servidor de Acesso para Cliente que deve fazer o serviço da solicitação está em um site diferente.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Esse erro pode ocorrer nos seguintes cenários:<br/>  <br/>- É feita uma tentativa de acessar ou gravar uma propriedade em um item e o valor da propriedade é muito grande.<br/>- O tamanho do conteúdo MIME codificado em base64 dentro do XML de solicitação excede o limite.<br/>- O tamanho do corpo de um corpo de item existente excede o limite.<br/>- O consumidor tenta definir um HTML ou corpo de texto cujo comprimento (ou comprimento combinado no caso de apêndice) excede o limite. |
|ErrorDataSourceOperation  <br/> |Esse erro ocorre quando o provedor de dados subjacente falha ao concluir a operação.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Esse erro ocorre em uma **operação AddDelegate** quando o usuário especificado já existe na lista de representantes.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Esse erro ocorre em uma **operação AddDelegate** quando o usuário especificado a ser adicionado é o proprietário da caixa de correio.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Esse erro ocorre em uma operação **GetDelegate** quando não há informações de representante sobre a mensagem local do FreeBusy ou nenhum representante público do Active Directory (sem "representante público" ou nenhuma entrada "Enviar em nome" no AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Esse erro ocorre quando um usuário especificado não pode ser mapeado para um usuário no AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Esse erro ocorre na operação **AddDelegate** quando um usuário delegado adicionado não é válido.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Esse erro ocorre quando uma tentativa é feita para excluir uma pasta distinta.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Esse erro indica que uma ID de usuário distinta não é válida para a operação. **DistinguishedUserType** não deve estar presente na solicitação.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Esse erro indica que um membro da lista de distribuição de solicitação não existe na lista de distribuição.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Esse erro ocorre quando nomes de pasta duplicados são especificados no [elemento FolderNames](foldernames.md) da solicitação de operação **CreateManagedFolder.**  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Este erro indica que há headers SOAP duplicados.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Esse erro indica que uma ID de usuário duplicada foi encontrada em um conjunto de permissões, padrão ou anônimo são definidos mais de uma vez ou há SIDs ou destinatários duplicados.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Esse erro ocorre quando uma solicitação tenta criar/atualizar os parâmetros de pesquisa de uma pasta de pesquisa. Por exemplo, isso pode ocorrer quando uma pasta de pesquisa é criada na caixa de correio, mas a pasta de pesquisa é direcionada para procurar em outra caixa de correio.  <br/> |
|ErrorEventNotFound  <br/> |Esse erro ocorre quando o evento associado a uma marca d'água é excluído antes que o evento seja retornado. Quando esse erro é retornado, a assinatura também é excluída.  <br/> |
|ErrorExceededConnectionCount  <br/> |Esse erro -iIndica que há mais solicitações simultâneas contra o servidor do que são permitidas pela política de um usuário.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Esse erro indica que a contagem máxima de assinaturas da política de limite de um usuário foi excedida.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Esse erro indica que uma chamada de operação de pesquisa excedeu o número total de itens que podem ser retornados.  <br/> |
|ErrorExpiredSubscription  <br/> |Esse erro ocorrerá se a [operação GetEvents](getevents-operation.md) for chamada como uma assinatura sendo excluída porque ela expirou.  <br/> |
|ErrorExtensionNotFound  <br/> |Indica que a extensão não foi encontrada.  <br/> |
|ErrorFolderCorrupt  <br/> |Esse erro ocorre quando a pasta está corrompida e não pode ser salva.  <br/> |
|ErrorFolderExists  <br/> |Esse erro ocorre quando uma tentativa é feita para criar uma pasta com o mesmo nome que outra pasta no mesmo pai. Nomes de pastas duplicados não são permitidos.  <br/> |
|ErrorFolderNotFound  <br/> |Esse erro indica que a ID da pasta especificada não corresponde a uma pasta válida ou que o representante não tem permissão para acessar a pasta.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Esse erro indica que a propriedade solicitada não pôde ser recuperada. Isso não indica que a propriedade não existe, mas que a propriedade foi corrompida de alguma forma para que a recuperação falhasse.  <br/> |
|ErrorFolderSave  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSaveFailed  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a valores de propriedade inválidos. O código de resposta lista quais propriedades causaram o problema.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Esse erro indica que a contagem máxima de membros do grupo foi atingida para obter informações de livre/ocupado para uma lista de distribuição.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Esse erro é retornado quando as informações de livre/ocupado não podem ser recuperadas devido a uma falha de intervenção.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorImContactLimitReached  <br/> |Esse erro é retornado quando novos contatos de mensagens instantâneas (IM) não podem ser adicionados porque o número máximo de contatos foi atingido. Esse erro foi introduzido no Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Esse erro é retornado quando uma tentativa é feita para adicionar um nome de exibição de grupo quando um grupo existente já tem o mesmo nome de exibição. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Esse erro é retornado quando novos grupos de mensagens IM não podem ser adicionados porque o número máximo de grupos foi atingido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |O erro é retornado no caso de autorização de servidor para servidor para Exchange representação quando o chamador não tem os direitos apropriados para representar o usuário específico em questão. Esse erro é mapeado para o direito estendido do Active Directory ms-Exch-EPI-May-Impersonate.  <br/> |
|ErrorImpersonationDenied  <br/> |Esse erro é retornado na autorização de servidor para servidor para Exchange Representação quando o chamador não tem os direitos apropriados para representar por meio do servidor de Acesso para Cliente em que está fazendo a solicitação. Isso mapeia para o direito estendido do Active Directory ms-Exch-EPI-Impersonation.  <br/> |
|ErrorImpersonationFailed  <br/> |Esse erro indica que houve um erro inesperado quando foi feita uma tentativa de executar a autenticação de servidor para servidor. Esse código de resposta normalmente indica que a conta de serviço que está executando o pool de aplicativos Exchange Web Services está configurada incorretamente, que os Serviços Web do Exchange não podem falar com o diretório ou que uma confiança entre florestas não está configurada corretamente.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Esse erro indica que a solicitação era válida para a versão Exchange Server atual, mas era inválida para a versão do servidor de solicitação especificada.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Esse erro indica que cada descrição de alteração nos [elementos UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) deve listar apenas uma propriedade a ser atualizada.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Esse erro ocorre quando a solicitação contém muitos participantes para resolver. Por padrão, o número máximo de participantes a resolver é 100.  <br/> |
|ErrorInsufficientResources  <br/> |Esse erro ocorre quando o servidor de caixa de correio é sobrecarregado. Tente sua solicitação novamente mais tarde.  <br/> |
|ErrorInternalServerError  <br/> |Esse erro indica que Exchange Web Services encontrou um erro do que não pôde recuperar, e um código de resposta mais específico associado ao erro que ocorreu não existe.  <br/> |
|ErrorInternalServerTransientError  <br/> |Esse erro indica que ocorreu um erro de servidor interno e que você deve tentar sua solicitação novamente mais tarde.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Esse erro indica que o nível de acesso que o chamador tem nos dados de livre/ocupado é inválido.  <br/> |
|ErrorInvalidArgument  <br/> |Este erro indica um erro causado por todos os argumentos inválidos passados para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Este erro é retornado nos seguintes cenários: <br/><br/>- O usuário especificado no parâmetro  _sending-as_ não existe no diretório. <br/>- O usuário especificado no parâmetro  _sending-as_ não é exclusivo no diretório. <br/>- O  _endereço de envio como_ está vazio.<br/>- O  _endereço de envio como_ não é um endereço de email válido.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Esse erro é retornado pela operação [GetAttachment](getattachment-operation.md) ou pela operação [DeleteAttachment](deleteattachment-operation.md) quando um anexo que corresponde à ID especificada não é encontrado.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Esse erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexos complexa. Exchange Os Serviços Web só suportam filtros simples que contêm filtros na tabela de anexos. Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexos mais complexa (um subfiltro), os Serviços Web do Exchange não poderão renderizar o XML para esse filtro e retornarão esse código de resposta. <br/><br/>Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitar o [elemento SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Esse erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexos complexa. Exchange Os Serviços Web só suportam filtros simples que contêm filtros na tabela de anexos. <br/><br/>Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexos mais complexa Exchange, os Serviços Web não poderão renderizar o XML desse filtro. Nesse caso, o subfiltro de anexo contém um filtro de texto, mas não está olhando para o nome de exibição do anexo.<br/><br/> Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitar o [elemento SearchParameters.](searchparameters.md)  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Esse erro indica que o procedimento de autorização do solicitante falhou.  <br/> |
|ErrorInvalidChangeKey  <br/> |Esse erro ocorre quando um consumidor passa um identificador de pasta ou item com uma chave de alteração que não pode ser analisado. Por exemplo, pode ser conteúdo base64 inválido ou uma cadeia de caracteres vazia.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Esse erro indica que houve um erro interno quando uma tentativa foi feita para resolver a identidade do chamador.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Esse erro é retornado quando uma tentativa é feita para definir o valor do elemento [CompleteDate](completedate.md) de uma tarefa para um tempo no futuro. Quando ele é convertido para a hora local do servidor de Acesso para Cliente, o [CompleteDate](completedate.md) de uma tarefa não pode ser definido como um valor posterior ao horário local no servidor de Acesso para Cliente.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Esse erro indica que um endereço de email inválido foi fornecido para um contato.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Esse erro indica que um valor de índice de email inválido foi fornecido para uma entrada de email.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Esse erro ocorre quando as credenciais usadas para fazer proxy de uma solicitação para uma autenticação de falha de uma floresta de serviço de diretório diferente.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Esse erro indica que as permissões de pasta especificadas são inválidas.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Esse erro indica que a ID do usuário delegada especificada é inválida.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Esse erro ocorre durante Exchange Representação quando um chamador não especifica um UPN, um endereço de email ou um SID de usuário. Isso também ocorrerá se o chamador especificar um ou mais desses e os valores estão vazios.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Esse erro ocorre quando a máscara de bits passada para uma restrição de elemento [Excludes](excludes.md) não pode ser analisado.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Esse erro ocorre quando os seguintes eventos ocorrem: <br/> <br/>- O chamador tenta usar uma propriedade estendida que não é suportada pelos Serviços Web Exchange Web.  <br/>- O chamador passa uma combinação inválida de valores de atributo para uma propriedade estendida. Isso também ocorrerá se nenhum atributos for passado. Somente determinadas combinações são permitidas.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Esse erro ocorre quando a seção valor de uma propriedade estendida não corresponder ao tipo da propriedade. <br/><br/>Por exemplo, definir uma propriedade estendida que tenha PropertyType="String" como uma matriz de inteiros resultará nesse erro. Qualquer representação de cadeia de caracteres que não seja coercível no tipo especificado para a propriedade estendida dará esse erro.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Esse erro indica que o remetente do convite de compartilhamento não criou os metadados do convite de compartilhamento.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Esse erro indica que uma mensagem de compartilhamento não se destina ao chamador.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Esse erro indica que os objetos de federação da organização do solicitante não estão configurados corretamente.  <br/> |
|ErrorInvalidFolderId  <br/> |Esse erro ocorre quando a ID da pasta está corrompida.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Esse erro indica que o tipo de pasta especificado é inválido para a operação atual. Por exemplo, você não pode criar uma pasta de Pesquisa em uma pasta pública.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Esse erro ocorre na paja fracional quando o usuário especificou um dos seguintes: <br/> <br/>- Um numerador maior que o denominador  <br/>- Um numerador menor que zero  <br/>- Um denominador menor ou igual a zero  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Esse erro indica que os [elementos DataType](datatype.md) e ShareFolderId estão presentes em uma solicitação.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Esse erro ocorre quando a [operação GetUserAvailability](getuseravailability-operation.md) é chamada com [um FreeBusyViewType](freebusyviewtype.md) de None.  <br/> |
|ErrorInvalidId  <br/> |Esse erro indica que a ID e/ou tecla de alteração está malformada.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Esse erro ocorre quando o chamador especifica um **atributo Id** que está vazio.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Esse erro ocorre quando o item não pode ser curtido. As versões Exchange a partir do número de com build 15.00.0913.09 incluem esse valor.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Esse erro ocorre quando o chamador especifica um **atributo Id** que está malformado.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Este erro indica que uma ID de pasta ou item que está usando o formato Exchange 2007 foi especificada para uma solicitação com uma versão do Exchange 2007 SP1 ou posterior. Você não pode usar Exchange IDs 2007 em Exchange 2007 SP1 ou solicitações posteriores. Você precisa usar a operação [ConvertId para](convertid-operation.md) convertê-las primeiro.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Esse erro ocorre quando o chamador especifica um **atributo Id** muito longo.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Esse erro é retornado sempre que uma ID que não é uma ID de anexo de item é passada para um método de serviço Web que espera uma ID de anexo.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Esse erro ocorre quando um contato em sua caixa de correio está corrompido.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Esse erro ocorre quando o chamador especifica um **atributo Id** muito longo.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Esse erro é retornado quando a hierarquia de anexos em um item excede o máximo de 255 níveis de profundidade.  <br/> |
|ErrorInvalidIdXml  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidImContactId  <br/> |Esse erro é retornado quando o identificador de contato de IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Esse erro é retornado quando o identificador de endereço SMTP do grupo de distribuição de mensagens IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Esse erro é retornado quando o identificador de grupo de mensagens IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Esse erro ocorrerá se o deslocamento para pajamento indexado for negativo.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indica que o item era inválido para uma **operação ArchiveItem.**  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Esse erro ocorre quando uma tentativa é feita para usar um objeto de resposta AcceptItem para um tipo de item diferente de uma solicitação de reunião ou um item de calendário, ou quando uma tentativa é feita para aceitar uma ocorrência de item de calendário que está na pasta Itens Excluídos.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Esse erro ocorre quando uma tentativa é feita para usar um objeto de resposta CancelItem em um tipo de item diferente de um item de calendário.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Esse erro é retornado quando uma tentativa é feita para criar um anexo de item de um tipo sem suporte.  <br/><br/>  Os tipos de item com suporte para anexos de item incluem os seguintes objetos:  <br/><br/>- [Item](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Contato](contact.md) <br/> <br/> Por exemplo, se você tentar criar um anexo [MeetingMessage,](meetingmessage.md) encontrará esse código de resposta.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Esse erro será retornado de uma [operação CreateItem](createitem-operation.md) se a solicitação contiver um tipo de item sem suporte. <br/><br/>Os itens com suporte incluem os seguintes objetos:<br/>  <br/>- [Item](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Contato](contact.md) <br/><br/>  Determinados tipos são criados como um efeito colateral de fazer outra coisa. As mensagens de reunião, por exemplo, são criadas quando você envia um item de calendário para os participantes; eles não são criados explicitamente.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Esse erro ocorre quando uma tentativa é feita para usar um objeto de resposta DeclineItem para um tipo de item diferente de uma solicitação de reunião ou um item de calendário, ou quando uma tentativa é feita para recusar uma ocorrência de item de calendário que está na pasta Itens Excluídos.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Esse erro indica que a operação [ExpandDL](expanddl-operation.md) é válida somente para listas de distribuição privadas.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Esse erro será retornado de um objeto de resposta RemoveItem se a solicitação especificar um item que não seja um item de cancelamento de reunião.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Esse erro será retornado de uma [operação SendItem](senditem-operation.md) se a solicitação especificar um item que não seja um item de mensagem.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Esse erro ocorre quando uma tentativa é feita para usar [TentativelyAcceptItem](tentativelyacceptitem.md) para um tipo de item diferente de uma solicitação de reunião ou um item de calendário, ou quando uma tentativa é feita para aceitar provisivamente uma ocorrência de item de calendário que está na pasta Itens Excluídos.  <br/> |
|ErrorInvalidLogonType  <br/> |Esse erro é apenas para uso interno. Esse erro não é retornado.  <br/> |
|ErrorInvalidMailbox  <br/> |Esse erro indica que a operação [CreateItem](createitem-operation.md) ou [a operação UpdateItem](updateitem-operation.md) falhou ao criar ou atualizar uma lista de distribuição pessoal.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Esse erro ocorre quando a estrutura da pasta gerenciada está corrompida e não pode ser renderizada.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Esse erro ocorre quando a cota definida na pasta gerenciada é menor que zero, o que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Esse erro ocorre quando o tamanho definido na pasta gerenciada é menor que zero, o que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Esse erro ocorre quando o valor interno mesclado/ocupado fornecido é inválido. O valor mínimo padrão é 5 minutos. O valor máximo padrão é 1440 minutos.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Esse erro ocorre quando o nome é inválido para a [operação ResolveNames.](resolvenames-operation.md) Por exemplo, uma cadeia de caracteres de comprimento zero, um único espaço, uma vírgula e um traço são todos nomes inválidos.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Esse erro indica um erro na conta de Serviço de Rede no servidor de Acesso para Cliente.  <br/> |
|ErrorInvalidOofParameter  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidOperation  <br/> | Este é um erro geral que é usado quando a operação solicitada é inválida. <br/><br/>Por exemplo, você não pode fazer o seguinte: <br/> <br/>- Execute uma atravessação "Profunda" usando a operação [FindFolder](findfolder-operation.md) em uma pasta pública.  <br/>- Mover ou copiar a raiz da pasta pública.  <br/>- Exclua um item associado usando qualquer modo, exceto a exclusão "Hard".  <br/>- Mover ou copiar um item associado.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Esse erro indica que um chamador solicitou informações de livre/ocupado para um usuário em outra organização, mas a relação organizacional não tem o tempo livre/ocupado habilitado.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Esse erro ocorre quando um consumidor passa um valor zero ou negativo para que as linhas máximas sejam retornadas.  <br/> |
|ErrorInvalidParentFolder  <br/> |Esse erro ocorre quando um consumidor passa em uma pasta pai inválida para uma operação. Por exemplo, esse erro será retornado se você tentar criar uma pasta em uma pasta de pesquisa.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Esse erro é retornado quando uma tentativa é feita para definir uma porcentagem de conclusão da tarefa como um valor inválido. O valor deve estar entre 0 e 100 (inclusive).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Esse erro indica que o nível de permissão é inconsistente com as configurações de permissão.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Esse erro indica que o identificador do chamador não é válido.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Esse erro indica que o número de telefone não está correto ou não se encaixa nas regras do plano de discagem.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Esse erro ocorre quando a propriedade à que você está tentando anexar não oferece suporte à anexação. <br/><br/>A seguir estão as únicas propriedades que suportam a seguinte situação: <br/> <br/>- Coleções de destinatários (ToRecipients, CcRecipients, BccRecipients)  <br/>- Coleções de participantes (RequiredAttendees, OptionalAttendees, Resources)  <br/>- Corpo  <br/>- ReplyTo  <br/><br/>  Além disso, esse erro ocorre quando um corpo da mensagem é anexado se o formato especificado na solicitação não corresponder ao formato do item na loja.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Esse erro ocorrerá se a operação de exclusão for especificada em uma operação [UpdateItem](updateitem-operation.md) ou chamada de operação [UpdateFolder](updatefolder-operation.md) para uma propriedade que não dá suporte à operação de exclusão. Por exemplo, não é possível excluir o [elemento ItemId](itemid.md) do [objeto Item.](item.md)  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Esse erro ocorrerá se o consumidor passar em uma das propriedades de sinalizador em um [filtro Exists.](exists.md) Por exemplo, esse erro ocorrerá se os [sinalizadores IsRead](isread.md) ou [IsFromMe](isfromme.md) são especificados no [elemento Exists.](exists.md) A solicitação deve usar o [elemento IsEqualTo](isequalto.md) em vez disso, pois são sinalizadores e, portanto, parte de uma única propriedade.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Esse erro ocorre quando a propriedade que você está tentando manipular não dá suporte à operação que está sendo executada nele.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Esse erro ocorrerá se uma propriedade especificada na solicitação não estiver disponível para o tipo de item. Por exemplo, esse erro será retornado se uma propriedade que está disponível apenas em itens de calendário for solicitada em uma chamada de operação [GetItem](getitem-operation.md) para uma mensagem ou for atualizada em uma chamada de operação [UpdateItem](updateitem-operation.md) para uma mensagem. <br/> <br/>  Isso ocorre nas seguintes operações: <br/> <br/>- [Operação GetItem](getitem-operation.md) <br/>- [Operação GetFolder](getfolder-operation.md) <br/>- [Operação UpdateItem](updateitem-operation.md) <br/>- [Operação UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Esse erro indica que a propriedade que você está tentando manipular não dá suporte à operação que está sendo executada nele. Por exemplo, esse erro será retornado se a propriedade que você está tentando definir for somente leitura.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Esse erro ocorre durante uma [operação UpdateItem](updateitem-operation.md) quando um cliente tenta atualizar determinadas propriedades de uma mensagem que já foi enviada.<br/><br/> Por exemplo, as seguintes propriedades não podem ser atualizadas em uma mensagem enviada: <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Esse erro ocorrerá se você chamar a [operação GetEvents](getevents-operation.md) ou a operação [Cancelar](unsubscribe-operation.md) assinatura usando uma ID de assinatura por push. Para cancelar a assinatura de uma assinatura por push, você deve responder a uma solicitação por push com uma resposta de cancelamento de assinatura ou desconectar seu serviço Web e aguardar o tempo de espera das notificações por push.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Esse erro é retornado pela operação [Assinar](subscribe-operation.md) quando cria uma assinatura "push" e indica que a URL incluída na solicitação é inválida.<br/><br/>As seguintes condições devem ser atendidas para que Exchange Web Services aceitem a URL: <br/> <br/>- Comprimento da \> cadeia de caracteres 0 \< 2083.  <br/> e - Protocolo é http ou https.  <br/>- A URL pode ser analisado pela classe URI Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Esse erro indica que a coleção de destinatários em sua mensagem ou a coleção attendee em seu item de calendário é inválida. Por exemplo, esse erro será retornado quando uma tentativa for feita para enviar um item que não tenha destinatários.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que Exchange Web Services não podem representar. Para evitar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que Exchange Web Services não podem representar. Para evitar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que Exchange Web Services não podem representar. Para evitar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que Exchange Web Services não podem representar. Para evitar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Este erro é retornado da operação [CreateItem para](createitem-operation.md) objetos de resposta Forward e Reply nos seguintes cenários:<br/>  <br/>- O identificador de item referenciado não é [um Message](message-ex15websvcsotherref.md), um [CalendarItem](calendaritem.md)ou um descendente de **uma Mensagem** ou **CalendarItem**.  <br/>- O identificador de item de referência é para **um CalendarItem** e o organizador está tentando responder ou ReplyAll para si mesmo.  <br/>- A mensagem é um rascunho e Reply ou ReplyAll está selecionado.  <br/>- O item de referência, [para SuppressReadReceipt](suppressreadreceipt.md), não é **uma Mensagem** ou um descendente de uma **Mensagem**.  <br/> |
|ErrorInvalidRequest  <br/> |Esse erro ocorre quando a solicitação SOAP tem um header de ação SOAP, mas nada no corpo SOAP. Observe que o header ação SOAP não é necessário, pois os Serviços Web Exchange podem determinar o método a ser chamado a partir do nome local do elemento raiz no corpo SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Esse erro é retornado quando a marca de retenção especificada tem uma ação incorreta associada a ela. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Esse erro é retornado quando uma tentativa é feita para definir uma marca inexistente ou invisível em uma **propriedade PolicyTag.** Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Esse erro é retornado quando uma tentativa é feita para definir uma marca implícita na **propriedade PolicyTag.** Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indica que o GUID da marca de retenção era inválido.  <br/> |
|ErrorInvalidRoutingType  <br/> |Esse erro ocorrerá se o tipo de roteamento passado para um elemento [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) for inválido. Normalmente, o tipo de roteamento é definido como SMTP (Simple Mail Transfer Protocol).  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Esse erro ocorrerá se a hora de término da duração especificada não for maior do que a hora de início ou se a hora de término não ocorrer no futuro.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Esse erro indica que uma solicitação de proxy que foi enviada a outro servidor não é capaz de fazer o serviço da solicitação devido a uma incompatibilidade de versão.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Esse erro indica que o descritor Exchange de segurança na pasta Calendário no armazenamento está corrompido.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Esse erro ocorre durante uma tentativa de enviar um item em que [SavedItemFolderId](saveditemfolderid.md) é especificado na solicitação, mas a **propriedade SaveItemToFolder** é definida como **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Esse erro indica que o token passado no header está malformado, não se refere a uma conta válida no diretório ou está faltando o grupo principal **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Esse erro indica que os metadados de compartilhamento não são válidos. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorInvalidSid  <br/> |Esse erro ocorre quando um SID inválido é passado em uma solicitação.  <br/> |
|ErrorInvalidSIPUri  <br/> |Esse erro indica que o nome SIP, o plano de discagem ou o número de telefone são URIs SIP inválidos.  <br/> |
|ErrorInvalidServerVersion  <br/> |Esse erro indica que uma versão inválida do servidor de solicitação foi especificada na solicitação.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Esse erro ocorre quando o endereço SMTP não pode ser analisado.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidSubscription  <br/> |Esse erro indica que a assinatura não é mais válida. Isso pode ser porque o servidor de Acesso para Cliente está sendo reiniciado ou porque a assinatura expirou.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Esse erro indica que a solicitação de assinatura incluiu várias IDs de pasta pública. Uma assinatura pode incluir várias pastas da mesma caixa de correio ou uma ID de pasta pública.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Esse erro é retornado por [SyncFolderItems](syncfolderitems.md) ou [SyncFolderHierarchy](syncfolderhierarchy.md) se os dados [SyncState](syncstate-ex15websvcsotherref.md) passados for inválido. Para corrigir esse erro, você deve ressincronizar sem o estado de sincronização. Certifique-se de que, se você estiver persistindo bloBs de estado de sincronização, não está truncando acidentalmente o BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Esse erro indica que o intervalo de tempo especificado é inválido. A hora de início deve ser maior ou igual à hora de término.  <br/> |
|ErrorInvalidUserInfo  <br/> |Esse erro indica que um [UserId](userid.md) inconsistente internamente foi especificado para uma operação de permissões. Por exemplo, se uma ID de usuário distinta for especificada (Padrão ou Anônimo), esse erro será retornado se você também tentar especificar um SID, ou endereço SMTP principal ou nome de exibição para esse usuário.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Esse erro indica que as configurações do usuário Fora do Office (OOF) são inválidas devido a uma resposta interna ou externa ausente.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Esse erro ocorre durante Exchange Representação. O chamador passou em um UPN inválido no header SOAP que não estava acessível no diretório.  <br/> |
|ErrorInvalidUserSid  <br/> |Esse erro ocorre quando um SID inválido é passado em uma solicitação.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Esse erro indica que o valor de comparação na restrição é inválido para a propriedade que você está comparando.<br/><br/> Por exemplo, o valor de comparação de [DateTimeCreated](datetimecreated.md)  >  **true** retornaria esse código de resposta. <br/><br/>Esse código de resposta também será retornado se você especificar uma propriedade de enumeração na comparação, mas o valor que você está comparando não é um valor válido para essa enumeração.  <br/> |
|ErrorInvalidWatermark  <br/> |Esse erro é causado por uma marca d'água inválida.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Esse erro indica que um gateway VoIP válido não está disponível.  <br/> |
|ErrorIrresolvableConflict  <br/> |Esse erro indica que a resolução de conflitos não pôde resolver alterações para as propriedades. Os itens na loja podem ter sido alterados e devem ser atualizados. Recupere a chave de alteração atualizada e tente novamente.  <br/> |
|ErrorItemCorrupt  <br/> |Esse erro indica que o estado do objeto está corrompido e não pode ser recuperado. Quando você estiver recuperando um item, apenas determinados elementos estarão nesse estado, como [Body](body.md) e [MimeContent](mimecontent.md). Omita esses elementos e repetir a operação.  <br/> |
|ErrorItemNotFound  <br/> |Esse erro ocorre quando o item não foi encontrado ou você não tem permissão para acessar o item.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Esse erro ocorrerá se uma solicitação de propriedade em um item falhar. A propriedade pode existir, mas não pôde ser recuperada.  <br/> |
|ErrorItemSave  <br/> |Esse erro ocorre quando as tentativas de salvar o item ou pasta falham.  <br/> |
|ErrorItemSavePropertyError  <br/> |Esse erro ocorre quando as tentativas de salvar o item ou pasta falham devido a valores de propriedade inválidos. O código de resposta inclui o caminho das propriedades inválidas.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Esse erro indica que o serviço de Disponibilidade não pôde fazer logoff como o serviço de rede para solicitações de proxy para os sites ou florestas apropriados. Normalmente, essa resposta indica um erro de configuração.  <br/> |
|ErrorMailboxConfiguration  <br/> |Esse erro indica que as informações de caixa de correio no AD DS estão configuradas incorretamente.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Esse erro indica que o elemento [MailboxDataArray](mailboxdataarray.md) na solicitação está vazio. Você deve fornecer pelo menos um identificador de caixa de correio.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Esse erro ocorre quando mais de 100 entradas são fornecidas em um [elemento MailboxDataArray..](mailboxdataarray.md)  <br/> |
|ErrorMailboxFailover  <br/> |Esse erro indica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indica que a caixa de correio não foi encontrada.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Esse erro ocorre quando a conexão com a caixa de correio para obter as informações de exibição de calendário falhou.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Esse erro indica que a caixa de correio está sendo movida para um servidor ou armazenamento de caixa de correio diferente. Esse erro também pode indicar que a caixa de correio está em outro servidor ou banco de dados de caixa de correio.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Este erro indica que ocorreu uma das seguintes condições de erro:  <br/><br/>- O armazenamento da caixa de correio está corrompido.  <br/>- O armazenamento da caixa de correio está sendo interrompido.  <br/>- O armazenamento da caixa de correio está offline.  <br/>- Ocorreu um erro de rede quando foi feita uma tentativa de acessar o armazenamento da caixa de correio.  <br/>- O armazenamento da caixa de correio está sobrecarregado e não pode aceitar mais conexões.  <br/>- O armazenamento da caixa de correio foi pausado.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Esse erro ocorrerá se as informações do elemento [MailboxData](mailboxdata.md) não puderem ser mapeadas para uma conta de caixa de correio válida.  <br/> |
|ErrorMailTipsDisabled  <br/> |Esse erro indica que as dicas de email estão desabilitadas.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Esse erro ocorrerá se a pasta gerenciada que você está tentando criar já existir em uma caixa de correio.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Esse erro ocorre quando o nome da pasta especificado na solicitação não mapeia para uma definição de pasta gerenciada no AD DS. Você só pode criar instâncias de pastas gerenciadas para pastas definidas no AD DS. Verifique o nome e tente novamente.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Esse erro indica que a raiz de pastas gerenciadas foi excluída da caixa de correio ou que existe uma pasta na mesma pasta pai que tem o nome da raiz da pasta gerenciada. Isso também ocorrerá se a tentativa de criar a pasta gerenciada raiz falhar.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Esse erro indica que o mecanismo de sugestões encontrou um problema ao tentar gerar as sugestões.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Esse erro ocorrerá se o **atributo MessageDisposition** não estiver definido.<br/><br/> Este atributo é necessário para o seguinte: <br/> <br/>- A [operação CreateItem](createitem-operation.md) e [a operação UpdateItem](updateitem-operation.md) quando o item que está sendo criado ou atualizado é uma [Mensagem](message-ex15websvcsotherref.md).  <br/>- [Objetos de resposta CancelCalendarItem,](cancelcalendaritem.md) [AcceptItem,](acceptitem.md) [DeclineItem](declineitem.md)ou [TentativelyAcceptItem.](tentativelyacceptitem.md)  <br/> |
|ErrorMessageSizeExceeded  <br/> |Esse erro indica que a mensagem que você está tentando enviar excede os limites permitidos.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Esse erro indica que o domínio determinado não pode ser encontrado.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Esse erro indica que o serviço de controle de mensagens não pode rastrear a mensagem.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Esse erro indica que o serviço de controle de mensagens está para baixo ou ocupado. Este código de erro indica um erro transitório. Os clientes podem tentar novamente se conectar ao servidor quando esse erro for recebido.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Esse erro ocorre quando o conteúdo MIME não é um iCal válido para uma [operação CreateItem.](createitem-operation.md) Para uma [operação GetItem,](getitem-operation.md)essa resposta indica que o conteúdo MIME não pôde ser gerado.  <br/> |
|ErrorMimeContentInvalid  <br/> |Esse erro ocorre quando o conteúdo MIME é inválido.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Esse erro ocorre quando o conteúdo MIME na solicitação não é uma cadeia de caracteres base 64 válida.  <br/> |
|ErrorMissingArgument  <br/> |Esse erro indica que um argumento necessário estava ausente na solicitação. O texto da mensagem de resposta indica qual argumento verificar.  <br/> |
|ErrorMissingEmailAddress  <br/> |Esse erro indica que você especificou uma ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um sub-elemento [mailbox](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Esse erro indica que você especificou uma ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um sub-elemento [mailbox](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md). Essa resposta é retornada da [operação CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Esse erro ocorrerá se o [elemento EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) estiver ausente.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Esse erro ocorrerá se [ReferenceItemId](referenceitemid.md) estiver ausente.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Esse código de erro nunca é retornado.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Esse erro é retornado quando uma tentativa é feita para não incluir o elemento item no **elemento ItemAttachment** de uma solicitação de operação [CreateAttachment.](createattachment-operation.md)  <br/> |
|ErrorMissingManagedFolderId  <br/> |Esse erro ocorre quando a propriedade IDs de política, a marca 0x6732, para a pasta está ausente. Considere isso uma pasta corrompida.  <br/> |
|ErrorMissingRecipients  <br/> |Esse erro indica que você tentou enviar um item sem incluir destinatários. Observe que, se você chamar a operação [CreateItem](createitem-operation.md) com uma disposição de mensagem que faz com que a mensagem seja enviada, você receberá o seguinte código de resposta: **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Esse erro indica que um [UserId](userid.md) não foi totalmente especificado em um conjunto de permissões.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Esse erro indica que você especificou mais de um valor de [elemento ExchangeImpersonation](exchangeimpersonation.md) em uma solicitação.  <br/> |
|ErrorMoveCopyFailed  <br/> |Esse erro indica que a operação de movimentação ou cópia falhou. A movimentação ocorre na [operação CreateItem](createitem-operation.md) quando você aceita uma solicitação de reunião que está na pasta Itens Excluídos. Além disso, se você recusar uma solicitação de reunião, cancelar um item de calendário ou remover uma reunião do calendário, ela será movida para a pasta Itens Excluídos.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Esse erro ocorrerá se você tentar mover uma pasta distinta.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Esse erro ocorre quando uma solicitação tenta acessar vários servidores de caixa de correio. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Esse erro ocorrerá se a operação [ResolveNames](resolvenames-operation.md) retornar mais de um resultado ou o nome ambíguo especificado corresponde a mais de um objeto no diretório. O código de resposta inclui os nomes matched nos dados de resposta.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Esse erro indica que o chamador não tem uma caixa de correio no sistema. A [operação ResolveNames ou](resolvenames-operation.md) [ExpandDL](expanddl-operation.md) é inválida para conectar um usuário sem uma caixa de correio.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Esse erro indica que a operação [ResolveNames](resolvenames-operation.md) não retorna resultados.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Esse código de erro DEVE ser retornado quando o serviço Web não puder encontrar um servidor para lidar com a solicitação.  <br/> |
|ErrorNoCalendar  <br/> |Esse erro ocorrerá se não houver nenhuma pasta Calendário para a caixa de correio.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de Acesso para Cliente no site de destino foi configurado para autenticação Windows e, portanto, a solicitação não pôde ser consultada.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de Acesso para Cliente no site de destino foi configurado para conexões SSL e, portanto, a solicitação não pôde ser consultada.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de Acesso para Cliente no site de destino era de uma versão aceitável do produto para receber a solicitação e, portanto, a solicitação não pôde ser consultada.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Esse erro ocorrerá se você definir o [elemento FolderClass](folderclass.md) ao criar um item diferente de uma pasta genérica. Para pastas digitadas, como [CalendarFolder](calendarfolder.md) e [TasksFolder,](tasksfolder.md)a classe folder está implícita. Definir a classe de pasta como um tipo de pasta diferente usando a [operação UpdateFolder](updatefolder-operation.md) resulta na resposta **ErrorObjectTypeChanged.** Em vez disso, use um tipo de pasta genérica, mas de definir a classe de pasta como o valor necessário. Exchange Os Serviços Web criarão a pasta fortemente digitada corretamente.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Esse erro indica que o chamador não tem direitos de exibição de livre/ocupado na pasta Calendário em questão.  <br/> |
|ErrorNonExistentMailbox  <br/> | Esse erro ocorre nos seguintes cenários: <br/> <br/>- O endereço de email está vazio em [CreateManagedFolder](createmanagedfolder.md).  <br/>- O endereço de email não se refere a uma conta válida em uma solicitação que leva um endereço de email no corpo ou no header SOAP, como em uma chamada Exchange Representação.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Esse erro ocorre quando um chamador passa em um endereço SMTP não primário. A resposta inclui o endereço SMTP correto a ser usado.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Esse erro indica que as propriedades MAPI no intervalo personalizado, 0x8000 e superior, não podem ser referenciadas por marcas de propriedade. Você deve usar a propriedade EWS Managed API [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)ou o elemento EWS [ExtendedFieldURI](extendedfielduri.md) com o atributo PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Esse código de erro DEVE ser retornado se nenhum servidor de pasta pública estiver disponível ou se o chamador não tiver um servidor público em casa.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum dos servidores de Acesso para Cliente nesse site respondeu e, portanto, a solicitação não pôde ser consultada.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Esse erro indica que o chamador tentou conceder permissões em seu calendário ou pasta de contatos a um usuário em outra organização, e a tentativa falhou.  <br/> |
|ErrorNotDelegate  <br/> |Esse erro indica que o usuário não é um representante da caixa de correio. Ele é retornado pela operação [GetDelegate,](getdelegate-operation.md)pela operação [RemoveDelegate](removedelegate-operation.md)e pela operação [UpdateDelegate](updatedelegate-operation.md) quando o usuário delegado especificado não é encontrado na lista de representantes.  <br/> |
|ErrorNotEnoughMemory  <br/> |Esse erro indica que a operação não pôde ser concluída devido à memória insuficiente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorObjectTypeChanged  <br/> |Esse erro ocorrerá se o tipo de objeto for alterado.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Esse erro ocorre [](start.md) quando [](end-ex15websvcsotherref.md) a hora inicial ou final de uma ocorrência é atualizada para que a ocorrência seja agendada para acontecer antes ou posterior do que a ocorrência anterior ou próxima correspondente.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Esse erro indica que a loteação de tempo para uma determinada ocorrência se sobrepõe a outra ocorrência do mesmo item recorrente. Essa resposta também ocorre quando o comprimento em minutos de uma determinada ocorrência é maior que Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Esse erro indica que a operação atual não é válida para a raiz da pasta pública.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Esse erro indica que a organização do solicitante não é federada, portanto, o solicitante não pode criar mensagens de compartilhamento para enviar a um usuário externo ou não pode aceitar o compartilhamento de mensagens recebidas de um usuário externo.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorParentFolderNotFound  <br/> |Esse erro ocorre na operação [CreateFolder](createfolder-operation.md) quando a pasta pai não é encontrada.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Esse erro indica que você deve alterar sua senha antes de poder acessar essa caixa de correio. Isso ocorre quando uma nova conta foi criada e o administrador indicou que o usuário deve alterar a senha no primeiro logon. Não é possível atualizar a senha usando Exchange Web Services. Você deve usar uma ferramenta como Microsoft Office Outlook Web App para alterar sua senha.  <br/> |
|ErrorPasswordExpired  <br/> |Esse erro indica que a senha expirou. Não é possível alterar a senha usando Exchange Web Services. Você deve usar uma ferramenta como Outlook Web App para alterar sua senha.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos a um usuário externo, mas a política de compartilhamento atribuída ao solicitante indica que o nível de permissão solicitado é maior do que o que a política de compartilhamento permite.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Esse erro indica que o número de telefone não estava no formulário correto.  <br/> |
|ErrorPropertyUpdate  <br/> |Esse erro indica que a atualização falhou devido a valores de propriedade inválidos. A mensagem de resposta inclui os caminhos de propriedade inválidos.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Esse erro indica que a solicitação se refere a uma assinatura que existe em outro servidor de Acesso para Cliente, mas uma tentativa de proxy da solicitação para esse servidor de Acesso para Cliente falhou.  <br/> |
|ErrorProxyCallFailed  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory e que o chamador original é membro de mais de 3.000 grupos.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Esse erro indica que a solicitação que os Serviços Web Exchange enviados a outro servidor de Acesso para Cliente ao tentar atender a uma solicitação [GetUserAvailabilityRequest](getuseravailabilityrequest.md) era inválida. Esse código de resposta normalmente indica que ocorreu um erro de configuração ou direitos ou que alguém tentou, sem sucesso, imitar uma solicitação de proxy de disponibilidade.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Esse erro indica que Exchange Web Services tentaram fazer proxy de uma solicitação de disponibilidade para outro servidor de Acesso para Cliente para atendimento, mas a solicitação falhou. Essa resposta pode ser causada por problemas de conectividade de rede ou problemas de tempo-de-tempo de solicitação.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Esse código de erro deve ser retornado se o serviço Web não puder determinar se a solicitação deve ser executado no servidor de destino ou se será proxida para outro servidor.  <br/> |
|ErrorProxyTokenExpired  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Esse erro ocorre quando a URL da caixa de correio de pasta pública não pode ser encontrada. Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Esse erro ocorre quando uma tentativa é feita para acessar uma pasta pública e a tentativa não é bem-sucedida. Esse erro foi introduzido no Exchange 2013Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Esse erro ocorre quando o destinatário que foi passado para a operação [GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server que é anterior ao Exchange 2007 e a solicitação para recuperar informações de livre/ocupado para o destinatário do servidor de pasta pública falhou.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Esse erro ocorre quando o destinatário que foi passado para a operação [GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server que é anterior ao Exchange 2007 e a solicitação para recuperar informações de livre/ocupado para o destinatário do servidor de pasta pública falhou porque a unidade organizacional não tinha um servidor de pasta pública associado.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Esse erro ocorre quando uma operação de sincronização é bem-sucedida em relação à caixa de correio de pasta pública principal, mas não é bem-sucedida em relação à caixa de correio de pasta pública secundária. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Esse erro indica que a restrição de pasta de pesquisa pode ser válida, mas não é suportada pelo EWS. Exchange Os Serviços Web limitam restrições para conter no máximo 255 expressões de filtro. Se você tentar se vincular a uma pasta de pesquisa existente que exceda 255, esse código de resposta será retornado.  <br/> |
|ErrorQuotaExceeded  <br/> |Esse erro ocorre quando a cota de caixa de correio é excedida.  <br/> |
|ErrorReadEventsFailed  <br/> |Esse erro é retornado pela operação [GetEvents](getevents-operation.md) ou notificações por push quando ocorre uma falha durante a recuperação de informações de evento. Quando esse erro é retornado, a assinatura é excluída. Re-crie a sincronização de eventos com base em uma última marca d'água conhecida.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Esse erro é retornado pela operação [CreateItem](createitem-operation.md) se uma tentativa foi feita para suprimir um recibo de leitura quando o remetente da mensagem não solicitou um recibo de leitura na mensagem ou se a mensagem está na pasta Lixo Eletrônico.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Esse erro ocorre quando a data de término da recorrência é após 1/9/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Esse erro ocorre quando a recorrência especificada não tem instâncias de ocorrência no intervalo especificado.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Esse erro indica que a lista de representantes falhou ao ser salva após a remoção dos representantes.  <br/> |
|ErrorRequestAborted  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Esse erro ocorre quando o fluxo de solicitação é maior do que 400 KB.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Esse erro é retornado quando uma propriedade necessária está ausente em uma solicitação de operação [CreateAttachment.](createattachment-operation.md) O URI da propriedade ausente está incluído na resposta.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Esse erro indica que o chamador especificou uma pasta que não é uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Esse erro indica que o chamador especificou mais de uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorRestrictionTooLong  <br/> |Esse erro ocorrerá se a restrição contiver mais de 255 nós.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Esse erro ocorre quando a restrição não pode ser avaliada pelos Serviços Web Exchange Web.  <br/> |
|ErrorResultSetTooBig  <br/> |Esse erro indica que o número de entradas de calendário para um determinado destinatário excede o limite permitido de 1000. Reduza a janela e tente novamente.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Esse erro ocorre quando [SavedItemFolderId](saveditemfolderid.md) não é encontrado.  <br/> |
|ErrorSchemaValidation  <br/> | Esse erro ocorre quando a solicitação não pode ser validada em relação ao esquema.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Esse erro indica que a pasta de pesquisa foi criada, mas os critérios de pesquisa nunca foram definidos na pasta. Isso só ocorre quando você acessa pastas de pesquisa corrompidas que foram criadas usando outra API ou cliente. Para corrigir esse erro, use a [operação UpdateFolder](updatefolder-operation.md) para definir o [elemento SearchParameters](searchparameters.md) para incluir a restrição que deve estar na pasta.  <br/> |
|ErrorSendAsDenied  <br/> | Esse erro ocorre quando ocorrem ambas as seguintes condições: <br/> <br/>- Um usuário recebeu permissões CanActAsOwner, mas não recebe direitos de representante na caixa de correio da entidade.  <br/>- O mesmo usuário tenta criar e enviar uma mensagem de email na caixa de correio da entidade usando a opção SendAndSaveCopy.<br/>  <br/>  O resultado é um erro ErrorSendAsDenied e a criação da mensagem de email na pasta Rascunhos da entidade.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Esse erro será retornado pela operação [DeleteItem](deleteitem-operation.md) se o atributo **SendMeetingCancellations** estiver ausente da solicitação e o item a ser excluído for um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Esse erro será retornado pela [operação UpdateItem](updateitem-operation.md) se o atributo **SendMeetingInvitationsOrCancellations** estiver ausente da solicitação e o item a ser atualizado for um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Esse erro será retornado pela operação [CreateItem](createitem-operation.md) se o atributo **SendMeetingInvitations** estiver ausente da solicitação e o item a ser criado for um item de calendário.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Esse erro indica que, após o organizador enviar uma solicitação de reunião, a solicitação não poderá ser atualizada. Para modificar a reunião, modifique o item de calendário, não a solicitação de reunião.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Esse erro indica que, após o iniciador da tarefa enviar uma solicitação de tarefa, essa solicitação não poderá ser atualizada.  <br/> |
|ErrorServerBusy  <br/> |Esse erro ocorre quando o servidor está ocupado.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Esse erro indica que Exchange Web Services tentou fazer proxy de uma solicitação de disponibilidade do usuário para a floresta apropriada para o destinatário, mas não foi possível determinar para onde enviar a solicitação devido a uma falha de descoberta de serviço.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Esse erro indica que a propriedade URL externa não foi definida no banco de dados do Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Esse erro indica que falhou uma tentativa de sincronização de uma pasta de compartilhamento. <br/><br/>Este código de erro é retornado quando o seguinte ocorre:<br/><br/>- A assinatura de uma pasta de compartilhamento não foi encontrada.<br/>- A pasta de compartilhamento não foi encontrada.<br/>- O usuário de diretório correspondente não foi encontrado.<br/>- O usuário não existe mais.<br/>- O compromisso é inválido.<br/>- O item de contato é inválido.<br/>- Há uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorStaleObject  <br/> |Esse erro ocorre em uma operação [UpdateItem](updateitem-operation.md) ou em uma operação [SendItem](senditem-operation.md) quando a chave de alteração não está atualizada ou não foi fornecida. Chame a [operação GetItem](getitem-operation.md) para recuperar uma chave de alteração atualizada e tente a operação novamente.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Este erro Indica que um usuário não pode enviar imediatamente mais solicitações porque a cota de envio foi atingida.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Esse erro ocorre quando você tenta acessar uma assinatura usando uma conta que não criou essa assinatura. Cada assinatura só pode ser acessada pelo criador da assinatura.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Esse erro indica que não é possível criar uma assinatura se você não for o proprietário ou se não tiver acesso do proprietário à caixa de correio.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Esse erro ocorrerá se a assinatura que corresponde ao [SubscriptionId especificado (GetEvents)](subscriptionid-getevents.md) não for encontrada. A assinatura pode ter expirado, o processo Exchange Web Services pode ter sido reiniciado ou uma assinatura inválida foi passada. Se a assinatura for válida, re-crie a assinatura com a marca d'água mais recente. Isso é retornado pela operação [Unsubscribe ou](unsubscribe-operation.md) pelas respostas da operação [GetEvents.](getevents-operation.md)  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Esse código de erro deve ser retornado quando uma solicitação for feita para uma assinatura que foi descriada.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Esse erro será retornado pela operação [SyncFolderItems](syncfolderitems-operation.md) se a pasta pai especificada não puder ser encontrada.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Esse erro indica que uma caixa de correio de equipe não foi encontrada. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas que ela não está vinculada a um SharePoint Server. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas que o link para o servidor SharePoint não é válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Esse código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Esse código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Esse erro indica que uma tentativa de enviar uma notificação aos proprietários da caixa de correio da equipe não foi bem-sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Esse erro indica um erro geral que pode ocorrer ao tentar acessar uma caixa de correio de equipe. Tente enviar a solicitação posteriormente. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Esse erro indica que a janela de tempo especificada é maior do que o limite permitido. Por padrão, o limite permitido é 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Esse erro ocorre quando não há tempo suficiente para concluir o processamento da solicitação.  <br/> |
|ErrorTimeZone  <br/> |Esse erro indica que há um erro de fuso horário.  <br/> |
|ErrorToFolderNotFound  <br/> |Esse erro indica que a pasta de destino não existe.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Esse erro ocorrerá se o chamador tentar fazer uma solicitação de serialização de Token, mas não tiver a ms-Exch-EPI-TokenSerialization direita no servidor de Acesso para Cliente.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Esse erro ocorre quando o limite interno em objetos abertos foi excedido.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Esse erro indica que o plano de discagem de um usuário não está disponível.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Esse erro indica que o usuário não foi encontrado.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Esse erro indica que um servidor válido para o plano de discagem pode ser encontrado para lidar com a solicitação.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Esse erro ocorre quando uma tentativa malsucedida é feita para remover um contato de mensagens de um grupo. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Esse erro ocorre quando você tenta definir a propriedade **Culture** como um valor que não é analisado pela **classe System.Globalization.CultureInfo.**  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Esse erro ocorre quando um chamador tenta usar propriedades estendidas de objetos de tipos, matriz de objeto, erro ou nulo.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Esse erro ocorre quando você está tentando recuperar ou definir conteúdo MIME para um item diferente de [um objeto PostItem,](postitem.md) [Message](message-ex15websvcsotherref.md)ou [CalendarItem.](calendaritem.md)  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Esse erro ocorre quando o chamador passa uma propriedade inválida para uma consulta. Isso pode ocorrer quando as propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Esse erro ocorre quando o chamador passa uma propriedade inválida para uma classificação ou grupo por propriedade. Isso pode ocorrer quando as propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Esse erro indica que a restrição de pasta de pesquisa pode ser válida, mas não é suportada pelo EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Esse erro indica que a recorrência especificada não é suportada para tarefas.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Esse erro indica que Exchange Web Services encontrou um tipo de propriedade no armazenamento, mas não pode gerar XML para o tipo de propriedade.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Esse erro indica que a lista de representantes falhou ao ser salva depois que os representantes foram atualizados.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Esse erro ocorre quando o caminho de propriedade única listado em uma descrição de alteração não corresponderá à única propriedade que está sendo definida dentro do [objeto Item](item.md) ou [Pasta](folder.md) real.  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Esse erro indica que o solicitante não está habilitado.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos a um usuário externo, mas a política de compartilhamento atribuída ao solicitante indica que o domínio do usuário externo não está listado na política.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indica que a organização do solicitante tem um conjunto de domínios federados, mas a organização do solicitante não tem endereços proxy SMTP com um dos domínios federados.  <br/> |
|ErrorValueOutOfRange  <br/> |Este erro indica que uma data de início ou data de término do calendário foi definida como 1/1/0001 12:00:00 ou 31/12/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Esse erro indica que o Exchange local detectou um vírus na mensagem.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Esse erro indica que o Exchange o armazenamento detectou um vírus na mensagem e o excluiu.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorWin32InteropError  <br/> |Esse erro indica que houve uma falha interna durante a comunicação com o código não-administrativo.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Esse código de resposta não é usado.  <br/> |
|ErrorWrongServerVersion  <br/> |Esse erro indica que uma solicitação só pode ser feita em um servidor que seja a mesma versão do servidor de caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Esse erro indica que uma solicitação foi feita por um representante que tem uma versão de servidor diferente do servidor de caixa de correio da entidade.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Esse código de erro nunca é retornado.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Especifica que há headers SOAP duplicados.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Especifica que uma tentativa de sincronização de uma pasta de compartilhamento falhou.<br/><br/> Este código de erro DEVE ser retornado quando:<br/><br/>- A assinatura de uma pasta de compartilhamento não foi encontrada.  <br/>- A pasta de compartilhamento não foi encontrada.  <br/>- O usuário de diretório correspondente não foi encontrado.  <br/>- O usuário não existe mais.  <br/>- O compromisso é inválido.  <br/>- O item de contato é inválido.  <br/>- Houve uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Especifica que a propriedade URL externa não foi definida no banco de dados do Active Directory. Esse código de erro DEVE ser retornado se a propriedade URL externa não tiver sido definida no banco de dados do Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Especifica que a contagem máxima de membros do grupo foi atingida para obter informações de livre/ocupado para uma lista de distribuição. Esse erro DEVE ser retornado quando a contagem máxima de membros do grupo tiver sido atingida para obter informações de livre/ocupado para uma lista de distribuição.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Especifica que os elementos DataType e ShareFolderId estão presentes em uma solicitação. Esse código de erro DEVE ser retornado se os elementos DataType e ShareFolderId estão presentes em uma solicitação.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Especifica que o chamador tentou conceder permissões em seu calendário ou pasta de contatos a um usuário em outra organização e a tentativa falhou. Esse código de erro DEVE ser retornado quando a política de compartilhamento estiver desabilitada para o chamador ou quando a política de compartilhamento atribuída ao chamador não permitir o compartilhamento para o nível solicitado ou o tipo de pasta solicitado.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Especifica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos a um usuário externo, mas a política de compartilhamento atribuída ao solicitante especifica que o domínio do usuário externo não está listado na política.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Especifica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos a um usuário externo, mas a política de compartilhamento atribuída ao solicitante especifica que o nível de permissão solicitado é maior do que o que a política de compartilhamento permite.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Especifica que a organização do solicitante não é federada, portanto, o solicitante não pode criar mensagens de compartilhamento para enviar a um usuário externo ou não pode aceitar o compartilhamento de mensagens recebidas de um usuário externo. Esse código de erro DEVE ser retornado se a organização do solicitante não for federada.  <br/> |
|ErrorMailboxFailover  <br/> |Especifica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Especifica que o remetente do convite de compartilhamento não criou os metadados do convite de compartilhamento. Esse código de erro DEVE ser retornado se o remetente do convite de compartilhamento não tiver criado os metadados do convite de compartilhamento.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Especifica que o serviço de controle de mensagens não pode rastrear a mensagem.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Especifica que o serviço de controle de mensagens está para baixo ou ocupado. Este código de erro especifica um erro transitório. Os clientes podem tentar novamente se conectar ao servidor quando esse erro for recebido.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Especifica que o domínio determinado não pode ser encontrado.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Especifica que a organização do solicitante tem um conjunto de domínios federados, mas a organização do solicitante não tem endereços proxy SMTP com um dos domínios federados.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Especifica que um chamador solicitou informações de livre/ocupado para um usuário em outra organização, mas a relação organizacional não tem o tempo livre/ocupado habilitado.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Especifica que os objetos de federação da organização do solicitante não estão configurados corretamente.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Especifica que uma mensagem de compartilhamento não se destina ao chamador.  <br/> |
|ErrorInvalidSharingData  <br/> |Especifica que os metadados de compartilhamento não são válidos. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Esse erro DEVE ser retornado se uma ação não puder ser aplicada a um ou mais itens na conversa.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Esse erro DEVE ser retornado se qualquer regra não for validada.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Esse erro DEVE ser retornado quando ocorrer uma tentativa de gerenciar regras de Caixa de Entrada depois que outro cliente tiver acessado as regras de Caixa de Entrada.  <br/> |
|ErrorRulesOverQuota  <br/> |Esse erro DEVE ser retornado quando a cota de regra de um usuário tiver sido excedida.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Esse erro DEVE ser retornado à primeira conexão de assinatura se uma segunda conexão de assinatura for aberta.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Esse erro DEVE ser retornado quando as notificações de evento são perdidas.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Esse erro é retornado quando há nomes diferenciados herdados duplicados nos Serviços de Domínio do Active Directory (AD DS). Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Esse erro indica que uma solicitação para obter um token de acesso para cliente não era válida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Esse erro será retornado se o header [ManagementRole](managementrole.md) no header SOAP estiver incorreto. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Esse erro destina-se apenas ao uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Esse erro é retornado quando uma tentativa de pesquisa com escopo é executada sem usar um [elemento QueryString (String)](querystring-string.md) para uma pesquisa de indexação de conteúdo. Isso é aplicável às **operações SearchMailboxes** e **FindConversation.** Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Esse erro é retornado quando uma pesquisa de caixa de correio de arquivo morto não é bem-sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Esse erro é retornado quando a URL de uma caixa de correio de arquivo morto não é descoberta. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Esse erro ocorre quando a operação para obter a pasta de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Esse erro ocorre quando a operação para encontrar a pasta de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Esse erro ocorre quando a operação para obter o item de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Esse erro ocorre quando a operação para exportar itens de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Esse erro será retornado se um tamanho de foto inválido for solicitado do servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Esse erro é retornado quando um tamanho de foto inesperado é solicitado em uma solicitação de operação **GetUserPhoto.** Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Esse erro é retornado quando uma **solicitação de operação SearchMailboxes** contém muitas caixas de correio para pesquisar. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Esse erro indica que não foram encontradas marcas de retenção para esse usuário. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Esse erro é retornado quando as pesquisas de descoberta são desabilitadas em um locatário ou servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Esse erro ocorre ao tentar invocar a operação [FindItem](finditem-operation.md) com [um SeekToConditionPageItemView](seektoconditionpageitemview.md) para buscar itens de calendário, que não é suportado.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Esse erro destina-se apenas ao uso interno.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |O locatário está marcado para remoção.  <br/> |
|ErrorInvalidLicense  <br/> |O usuário não tem uma licença válida.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |A cota de recebimento de mensagens por pasta foi excedida.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento não é necessário e não está incluído em todas as respostas. 
  
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

