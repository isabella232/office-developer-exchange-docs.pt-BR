---
title: ResponseCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 4b84d670-74c9-4d6d-84e7-f0a9f76f0d93
description: O elemento ResponseCode fornece informações de status sobre a solicitação.
ms.openlocfilehash: 6481272c61aab3dc9aeb2fd988e3544169306f06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457463"
---
# <a name="responsecode"></a>ResponseCode

O elemento **ResponseCode** fornece informações de status sobre a solicitação. 
  
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
|[ResponseMessage](responsemessage.md) <br/> | Fornece informações descritivas sobre o status da resposta.<br/><br/>  A seguir estão as possíveis expressões XPath para este elemento:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [Operação DeleteItem](deleteitem-operation.md) .  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação SendItem](senditem-operation.md) .  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação DeleteFolder](deletefolder-operation.md) .  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação DeleteAttachment](deleteattachment-operation.md) .  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação de cancelamento de assinatura](unsubscribe-operation.md) .  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CreateFolder](createfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação GetFolder](getfolder-operation.md) .  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação UpdateFolder](updatefolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação MoveFolder](movefolder-operation.md) .  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CopyFolder](copyfolder-operation.md).  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação FindFolder](findfolder-operation.md) .  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação CreateItem](createitem-operation.md) única.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação GetItem](getitem-operation.md) .  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação UpdateItem](updateitem-operation.md) .  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação MoveItem](moveitem-operation.md) .  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CopyItem](copyitem-operation.md) .  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CreateAttachment](createattachment-operation.md) .  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação GetAttachment](getattachment-operation.md) .  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação FindItem](finditem-operation.md) .  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação ResolveNames](resolvenames-operation.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação ExpandDL](expanddl-operation.md) .  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação de assinatura](subscribe-operation.md) .  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação GetEvents](getevents-operation.md) .  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) .  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação SyncFolderItems](syncfolderitems-operation.md) .  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação convertid](convertid-operation.md) .  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação Getdelegate](getdelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contém o status e os resultados de uma resposta de [operação FindConversation](findconversation-operation.md) .  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação EmptyFolder](emptyfolder-operation.md) .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contém um status e o resultado de uma solicitação de [operação UpdateInboxRules](updateinboxrules-operation.md) .  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém um status e o resultado de uma solicitação de [operação UploadItems](uploaditems-operation.md) .  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contém uma resposta a uma solicitação [GetInboxRules](getinboxrules-operation.md) * * * *.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contém uma resposta a uma solicitação de [operação GetServiceConfiguration](getserviceconfiguration-operation.md) .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém definições de configuração de serviço.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto será necessário se esse elemento for usado. A tabela a seguir descreve os valores retornados com este elemento.
  
|Valor|Descrição|
|:-----|:-----|
|NoError  <br/> |Nenhum erro ocorreu para a solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Esse erro ocorre quando a conta de chamada não tem os direitos para executar a ação solicitada.  <br/> |
|ErrorAccessModeSpecified  <br/> |Este erro é somente para uso interno. Este erro não é retornado.  <br/> |
|ErrorAccountDisabled  <br/> |Esse erro ocorre quando a conta em questão tiver sido desabilitada.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Esse erro ocorre quando uma lista com delegados adicionados não pode ser salva.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Esse erro ocorre quando o registro de espaço de endereço ou o nome de domínio DNS (sistema de nomes de domínio), para disponibilidade entre florestas, não pôde ser encontrado no banco de dados do Active Directory.  <br/> |
|ErrorADOperation  <br/> |Esse erro ocorre quando a operação falhou devido a problemas de comunicação com o AD DS (serviços de domínio Active Directory).  <br/> |
|ErrorADSessionFilter  <br/> |Este erro é retornado quando uma solicitação de operação **ResolveNames** especifica um nome que não é válido.  <br/> |
|ErrorADUnavailable  <br/> |Este erro ocorre quando o AD DS não está disponível. Tente a solicitação novamente mais tarde.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Esse erro indica que o atributo **AffectedTaskOccurrences** não foi especificado. Quando o elemento [DeleteItem](deleteitem.md) é usado para excluir pelo menos um item que é uma tarefa e independentemente de a tarefa ser recorrente ou não, o atributo **AffectedTaskOccurrences** deve ser especificado para que o **DeleteItem** possa determinar se a ocorrência atual ou a série inteira deve ser excluída.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indica um erro na criação de caminho de pasta de arquivo morto.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indica que a caixa de correio de arquivo morto não foi habilitada.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indica que a descoberta de serviço de caixa de correio de arquivo morto falhou.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Especifica que foi feita uma tentativa de criar um item com mais de 10 anexos aninhados. Esse valor foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |O elemento [CreateAttachment](createattachment.md) retornará esse erro se for feita uma tentativa de criar um anexo com tamanho excedendo Int32. MaxValue, em bytes.  <br/> O elemento [GetAttachment](getattachment.md) retornará esse erro se uma tentativa de recuperar um anexo existente com tamanho exceder Int32. MaxValue, em bytes.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentaram determinar o local de um computador entre florestas que está executando o Exchange 2010 que tem a função de servidor de acesso para Cliente instalada usando o serviço de descoberta automática, mas a chamada para o serviço de descoberta automática falhou.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Esse erro indica que as informações de configuração de disponibilidade da floresta local estão ausentes no AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Esse erro indica que uma exceção ocorreu durante o processamento de um item e que a exceção provavelmente ocorrerá para os itens a seguir. As solicitações podem incluir vários itens; por exemplo, uma solicitação de operação do GetItem pode incluir vários identificadores. Em geral, os itens são processados um de cada vez. Se ocorrer uma exceção durante o processamento de um item e essa exceção for provavelmente ocorrer para os itens a seguir, os itens que seguir não serão processados.  <br/><br/>  Estes são exemplos de erros que interromperão o processamento de itens que seguem:<br/>  <br/>- ErrorAccessDenied  <br/>- ErrorAccountDisabled  <br/>- ErrorADUnavailable  <br/>- ErrorADOperation  <br/>- ErrorConnectionFailed  <br/>- ErrorMailboxStoreUnavailable  <br/>- ErrorMailboxMoveInProgress  <br/>- ErrorPasswordChangeRequired  <br/>- ErrorPasswordExpired  <br/>- ErrorQuotaExceeded  <br/>- ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Esse erro ocorre quando é feita uma tentativa de mover ou copiar uma ocorrência de um item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Esse erro ocorre quando uma tentativa é feita para atualizar um item de calendário que está localizado na pasta itens excluídos e quando as atualizações de reunião ou cancelamentos são enviados de acordo com o valor do atributo **SendMeetingInvitationsOrCancellations** . <br/><br/>Estes são os valores possíveis para este atributo:  <br/><br/>- SendToAllAndSaveCopy  <br/>- SendToChangedAndSaveCopy  <br/>- SendOnlyToAll  <br/>- SendOnlyToChanged  <br/>  <br/>No entanto, essa atualização só é permitida quando o valor desse atributo é definido como SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Esse erro ocorre quando a operação UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem é chamada e a ID especificada não é uma ID de ocorrência de qualquer item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Esse erro ocorre quando a operação **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem**ou **SendItem** é chamada e a ID especificada não é uma ID de qualquer item mestre recorrente.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando uma duração de item de calendário é maior do que o máximo permitido, que tem, atualmente, 5 anos.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Esse erro ocorre quando uma hora de término do calendário é definida com o mesmo horário ou após a hora de início.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Esse erro ocorre quando a pasta especificada para uma operação **FindItem** com um elemento [CalendarView](calendarview.md) não é do tipo de pasta do calendário.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando valores inválidos de Day, WeekendDay e Weekday são usados para definir o padrão de alteração de horário.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando valores inválidos de Day, Weekday e WeekendDay são usados para especificar a recorrência semanal.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Esse erro ocorre quando o estado de um BLOB (objeto grande binário) de recorrência de um item de calendário no repositório do Exchange é inválido.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Esse erro ocorre quando a recorrência especificada não pode ser criada.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Esse erro ocorre quando um fuso horário inválido é encontrado.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Esse erro indica que um item de calendário foi cancelado.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Esse erro indica que o elemento [AcceptItem](acceptitem.md) é inválido para um item de calendário ou uma solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Esse erro indica que o elemento [DeclineItem](declineitem.md) é inválido para um item de calendário ou uma solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Esse erro indica que o elemento [RemoveItem](removeitem.md) é inválido para o cancelamento de uma reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Esse erro indica que o elemento [TentativelyAcceptItem](tentativelyacceptitem.md) é inválido para um item de calendário ou uma solicitação de reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Esse erro indica que a operação (atualmente CancelItem) no item de calendário não é válida para um participante. Somente o organizador da reunião pode cancelar a reunião.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Esse erro indica que [AcceptItem](acceptitem.md) é inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Esse erro indica que [DeclineItem](declineitem.md) é inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Esse erro indica que [RemoveItem](removeitem.md) é inválido para o item de calendário do organizador. Para remover uma reunião do calendário, o organizador deve usar o CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Esse erro indica que [TentativelyAcceptItem](tentativelyacceptitem.md) é inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Esse erro indica que uma solicitação de reunião está desatualizada e não pode ser atualizada.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Esse erro indica que o índice de ocorrências não aponta para uma ocorrência dentro da recorrência atual. Por exemplo, se o seu padrão de recorrência define um conjunto de três ocorrências de reunião e você tenta acessar a quinta ocorrência, esse código de resposta resultará.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Esse erro indica que qualquer operação em uma ocorrência excluída (endereçado via ID mestre recorrente e índice de ocorrência) é inválida.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Este erro é relatado em operações CreateItem e UpdateItem para itens de calendário ou propriedades de recorrência de tarefa quando o valor da propriedade está fora do intervalo. Por exemplo, especificar a semana décimo quinto do mês resultará nesse código de resposta.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Este erro ocorre quando o intervalo de início ao fim do elemento [CalendarView](calendarview.md) é maior que o máximo permitido, atualmente em dois anos.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Esse erro indica que a conta solicitante não é uma conta válida no banco de dados de diretório.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indica que foi feita uma tentativa de arquivar uma pasta de tarefas de contato do calendário.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indica que foi feita uma tentativa de arquivar itens em pastas públicas.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indica que foi feita uma tentativa de arquivar itens na caixa de correio de arquivo morto.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Esse erro ocorre quando um item de calendário está sendo criado e o atributo **SavedItemFolderId** se refere a uma pasta que não é do calendário.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Esse erro ocorre quando um contato está sendo criado e o atributo **SavedItemFolderId** se refere a uma pasta que não é de contato.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Esse erro indica que um item de postagem não pode ser criado em uma pasta diferente de uma pasta de email, como calendário, contato, tarefas, anotações e assim por diante.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Esse erro ocorre quando uma tarefa está sendo criada e o atributo **SavedItemFolderId** se refere a uma pasta que não é de tarefa.  <br/> |
|ErrorCannotDeleteObject  <br/> |Esse erro ocorre quando o item ou a pasta a ser excluída não pode ser excluído.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |A [Operação DeleteItem](deleteitem-operation.md) retorna esse erro quando ele não exclui a ocorrência atual de uma tarefa recorrente. Isso só poderá acontecer se o atributo **AffectedTaskOccurrences** tiver sido definido como SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indica que foi feita uma tentativa de desabilitar uma extensão mandatorty.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Este erro deve ser retornado quando o servidor não pode esvaziar uma pasta.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indica que o caminho da pasta de origem não pôde ser recuperado.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Especifica que o servidor não pôde recuperar a URL externa para opções do Outlook Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |A operação **GetAttachment** retornará esse erro se não for possível recuperar o corpo de um anexo de arquivo.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões de calendário em uma pasta que não é de calendário.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões de não calendário em uma pasta de calendário.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Esse erro indica que você não pode definir permissões desconhecidas em um conjunto de permissões.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indica que foi feita uma tentativa de especificar a pasta de pesquisa como a pasta de origem.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Esse erro ocorre quando uma solicitação que requer um identificador de item recebe um identificador de pasta.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Esse erro ocorre quando uma solicitação que requer um identificador de pasta recebe um identificador de item.  <br/> |
|ErrorChangeKeyRequired  <br/> |Este código de resposta foi substituído pelo **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Este erro é retornado quando a tecla Change de um item está ausente ou é obsoleta. <br/><br/>Para as operações SendItem, UpdateItem e UpdateFolder, o chamador deve passar uma chave de alteração correta e atual para o item. Observe que esse é o caso com UpdateItem mesmo quando a resolução de conflitos está definida para substituir sempre.  <br/> |
|ErrorClientDisconnected  <br/> |Especifica que o cliente foi desconectado.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorClientIntentNotFound  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorConnectionFailed  <br/> |Este erro ocorre quando os serviços Web do Exchange não podem se conectar à caixa de correio.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Esse erro indica que a propriedade que foi inspecionada para um filtro contém não é um tipo de cadeia de caracteres.  <br/> |
|ErrorContentConversionFailed  <br/> |A operação **GetItem** retorna esse erro quando os serviços Web do Exchange não conseguem recuperar o conteúdo MIME para o item solicitado. <br/><br/>A operação **CreateItem** retorna esse erro quando os serviços Web do Exchange não conseguem criar o item do conteúdo MIME fornecido. Normalmente, essa é uma indicação de que a propriedade item está corrompida ou truncada.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Esse erro ocorre quando uma solicitação de pesquisa é feita usando a opção QueryString e a indexação de conteúdo não está habilitada para a caixa de correio de destino.  <br/> |
|ErrorCorruptData  <br/> |Este erro ocorre quando os dados estão corrompidos e não podem ser processados.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Esse erro ocorre quando o chamador não tem permissão para criar o item.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Esse erro ocorre quando uma ou mais pastas gerenciadas que foram especificadas na solicitação de operação CreateManagedFolder não foram criadas. Procure cada pasta para determinar quais pastas foram criadas e quais pastas não existem.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Esse erro ocorre quando a conta de chamada não tem as permissões necessárias para criar a subpasta.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Esse erro ocorre quando é feita uma tentativa de mover um item ou uma pasta de uma caixa de correio para outra. Se a caixa de correio de origem e a caixa de correio de destino forem diferentes, você receberá esse erro.  <br/> |
|ErrorCrossSiteRequest  <br/> |Esse erro indica que a solicitação não é permitida porque o servidor de acesso para cliente que deve atender à solicitação está em um site diferente.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Este erro pode ocorrer nos seguintes cenários:<br/>  <br/>– É feita uma tentativa de acessar ou gravar uma propriedade em um item e o valor da propriedade é muito grande.<br/>– O comprimento de conteúdo MIME codificado em base64 dentro do XML de solicitação excede o limite.<br/>-O tamanho do corpo de um corpo de item existente excede o limite.<br/>– O consumidor tenta definir um texto HTML ou de texto cujo comprimento (ou o comprimento combinado no caso de append) exceda o limite. |
|ErrorDataSourceOperation  <br/> |Esse erro ocorre quando o provedor de dados subjacente falha ao concluir a operação.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Esse erro ocorre em uma operação **AddDelegate** quando o usuário especificado já existe na lista de representantes.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Esse erro ocorre em uma operação **AddDelegate** quando o usuário especificado a ser adicionado é o proprietário da caixa de correio.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Esse erro ocorre em uma operação **Getdelegate** quando não há informações de representante sobre a mensagem do FreeBusy local ou nenhum representante público do Active Directory (sem "representante público" ou nenhuma entrada "enviar em nome" no AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Esse erro ocorre quando um usuário especificado não pode ser mapeado para um usuário no AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Esse erro ocorre na operação **AddDelegate** quando um usuário delegado adicionado não é válido.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Esse erro ocorre quando é feita uma tentativa de excluir uma pasta distinta.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Esse erro indica que uma ID de usuário distinto não é válida para a operação. **DistinguishedUserType** não deve estar presente na solicitação.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Esse erro indica que um membro da lista de distribuição de solicitações não existe na lista de distribuição.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Esse erro ocorre quando nomes de pastas duplicados são especificados no elemento [FolderNames](foldernames.md) da solicitação de operação **CreateManagedFolder** .  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Esse erro indica que há cabeçalhos SOAP duplicados.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Esse erro indica que uma ID de usuário duplicada foi encontrada em um conjunto de permissões, padrão ou anônimo são definidos mais de uma vez, ou há SIDs ou destinatários duplicados.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Esse erro ocorre quando uma solicitação tenta criar/atualizar os parâmetros de pesquisa de uma pasta de pesquisa. Por exemplo, isso pode ocorrer quando uma pasta de pesquisa é criada na caixa de correio, mas a pasta de pesquisa é direcionada para procurar em outra caixa de correio.  <br/> |
|ErrorEventNotFound  <br/> |Esse erro ocorre quando o evento associado a uma marca d' água é excluído antes do evento ser retornado. Quando esse erro é retornado, a assinatura também é excluída.  <br/> |
|ErrorExceededConnectionCount  <br/> |Este erro-iIndicates que há mais solicitações simultâneas no servidor do que o permitido pela política de um usuário.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Esse erro indica que a contagem máxima de assinaturas da política de limitação do usuário foi excedida.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Esse erro indica que uma chamada de operação de pesquisa excedeu o número total de itens que podem ser retornados.  <br/> |
|ErrorExpiredSubscription  <br/> |Esse erro ocorrerá se a [operação GetEvents](getevents-operation.md) for chamada como uma assinatura estiver sendo excluída, pois expirou.  <br/> |
|ErrorExtensionNotFound  <br/> |Indica que a extensão não foi encontrada.  <br/> |
|ErrorFolderCorrupt  <br/> |Este erro ocorre quando a pasta está corrompida e não pode ser salva.  <br/> |
|ErrorFolderExists  <br/> |Esse erro ocorre quando é feita uma tentativa de criar uma pasta com o mesmo nome de outra pasta no mesmo pai. Nomes de pastas duplicados não são permitidos.  <br/> |
|ErrorFolderNotFound  <br/> |Esse erro indica que a ID de pasta especificada não corresponde a uma pasta válida ou que o representante não tem permissão para acessar a pasta.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Esse erro indica que a propriedade solicitada não pôde ser recuperada. Isso não indica que a propriedade não existe, mas que a propriedade foi corrompida de alguma forma para que a recuperação falhasse.  <br/> |
|ErrorFolderSave  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSaveFailed  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a valores de propriedade inválidos. O código de resposta lista quais propriedades causaram o problema.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Esse erro indica que a contagem de membros do grupo máximo foi atingida para a obtenção de informações de disponibilidade de uma lista de distribuição.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Este erro é retornado quando as informações de disponibilidade não podem ser recuperadas devido a uma falha intermediária.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorImContactLimitReached  <br/> |Este erro é retornado quando novos contatos de mensagens instantâneas (IM) não podem ser adicionados porque o número máximo de contatos foi atingido. Este erro foi introduzido no Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Esse erro é retornado quando é feita uma tentativa de adicionar um nome de exibição de grupo quando um grupo existente já tem o mesmo nome de exibição. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Este erro é retornado quando novos grupos de IM não podem ser adicionados porque o número máximo de grupos foi atingido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |O erro é retornado no caso de autorização de servidor para servidor para representação do Exchange quando o chamador não tem os direitos adequados para representar o usuário específico em questão. Este erro mapeia para o direito do Active Directory estendido ms-Exch-EPI-Mai-Impersonate.  <br/> |
|ErrorImpersonationDenied  <br/> |Esse erro é retornado na autorização de servidor para servidor para a representação do Exchange quando o chamador não tem os direitos adequados para representar o servidor de acesso para cliente para o qual ele está fazendo a solicitação. Isso mapeia para o direito do Active Directory estendido ms-Exch-EPI-Impersonation.  <br/> |
|ErrorImpersonationFailed  <br/> |Esse erro indica que houve um erro inesperado quando foi feita uma tentativa de executar a autenticação de servidor para servidor. Esse código de resposta normalmente indica que a conta de serviço que está executando o pool de aplicativos dos serviços Web do Exchange está configurada incorretamente, que os serviços Web do Exchange não podem falar com o diretório ou que uma confiança entre florestas não está configurada corretamente.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Esse erro indica que a solicitação era válida para a versão atual do Exchange Server, mas era inválida para a versão do servidor de solicitação que foi especificada.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Esse erro indica que cada descrição de alteração nos elementos [UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) deve listar apenas uma propriedade para atualizar.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Esse erro ocorre quando a solicitação contém muitos participantes para resolver. Por padrão, o número máximo de participantes a serem resolvidos é 100.  <br/> |
|ErrorInsufficientResources  <br/> |Esse erro ocorre quando o servidor de caixa de correio está sobrecarregado. Tente a solicitação novamente mais tarde.  <br/> |
|ErrorInternalServerError  <br/> |Esse erro indica que os serviços Web do Exchange encontraram um erro que não pôde se recuperar de, e um código de resposta mais específico associado ao erro que ocorreu não existe.  <br/> |
|ErrorInternalServerTransientError  <br/> |Esse erro indica que ocorreu um erro interno no servidor e que você deve tentar a solicitação novamente mais tarde.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Esse erro indica que o nível de acesso que o chamador tem nos dados de disponibilidade é inválido.  <br/> |
|ErrorInvalidArgument  <br/> |Esse erro indica um erro causado por todos os argumentos inválidos passados para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Este erro é retornado nos seguintes cenários: <br/><br/>– O usuário especificado no parâmetro _Send-as_ não existe no diretório. <br/>– O usuário especificado no parâmetro _enviando-como_ não é exclusivo no diretório. <br/>-O endereço de _envio como_ está vazio.<br/>– O endereço de _envio como_ não é um endereço de email válido.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Esse erro é retornado pela [operação GetAttachment](getattachment-operation.md) ou pela [operação DeleteAttachment](deleteattachment-operation.md) quando um anexo que corresponde à ID especificada não é encontrado.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Esse erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexo complexa. Os serviços Web do Exchange só dão suporte a filtros simples na tabela de anexos. Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexo mais complexa (um subfiltro), os serviços Web do Exchange não poderão renderizar o XML desse filtro e retornará esse código de resposta. <br/><br/>Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitar o elemento [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Esse erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexo complexa. Os serviços Web do Exchange só dão suporte a filtros simples na tabela de anexos. <br/><br/>Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexo mais complexa, os serviços Web do Exchange não poderão renderizar o XML para esse filtro. Nesse caso, o subfiltro de anexo contém um filtro de texto, mas não está examinando o nome de exibição do anexo.<br/><br/> Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitar o elemento [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Esse erro indica que o procedimento de autorização para o solicitante falhou.  <br/> |
|ErrorInvalidChangeKey  <br/> |Esse erro ocorre quando um consumidor passa um identificador de pasta ou item com uma chave de alteração que não pode ser analisada. Por exemplo, isso pode ser um conteúdo Base64 inválido ou uma cadeia de caracteres vazia.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Esse erro indica que houve um erro interno quando foi feita uma tentativa de resolver a identidade do chamador.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Esse erro é retornado quando é feita uma tentativa de definir o valor de elemento [Completed](completedate.md) de uma tarefa para uma hora no futuro. Quando é convertido no horário local do servidor de acesso para cliente, a [conclusão](completedate.md) de uma tarefa não pode ser definida como um valor posterior à hora local no servidor de acesso para cliente.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Esse erro indica que um endereço de email inválido foi fornecido para um contato.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Esse erro indica que um valor de índice de email inválido foi fornecido para uma entrada de email.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Esse erro ocorre quando as credenciais que são usadas para fazer proxy de uma solicitação para uma floresta de serviço de diretório diferente falham.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Esse erro indica que as permissões da pasta especificada são inválidas.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Esse erro indica que a ID de usuário do representante especificado é inválida.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Esse erro ocorre durante a representação do Exchange quando um chamador não especifica um UPN, um endereço de email ou um SID de usuário. Isso também ocorrerá se o chamador especificar um ou mais desses e os valores estiverem vazios.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Esse erro ocorre quando o bitmask passado para uma restrição de elemento [excludetes](excludes.md) não pode ser analisado.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Este erro ocorre quando ocorrem os seguintes eventos: <br/> <br/>– O chamador tenta usar uma propriedade estendida que não é suportada pelos serviços Web do Exchange.  <br/>– O chamador passa uma combinação inválida de valores de atributo para uma propriedade estendida. Isso também ocorre se nenhum atributo for passado. Apenas algumas combinações são permitidas.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Esse erro ocorre quando a seção Value de uma propriedade estendida não corresponde ao tipo da propriedade. <br/><br/>Por exemplo, a definição de uma propriedade estendida que tenha Recordtypepropriedade = "cadeia de caracteres" como uma matriz de números inteiros resultará em erro. Qualquer representação de cadeia de caracteres que não seja coercible no tipo especificado para a propriedade estendida gerará esse erro.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Esse erro indica que o remetente do convite de compartilhamento não criou os metadados de convite de compartilhamento.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Esse erro indica que uma mensagem de compartilhamento não se destina ao chamador.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Esse erro indica que os objetos de Federação da organização do solicitante não estão configurados corretamente.  <br/> |
|ErrorInvalidFolderId  <br/> |Esse erro ocorre quando a ID da pasta está corrompida.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Esse erro indica que o tipo de pasta especificado é inválido para a operação atual. Por exemplo, não é possível criar uma pasta de pesquisa em uma pasta pública.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Esse erro ocorrerá na paginação fracionária quando o usuário tiver especificado uma das seguintes opções: <br/> <br/>-Um numerador maior que o denominador  <br/>-Um numerador menor que zero  <br/>-Um denominador que é menor ou igual a zero  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Esse erro indica que os elementos [DataType](datatype.md) e ShareFolderId estão presentes em uma solicitação.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Esse erro ocorre quando a [operação GetUserAvailability](getuseravailability-operation.md) é chamada com um [FreeBusyViewType](freebusyviewtype.md) de nenhum.  <br/> |
|ErrorInvalidId  <br/> |Esse erro indica que a ID e/ou a tecla Change está malformada.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Esse erro ocorre quando o chamador especifica um atributo **ID** que está vazio.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Esse erro ocorre quando o item não pode ser curtido. As versões do Exchange que começam com o número de compilação 15.00.0913.09 incluem esse valor.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Esse erro ocorre quando o chamador especifica um atributo **ID** malformado.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Esse erro indica que uma ID de pasta ou de item que está usando o formato Exchange 2007 foi especificada para uma solicitação com uma versão do Exchange 2007 SP1 ou posterior. Você não pode usar IDs do Exchange 2007 no Exchange 2007 SP1 ou em solicitações posteriores. Você precisa usar a [operação convertid](convertid-operation.md) para convertê-los primeiro.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Esse erro ocorre quando o chamador especifica um atributo **ID** muito longo.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Esse erro é retornado sempre que uma ID que não é uma ID de anexo de item é passada para um método de serviço Web que espera uma ID de anexo.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Esse erro ocorre quando um contato na sua caixa de correio está corrompido.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Esse erro ocorre quando o chamador especifica um atributo **ID** muito longo.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Este erro é retornado quando a hierarquia de anexos em um item excede o máximo de 255 níveis de profundidade.  <br/> |
|ErrorInvalidIdXml  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidImContactId  <br/> |Este erro é retornado quando o identificador de contato de IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Esse erro é retornado quando o identificador de endereço SMTP do grupo de distribuição de IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Este erro é retornado quando o identificador do grupo de IM especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Esse erro ocorrerá se o deslocamento da paginação indexada for negativo.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indica que o item era inválido para uma operação **ArchiveItem** .  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Esse erro ocorre quando é feita uma tentativa de usar um objeto de resposta AcceptItem Para um tipo de item diferente de uma solicitação de reunião ou de um item de calendário, ou quando é feita uma tentativa de aceitar uma ocorrência de item de calendário que está na pasta itens excluídos.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Esse erro ocorre quando é feita uma tentativa de usar um objeto de resposta CancelItem em um tipo de item diferente de um item de calendário.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Esse erro é retornado quando é feita uma tentativa de criar um anexo de item de um tipo sem suporte.  <br/><br/>  Os tipos de item suportados para anexos de item incluem os seguintes objetos:  <br/><br/>- [Discrimina](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Amostra](contact.md) <br/> <br/> Por exemplo, se você tentar criar um anexo [MeetingMessage](meetingmessage.md) , encontrará esse código de resposta.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Esse erro será retornado de uma [operação CreateItem](createitem-operation.md) se a solicitação contiver um tipo de item sem suporte. <br/><br/>Os itens com suporte incluem os seguintes objetos:<br/>  <br/>- [Discrimina](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Amostra](contact.md) <br/><br/>  Determinados tipos são criados como um efeito colateral de fazer algo mais. As mensagens de reunião, por exemplo, são criadas quando você envia um item de calendário para participantes; Eles não são criados explicitamente.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Esse erro ocorre quando é feita uma tentativa de usar um objeto de resposta DeclineItem para um tipo de item diferente de uma solicitação de reunião ou de um item de calendário, ou quando é feita uma tentativa de recusar uma ocorrência de item de calendário que está na pasta itens excluídos.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Esse erro indica que a [operação ExpandDL](expanddl-operation.md) é válida apenas para listas de distribuição particulares.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Esse erro será retornado de um objeto de resposta RemoveItem se a solicitação especificar um item que não seja um item de cancelamento de reunião.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Esse erro será retornado de uma [operação SendItem](senditem-operation.md) se a solicitação especificar um item que não seja um item de mensagem.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Esse erro ocorre quando é feita uma tentativa de usar o [TentativelyAcceptItem](tentativelyacceptitem.md) para um tipo de item diferente de uma solicitação de reunião ou de um item de calendário, ou quando é feita uma tentativa de aceitar provisoriamente uma ocorrência de item de calendário que está na pasta itens excluídos.  <br/> |
|ErrorInvalidLogonType  <br/> |Este erro é somente para uso interno. Este erro não é retornado.  <br/> |
|ErrorInvalidMailbox  <br/> |Esse erro indica que a [operação CreateItem](createitem-operation.md) ou a [operação UpdateItem](updateitem-operation.md) falhou ao criar ou atualizar uma lista de distribuição pessoal.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Esse erro ocorre quando a estrutura da pasta gerenciada está corrompida e não pode ser renderizada.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Esse erro ocorre quando a cota definida na pasta gerenciada é menor que zero, que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Esse erro ocorre quando o tamanho definido na pasta gerenciada é menor que zero, que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Este erro ocorre quando o valor interno de disponibilidade mesclado fornecido é inválido. O valor mínimo padrão é 5 minutos. O valor máximo padrão é de 1440 minutos.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Esse erro ocorre quando o nome é inválido para a [operação ResolveNames](resolvenames-operation.md). Por exemplo, uma cadeia de caracteres com comprimento zero, um único espaço, uma vírgula e um traço são todos os nomes inválidos.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Esse erro indica um erro na conta de serviço de rede no servidor de acesso para cliente.  <br/> |
|ErrorInvalidOofParameter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidOperation  <br/> | Este é um erro geral que é usado quando a operação solicitada é inválida. <br/><br/>Por exemplo, não é possível fazer o seguinte: <br/> <br/>– Realize uma passagem "profunda" usando a [operação FindFolder](findfolder-operation.md) em uma pasta pública.  <br/>-Mova ou copie a raiz da pasta pública.  <br/>-Excluir um item associado usando qualquer modo, exceto a exclusão "difícil".  <br/>-Move ou copia um item associado.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Esse erro indica que um chamador solicitou informações de disponibilidade para um usuário em outra organização, mas a relação organizacional não tem disponibilidade habilitada.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Esse erro ocorre quando um consumidor passa um valor de zero ou negativo para que as linhas máximas sejam retornadas.  <br/> |
|ErrorInvalidParentFolder  <br/> |Esse erro ocorre quando um consumidor passa uma pasta pai inválida para uma operação. Por exemplo, esse erro será retornado se você tentar criar uma pasta dentro de uma pasta de pesquisa.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Esse erro é retornado quando é feita uma tentativa de definir uma porcentagem de conclusão da tarefa como um valor inválido. O valor deve estar entre 0 e 100 (inclusive).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Esse erro indica que o nível de permissão é inconsistente com as configurações de permissão.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Esse erro indica que o identificador do chamador não é válido.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Esse erro indica que o número de telefone não está correto ou não atende às regras do plano de discagem.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Esse erro ocorre quando a propriedade à qual você está tentando acrescentar não dá suporte à anexação. <br/><br/>A seguir estão as únicas propriedades que oferecem suporte à anexação: <br/> <br/>– Coleções de destinatários (ToRecipients, CcRecipients, BccRecipients)  <br/>Conjuntos de participantes (RequiredAttendees, OptionalAttendees, recursos)  <br/>-Body  <br/>-ReplyTo  <br/><br/>  Além disso, esse erro ocorre quando um corpo de mensagem é acrescentado se o formato especificado na solicitação não corresponder ao formato do item no repositório.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Esse erro ocorrerá se a operação de exclusão for especificada em uma chamada de operação [UpdateItem](updateitem-operation.md) ou [UpdateFolder](updatefolder-operation.md) para uma propriedade que não ofereça suporte à operação de exclusão. Por exemplo, não é possível excluir o elemento [ItemId](itemid.md) do objeto [Item](item.md) .  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Esse erro ocorrerá se o consumidor passar em uma das propriedades de sinalizador em um filtro [Exists](exists.md) . Por exemplo, esse erro ocorrerá se os sinalizadores [IsRead](isread.md) ou [IsFromMe](isfromme.md) forem especificados no elemento [Exists](exists.md) . A solicitação deve usar o elemento [IsEqualTo](isequalto.md) em vez desses sinalizadores, e portanto parte de uma única propriedade.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Esse erro ocorre quando a propriedade que você está tentando manipular não é compatível com a operação que está sendo executada nele.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Esse erro ocorrerá se uma propriedade especificada na solicitação não estiver disponível para o tipo de item. Por exemplo, esse erro é retornado se uma propriedade que está disponível somente em itens de calendário é solicitada em uma chamada de [operação GetItem](getitem-operation.md) para uma mensagem ou é atualizada em uma chamada de [operação UpdateItem](updateitem-operation.md) para uma mensagem. <br/> <br/>  Isso ocorre nas seguintes operações: <br/> <br/>- [Operação GetItem](getitem-operation.md) <br/>- [Operação GetFolder](getfolder-operation.md) <br/>- [Operação UpdateItem](updateitem-operation.md) <br/>- [Operação UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Esse erro indica que a propriedade que você está tentando manipular não dá suporte à operação que está sendo executada nele. Por exemplo, esse erro é retornado se a propriedade que você está tentando definir é somente leitura.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Esse erro ocorre durante uma [operação UpdateItem](updateitem-operation.md) quando um cliente tenta atualizar determinadas propriedades de uma mensagem que já foi enviada.<br/><br/> Por exemplo, as seguintes propriedades não podem ser atualizadas em uma mensagem enviada: <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Esse erro ocorrerá se você chamar a [operação GetEvents](getevents-operation.md) ou a [operação de cancelamento](unsubscribe-operation.md) de assinatura usando uma ID de assinatura push. Para cancelar a assinatura de uma assinatura push, você deve responder a uma solicitação de envio com uma resposta de cancelamento de assinatura ou desconectar o serviço Web e aguardar o tempo limite das notificações por push.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Esse erro é retornado pela [operação Subscribe](subscribe-operation.md) quando ele cria uma assinatura "Push" e indica que a URL incluída na solicitação é inválida.<br/><br/>As seguintes condições devem ser atendidas para que os serviços Web do Exchange aceitem a URL: <br/> <br/>-O comprimento \> 0 e-o protocolo da cadeia de caracteres \< 2083.  <br/> é http ou HTTPS.  <br/>– A URL pode ser analisada pela classe URI do Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Esse erro indica que a coleção de destinatários em sua mensagem ou a coleção de participantes no item de calendário é inválida. Por exemplo, este erro será retornado quando for feita uma tentativa de enviar um item sem destinatários.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que os serviços Web do Exchange não podem representar. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que os serviços Web do Exchange não podem representar. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que os serviços Web do Exchange não podem representar. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que os serviços Web do Exchange não podem representar. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Este erro é retornado da [operação CreateItem](createitem-operation.md) para objetos de resposta de encaminhamento e resposta nos seguintes cenários:<br/>  <br/>– O identificador do item referenciado não é uma [mensagem](message-ex15websvcsotherref.md), um [CalendarItem](calendaritem.md)ou um descendente de uma **mensagem** ou **CalendarItem**.  <br/>– O identificador do item de referência é para um **CalendarItem** e o organizador está tentando responder ou responder para si mesmo.  <br/>– A mensagem é um rascunho e responder ou ReplyAll está selecionado.  <br/>– O item de referência, para [SuppressReadReceipt](suppressreadreceipt.md), não é uma **mensagem** ou um descendente de uma **mensagem**.  <br/> |
|ErrorInvalidRequest  <br/> |Esse erro ocorre quando a solicitação SOAP tem um cabeçalho de ação SOAP, mas nada no corpo SOAP. Observe que o cabeçalho de ação SOAP não é necessário, pois os serviços Web do Exchange podem determinar o método a ser chamado a partir do nome local do elemento raiz no corpo SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Esse erro é retornado quando a marca de retenção especificada tem uma ação incorreta associada a ela. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Esse erro é retornado quando é feita uma tentativa de definir uma marca inexistente ou invisível em uma propriedade **PolicyTag** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Esse erro é retornado quando é feita uma tentativa de definir uma marca implícita na propriedade **PolicyTag** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indica que o GUID da marca de retenção era inválido.  <br/> |
|ErrorInvalidRoutingType  <br/> |Este erro ocorre quando o tipo de roteamento que é passado para um elemento [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) é inválido. Normalmente, o tipo de roteamento é definido como Simple Mail Transfer Protocol (SMTP).  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Esse erro ocorrerá se a hora de término da duração especificada não for maior do que a hora de início ou se a hora de término não ocorrer no futuro.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Esse erro indica que uma solicitação de proxy que foi enviada para outro servidor não pode atender à solicitação devido a uma incompatibilidade de controle de versão.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Esse erro indica que o descritor de segurança do Exchange na pasta calendário no repositório está corrompido.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Esse erro ocorre durante uma tentativa de enviar um item onde o [SavedItemFolderId](saveditemfolderid.md) é especificado na solicitação, mas a propriedade **SaveItemToFolder** é definida como **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Esse erro indica que o token passado no cabeçalho está malformado, não se refere a uma conta válida no diretório ou está faltando o grupo primário **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Esse erro indica que os metadados de compartilhamento não são válidos. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorInvalidSid  <br/> |Esse erro ocorre quando um SID inválido é passado em uma solicitação.  <br/> |
|ErrorInvalidSIPUri  <br/> |Esse erro indica que o nome SIP, o plano de discagem ou o número de telefone são URIs SIP inválidos.  <br/> |
|ErrorInvalidServerVersion  <br/> |Esse erro indica que uma versão de servidor de solicitação inválida foi especificada na solicitação.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Esse erro ocorre quando o endereço SMTP não pode ser analisado.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubscription  <br/> |Esse erro indica que a assinatura não é mais válida. Isso pode ter ocorrido porque o servidor de acesso para cliente está sendo reiniciado ou porque a assinatura expirou.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Esse erro indica que a solicitação de assinatura incluiu várias IDs de pasta pública. Uma assinatura pode incluir várias pastas da mesma caixa de correio ou uma ID de pasta pública.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Esse erro é retornado por [SyncFolderItems](syncfolderitems.md) ou [SyncFolderHierarchy](syncfolderhierarchy.md) se os dados [SyncState](syncstate-ex15websvcsotherref.md) que são passados são inválidos. Para corrigir esse erro, você deve sincronizar novamente sem o estado de sincronização. Certifique-se de que, se você estiver mantendo BLOBs de estado de sincronização, não estará truncando acidentalmente o BLOB.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Esse erro indica que o intervalo de tempo especificado é inválido. A hora de início deve ser maior ou igual à hora de término.  <br/> |
|ErrorInvalidUserInfo  <br/> |Esse erro indica que um [userid](userid.md) internamente inconsistente foi especificado para uma operação de permissões. Por exemplo, se uma ID de usuário diferenciada for especificada (padrão ou anônima), esse erro será retornado se você também tentar especificar um SID ou o endereço SMTP principal ou o nome de exibição para esse usuário.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Esse erro indica que as configurações de ausência temporária (OOF) do usuário são inválidas devido a uma resposta interna ou externa ausente.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Esse erro ocorre durante a representação do Exchange. O chamador transmitiu um UPN inválido no cabeçalho SOAP que não estava acessível no diretório.  <br/> |
|ErrorInvalidUserSid  <br/> |Esse erro ocorre quando um SID inválido é passado em uma solicitação.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Esse erro indica que o valor de comparação na restrição é inválido para a propriedade que você está comparando.<br/><br/> Por exemplo, o valor de comparação de [DateTimeCreated](datetimecreated.md)  >  **true** retornaria esse código de resposta. <br/><br/>Esse código de resposta também é retornado se você especificar uma propriedade de enumeração na comparação, mas o valor que você está comparando em comparação não é um valor válido para essa enumeração.  <br/> |
|ErrorInvalidWatermark  <br/> |Este erro é causado por uma marca d' água inválida.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Esse erro indica que um gateway VoIP válido não está disponível.  <br/> |
|ErrorIrresolvableConflict  <br/> |Esse erro indica que a resolução de conflitos não pôde resolver as alterações para as propriedades. Os itens no repositório podem ter sido alterados e precisam ser atualizados. Recupere a chave de alteração atualizada e tente novamente.  <br/> |
|ErrorItemCorrupt  <br/> |Esse erro indica que o estado do objeto está corrompido e não pode ser recuperado. Quando você estiver recuperando um item, apenas determinados elementos estarão nesse estado, como [Body](body.md) e [MimeContent](mimecontent.md). Omita esses elementos e repita a operação.  <br/> |
|ErrorItemNotFound  <br/> |Esse erro ocorre quando o item não foi encontrado ou você não tem permissão para acessar o item.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Esse erro ocorrerá se uma solicitação de propriedade em um item falhar. A propriedade pode existir, mas não pôde ser recuperada.  <br/> |
|ErrorItemSave  <br/> |Esse erro ocorre quando as tentativas de salvar o item ou a pasta falham.  <br/> |
|ErrorItemSavePropertyError  <br/> |Esse erro ocorre quando as tentativas de salvar o item ou a pasta falham devido a valores de propriedade inválidos. O código de resposta inclui o caminho das propriedades inválidas.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Esse erro indica que o serviço de disponibilidade não pôde fazer logon como o serviço de rede para solicitações de proxy para os sites ou florestas apropriados. Essa resposta normalmente indica um erro de configuração.  <br/> |
|ErrorMailboxConfiguration  <br/> |Esse erro indica que as informações de caixa de correio no AD DS estão configuradas incorretamente.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Esse erro indica que o elemento [MailboxDataArray](mailboxdataarray.md) na solicitação está vazio. Você deve fornecer pelo menos um identificador de caixa de correio.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Esse erro ocorre quando mais de 100 entradas são fornecidas em um elemento [MailboxDataArray](mailboxdataarray.md) ..  <br/> |
|ErrorMailboxFailover  <br/> |Esse erro indica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indica que a retenção de caixa de correio não foi encontrada.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Esse erro ocorre quando a conexão com a caixa de correio para obter as informações de exibição do calendário falhou.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Esse erro indica que a caixa de correio está sendo movida para um repositório ou servidor de caixa de correio diferente. Esse erro também pode indicar que a caixa de correio está em outro servidor ou banco de dados de caixa de correio.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Esse erro indica que uma das seguintes condições de erro ocorreu:  <br/><br/>-O repositório de caixa de correio está corrompido.  <br/>– O repositório de caixa de correio está sendo interrompido.  <br/>-O repositório de caixa de correio está offline.  <br/>-Ocorreu um erro de rede quando foi feita uma tentativa de acessar o repositório de caixa de correio.  <br/>– O repositório de caixa de correio está sobrecarregado e não pode aceitar mais conexões.  <br/>– O repositório de caixa de correio foi pausado.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Esse erro ocorrerá se as informações do elemento [MailboxData](mailboxdata.md) não puderem ser mapeadas para uma conta de caixa de correio válida.  <br/> |
|ErrorMailTipsDisabled  <br/> |Esse erro indica que as dicas de email estão desabilitadas.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Esse erro ocorrerá se a pasta gerenciada que você está tentando criar já existir em uma caixa de correio.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Esse erro ocorre quando o nome da pasta que foi especificado na solicitação não é mapeado para uma definição de pasta gerenciada no AD DS. Você só pode criar instâncias de pastas gerenciadas para pastas definidas no AD DS. Verifique o nome e tente novamente.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Esse erro indica que a raiz de pastas gerenciadas foi excluída da caixa de correio ou que uma pasta existe na mesma pasta pai que tem o nome da raiz da pasta gerenciada. Isso também ocorrerá se a tentativa de criar a pasta raiz gerenciada falhar.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Esse erro indica que o mecanismo de sugestões encontrou um problema ao tentar gerar as sugestões.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Esse erro ocorrerá se o atributo **MessageDisposition** não estiver definido.<br/><br/> Este atributo é necessário para o seguinte: <br/> <br/>-A [operação CreateItem](createitem-operation.md) e a [operação UpdateItem](updateitem-operation.md) quando o item que está sendo criado ou atualizado é uma [mensagem](message-ex15websvcsotherref.md).  <br/>- Objetos de resposta [CancelCalendarItem](cancelcalendaritem.md), [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)ou [TentativelyAcceptItem](tentativelyacceptitem.md) .  <br/> |
|ErrorMessageSizeExceeded  <br/> |Esse erro indica que a mensagem que você está tentando enviar excede os limites permitidos.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Esse erro indica que o domínio fornecido não pode ser encontrado.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Esse erro indica que o serviço de controle de mensagens não pode rastrear a mensagem.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Esse erro indica que o serviço de controle de mensagens está inativo ou ocupado. Esse código de erro indica um erro transitório. Os clientes podem repetir a conexão com o servidor quando esse erro é recebido.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Esse erro ocorre quando o conteúdo MIME não é um iCal válido para uma [operação CreateItem](createitem-operation.md). Para uma [operação GetItem](getitem-operation.md), essa resposta indica que o conteúdo MIME não pôde ser gerado.  <br/> |
|ErrorMimeContentInvalid  <br/> |Esse erro ocorre quando o conteúdo MIME é inválido.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Esse erro ocorre quando o conteúdo MIME na solicitação não é uma cadeia de caracteres base 64 válida.  <br/> |
|ErrorMissingArgument  <br/> |Esse erro indica que um argumento necessário estava ausente da solicitação. O texto da mensagem de resposta indica qual argumento deve ser verificado.  <br/> |
|ErrorMissingEmailAddress  <br/> |Esse erro indica que você especificou uma ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um sub-elemento de [caixa de correio](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Esse erro indica que você especificou uma ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um sub-elemento de [caixa de correio](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md). Essa resposta é retornada da [operação CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Esse erro ocorrerá se o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) estiver ausente.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Esse erro ocorrerá se o [ReferenceItemId](referenceitemid.md) estiver ausente.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Este código de erro nunca é retornado.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Esse erro é retornado quando é feita uma tentativa de não incluir o elemento item no elemento item de **anexo** de uma solicitação de [operação CreateAttachment](createattachment-operation.md) .  <br/> |
|ErrorMissingManagedFolderId  <br/> |Esse erro ocorre quando a propriedade IDs de política, a marca de propriedade 0x6732, para a pasta está ausente. Você deve considerar esta pasta corrompida.  <br/> |
|ErrorMissingRecipients  <br/> |Esse erro indica que você tentou enviar um item sem incluir destinatários. Observe que, se você chamar a [operação CreateItem](createitem-operation.md) com uma disposição de mensagem que faz com que a mensagem seja enviada, receberá o seguinte código de resposta: **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Esse erro indica que um [userid](userid.md) não foi totalmente especificado em um conjunto de permissões.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Esse erro indica que você especificou mais de um valor de elemento [ExchangeImpersonation](exchangeimpersonation.md) em uma solicitação.  <br/> |
|ErrorMoveCopyFailed  <br/> |Esse erro indica que a operação de movimentação ou cópia falhou. A movimentação ocorre na [operação CreateItem](createitem-operation.md) quando você aceita uma solicitação de reunião que está na pasta itens excluídos. Além disso, se você recusar uma solicitação de reunião, cancelar um item de calendário ou remover uma reunião do calendário, ela será movida para a pasta itens excluídos.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Esse erro ocorrerá se você tentar mover uma pasta distinta.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Esse erro ocorre quando uma solicitação tenta acessar vários servidores de caixa de correio. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Esse erro ocorrerá se a [operação ResolveNames](resolvenames-operation.md) retornar mais de um resultado ou se o nome ambíguo especificado corresponder a mais de um objeto no diretório. O código de resposta inclui os nomes correspondentes nos dados de resposta.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Esse erro indica que o chamador não tem uma caixa de correio no sistema. A operação [ResolveNames](resolvenames-operation.md) ou [ExpandDL](expanddl-operation.md) é inválida para conectar um usuário sem uma caixa de correio.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Esse erro indica que a [operação ResolveNames](resolvenames-operation.md) não retorna nenhum resultado.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Este código de erro deve ser retornado quando o serviço Web não consegue localizar um servidor para lidar com a solicitação.  <br/> |
|ErrorNoCalendar  <br/> |Esse erro ocorrerá se não houver uma pasta de calendário para a caixa de correio.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de acesso para cliente no site de destino foi configurado para a autenticação do Windows e, portanto, a solicitação não pode ser de proxy.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Esse erro indica que a solicitação se refere a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de acesso para cliente no site de destino foi configurado para conexões SSL e, portanto, a solicitação não pode ser de proxy.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Esse erro indica que a solicitação é referida a uma caixa de correio em outro site do Active Directory, mas nenhum servidor de acesso para cliente no site de destino é de uma versão de produto aceitável para receber a solicitação e, portanto, a solicitação não pôde ser proxy.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Esse erro ocorrerá se você definir o elemento [FolderClass](folderclass.md) quando estiver criando um item diferente de uma pasta genérica. Para pastas digitadas, como [CalendarFolder](calendarfolder.md) e [TasksFolder](tasksfolder.md), a classe Folder é implícita. A definição da classe Folder como um tipo de pasta diferente usando a [operação UpdateFolder](updatefolder-operation.md) resulta na resposta **ErrorObjectTypeChanged** . Em vez disso, use um tipo de pasta genérico, mas defina a classe Folder como o valor que você precisa. Os serviços Web do Exchange criarão a pasta com rigidez de tipos correta.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Esse erro indica que o chamador não tem direitos de exibição de disponibilidade na pasta calendário em questão.  <br/> |
|ErrorNonExistentMailbox  <br/> | Esse erro ocorre nos seguintes cenários: <br/> <br/>-O endereço de email está vazio no [CreateManagedFolder](createmanagedfolder.md).  <br/>– O endereço de email não se refere a uma conta válida em uma solicitação que usa um endereço de email no corpo ou no cabeçalho SOAP, como em uma chamada de representação do Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Esse erro ocorre quando um chamador passa um endereço SMTP não principal. A resposta inclui o endereço SMTP correto a ser usado.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Esse erro indica que as propriedades MAPI no intervalo personalizado, 0x8000 e superior, não podem ser referenciadas por marcas de propriedade. Você deve usar a propriedade [PropertySetId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)da API gerenciada do EWS ou o elemento EWS [ExtendedFieldURI](extendedfielduri.md) com o atributo PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Este código de erro deve ser retornado se nenhum servidor de pasta pública estiver disponível ou se o chamador não tiver um servidor público de casa.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Esse erro indica que a solicitação é referida a uma caixa de correio em outro site do Active Directory, mas nenhum dos servidores de acesso para cliente no site respondeu, e, portanto, a solicitação não pode ser proxy.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Esse erro indica que o chamador tentou conceder permissões em sua pasta de contatos ou calendário para um usuário em outra organização e a tentativa falhou.  <br/> |
|ErrorNotDelegate  <br/> |Esse erro indica que o usuário não é um representante da caixa de correio. Ele é retornado pela [operação Getdelegate](getdelegate-operation.md), pela [operação RemoveDelegate](removedelegate-operation.md)e pela [operação UpdateDelegate](updatedelegate-operation.md) quando o usuário delegado especificado não é encontrado na lista de representantes.  <br/> |
|ErrorNotEnoughMemory  <br/> |Esse erro indica que a operação não pôde ser concluída por causa de memória insuficiente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorObjectTypeChanged  <br/> |Esse erro ocorrerá se o tipo de objeto for alterado.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Esse erro ocorre quando a hora de [início](start.md) ou de [término](end-ex15websvcsotherref.md) de uma ocorrência é atualizada para que a ocorrência seja agendada para acontecer antes ou depois da ocorrência anterior ou seguinte.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Esse erro indica que a alocação de tempo para uma determinada ocorrência se sobrepõe a outra ocorrência do mesmo item recorrente. Essa resposta também ocorre quando o comprimento em minutos de uma determinada ocorrência é maior do que Int32. MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Esse erro indica que a operação atual não é válida para a raiz da pasta pública.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Esse erro indica que a organização do solicitante não é federada para que o solicitante não possa criar mensagens de compartilhamento para enviar para um usuário externo ou não pode aceitar mensagens de compartilhamento recebidas de um usuário externo.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorParentFolderNotFound  <br/> |Esse erro ocorre na [operação CreateFolder](createfolder-operation.md) quando a pasta pai não é encontrada.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Esse erro indica que você deve alterar sua senha antes de poder acessar esta caixa de correio. Isso ocorre quando uma nova conta é criada e o administrador indica que o usuário deve alterar a senha no primeiro logon. Você não pode atualizar a senha usando os serviços Web do Exchange. Você deve usar uma ferramenta como o Microsoft Office Outlook Web App para alterar sua senha.  <br/> |
|ErrorPasswordExpired  <br/> |Esse erro indica que a senha expirou. Você não pode alterar a senha usando os serviços Web do Exchange. Você deve usar uma ferramenta como o Outlook Web App para alterar sua senha.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos para um usuário externo, mas a política de compartilhamento atribuída ao solicitante indica que o nível de permissão solicitado é maior do que o permitido pela política de compartilhamento.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Esse erro indica que o número de telefone não estava no formato correto.  <br/> |
|ErrorPropertyUpdate  <br/> |Esse erro indica que a atualização falhou devido a valores de propriedade inválidos. A mensagem de resposta inclui os caminhos de propriedade inválidos.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Esse erro indica que a solicitação se refere a uma assinatura que existe em outro servidor de acesso para cliente, mas uma tentativa de fazer proxy da solicitação para o servidor de acesso para cliente falhou.  <br/> |
|ErrorProxyCallFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Esse erro indica que a solicitação é referida a uma caixa de correio em outro site do Active Directory e o chamador original é membro de mais de 3.000 grupos.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Esse erro indica que a solicitação que os serviços Web do Exchange enviaram para outro servidor de acesso para cliente ao tentar atender a uma solicitação [GetUserAvailabilityRequest](getuseravailabilityrequest.md) era inválida. Esse código de resposta normalmente indica que ocorreu um erro de configuração ou de direitos, ou que alguém tentou sem êxito a imitar uma solicitação de proxy de disponibilidade.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentaram fazer o proxy de uma solicitação de disponibilidade para outro servidor de acesso para cliente para o atendimento, mas a solicitação falhou. Essa resposta pode ser causada por problemas de conectividade de rede ou por problemas de tempo limite de solicitação.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Este código de erro deve ser retornado se o serviço Web não puder determinar se a solicitação deve ser executada no servidor de destino ou se será proxy para outro servidor.  <br/> |
|ErrorProxyTokenExpired  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Esse erro ocorre quando a URL da caixa de correio de pasta pública não é encontrada. Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Esse erro ocorre quando é feita uma tentativa de acessar uma pasta pública e a tentativa não é bem sucedida. Esse erro foi introduzido no Exchange 2013Caixa Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Esse erro ocorre quando o destinatário passado para a [operação GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server anterior ao Exchange 2007, e a solicitação para recuperar as informações de disponibilidade do destinatário do servidor de pasta pública falhou.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Este erro ocorre quando o destinatário passado para a [operação GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server anterior ao Exchange 2007, e a solicitação para recuperar informações de disponibilidade para o destinatário do servidor de pasta pública falhou porque a unidade organizacional não tinha um servidor de pasta pública associado.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Esse erro ocorre quando uma operação de sincronização é bem-sucedida em relação à caixa de correio de pasta pública principal, mas não é bem-sucedida na caixa de correio de pasta pública secundária. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Esse erro indica que a restrição de pasta de pesquisa pode ser válida, mas não é suportada pelo EWS. Os serviços Web do Exchange limitam as restrições para conter um máximo de 255 expressões de filtro. Se você tentar vincular a uma pasta de pesquisa existente que excede 255, esse código de resposta será retornado.  <br/> |
|ErrorQuotaExceeded  <br/> |Esse erro ocorre quando a cota da caixa de correio é excedida.  <br/> |
|ErrorReadEventsFailed  <br/> |Este erro é retornado pela [operação GetEvents](getevents-operation.md) ou notificações por push quando ocorre uma falha ao recuperar informações de evento. Quando esse erro é retornado, a assinatura é excluída. Recrie a sincronização de eventos com base em uma última marca d' água conhecida.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Esse erro é retornado pela [operação CreateItem](createitem-operation.md) se for feita uma tentativa de suprimir uma confirmação de leitura quando o remetente da mensagem não solicitar uma confirmação de leitura na mensagem ou se a mensagem estiver na pasta lixo eletrônico.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Esse erro ocorre quando a data de término da recorrência é após 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Esse erro ocorre quando a recorrência especificada não tem nenhuma instância de ocorrência no intervalo especificado.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Esse erro indica que a lista de representantes não pôde ser salva depois que os delegados foram removidos.  <br/> |
|ErrorRequestAborted  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Esse erro ocorre quando o fluxo de solicitação é maior que 400 KB.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Este erro é retornado quando uma propriedade obrigatória está ausente em uma solicitação de [operação CreateAttachment](createattachment-operation.md) . O URI de propriedade ausente está incluído na resposta.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Esse erro indica que o chamador especificou uma pasta que não é uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Esse erro indica que o chamador especificou mais de uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorRestrictionTooLong  <br/> |Esse erro ocorrerá se a restrição contiver mais de 255 nós.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Esse erro ocorre quando a restrição não pode ser avaliada pelos serviços Web do Exchange.  <br/> |
|ErrorResultSetTooBig  <br/> |Esse erro indica que o número de entradas de calendário para um determinado destinatário excede o limite permitido de 1000. Reduza a janela e tente novamente.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Este erro ocorre quando o [SavedItemFolderId](saveditemfolderid.md) não é encontrado.  <br/> |
|ErrorSchemaValidation  <br/> | Esse erro ocorre quando a solicitação não pode ser validada em relação ao esquema.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Esse erro indica que a pasta de pesquisa foi criada, mas os critérios de pesquisa nunca foram definidos na pasta. Isso ocorre somente quando você acessa pastas de pesquisa corrompidas que foram criadas usando outra API ou outro cliente. Para corrigir esse erro, use a [operação UpdateFolder](updatefolder-operation.md) para definir o elemento [SearchParameters](searchparameters.md) para incluir a restrição que deve estar na pasta.  <br/> |
|ErrorSendAsDenied  <br/> | Este erro ocorre quando ocorrem as duas condições a seguir: <br/> <br/>– Um usuário recebeu permissões de CanActAsOwner, mas não concedeu direitos de representante na caixa de correio da entidade de segurança.  <br/>– O mesmo usuário tenta criar e enviar uma mensagem de email na caixa de correio da entidade de segurança usando a opção SendAndSaveCopy.<br/>  <br/>  O resultado é um erro ErrorSendAsDenied e a criação da mensagem de email na pasta Rascunhos da entidade de segurança.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Esse erro é retornado pela [Operação DeleteItem](deleteitem-operation.md) se o atributo **SendMeetingCancellations** estiver ausente da solicitação e o item a ser excluído for um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Esse erro é retornado pela [operação UpdateItem](updateitem-operation.md) se o atributo **SendMeetingInvitationsOrCancellations** estiver ausente da solicitação e o item a ser atualizado for um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Esse erro é retornado pela [operação CreateItem](createitem-operation.md) se o atributo **SendMeetingInvitations** estiver ausente da solicitação e o item a ser criado for um item de calendário.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Esse erro indica que depois que o organizador enviar uma solicitação de reunião, a solicitação não poderá ser atualizada. Para modificar a reunião, modifique o item do calendário, não a solicitação de reunião.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Esse erro indica que depois que o iniciador da tarefa envia uma solicitação de tarefa, essa solicitação não pode ser atualizada.  <br/> |
|ErrorServerBusy  <br/> |Esse erro ocorre quando o servidor está ocupado.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentaram fazer o proxy de uma solicitação de disponibilidade do usuário para a floresta apropriada para o destinatário, mas não foi possível determinar onde enviar a solicitação devido a uma falha de descoberta de serviço.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Esse erro indica que a propriedade de URL externa não foi definida no banco de dados do Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Esse erro indica que uma tentativa de sincronização de uma pasta de compartilhamento falhou. <br/><br/>Este código de erro é retornado quando ocorre o seguinte:<br/><br/>– A assinatura de uma pasta de compartilhamento não foi encontrada.<br/>-A pasta de compartilhamento não foi encontrada.<br/>-O usuário de diretório correspondente não foi encontrado.<br/>-O usuário não existe mais.<br/>-O compromisso é inválido.<br/>-O item de contato é inválido.<br/>-Há uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorStaleObject  <br/> |Esse erro ocorre em uma [operação UpdateItem](updateitem-operation.md) ou em uma [operação SendItem](senditem-operation.md) quando a tecla Change não está atualizada ou não foi fornecida. Chame a [operação GetItem](getitem-operation.md) para recuperar uma chave de alteração atualizada e repita a operação.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Esse erro indica que um usuário não pode enviar mais solicitações imediatamente porque a cota de envio foi atingida.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Esse erro ocorre quando você tenta acessar uma assinatura usando uma conta que não criou essa assinatura. Cada assinatura só pode ser acessada pelo criador da assinatura.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Esse erro indica que você não pode criar uma assinatura se não for o proprietário ou não tiver acesso de proprietário à caixa de correio.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Esse erro ocorrerá se a assinatura que corresponde ao [SubscriptionId especificado (GetEvents)](subscriptionid-getevents.md) não for encontrada. A assinatura pode ter expirado, o processo dos serviços Web do Exchange pode ter sido reiniciado ou uma assinatura inválida foi passada. Se a assinatura for válida, recrie a assinatura com a marca d' água mais recente. Isso é retornado pela [operação unsubscribe](unsubscribe-operation.md) ou as respostas da [operação GetEvents](getevents-operation.md) .  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Este código de erro deve ser retornado quando uma solicitação é feita para uma assinatura que tenha sido cancelada.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Esse erro é retornado pela [operação SyncFolderItems](syncfolderitems-operation.md) se a pasta pai especificada não for encontrada.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Esse erro indica que uma caixa de correio de equipe não foi encontrada. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas não está vinculada a um SharePoint Server. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas que o link para o servidor do SharePoint não é válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Este código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Este código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Esse erro indica que uma tentativa de enviar uma notificação para os proprietários da caixa de correio da equipe não foi bem sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Esse erro indica um erro geral que pode ocorrer ao tentar acessar uma caixa de correio de equipe. Tente enviar a solicitação mais tarde. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Esse erro indica que a janela de tempo especificada é maior do que o limite permitido. Por padrão, o limite permitido é 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Esse erro ocorre quando não há tempo suficiente para concluir o processamento da solicitação.  <br/> |
|ErrorTimeZone  <br/> |Esse erro indica que há um erro de fuso horário.  <br/> |
|ErrorToFolderNotFound  <br/> |Esse erro indica que a pasta de destino não existe.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Esse erro ocorrerá se o chamador tentar fazer uma solicitação de serialização de token, mas não tiver o direito ms-Exch-EPI-TokenSerialization no servidor de acesso para cliente.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Esse erro ocorre quando o limite interno de objetos abertos foi excedido.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Esse erro indica que o plano de discagem de um usuário não está disponível.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Esse erro indica que o usuário não pôde ser encontrado.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Esse erro indica que um servidor válido para o plano de discagem pode ser encontrado para lidar com a solicitação.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Esse erro ocorre quando uma tentativa malsucedida de remover um contato de mensagens instantâneas de um grupo. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Esse erro ocorre quando você tenta definir a propriedade **Culture** como um valor que não é analisável pela classe **System. Globalization. CultureInfo** .  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Esse erro ocorre quando um chamador tenta usar propriedades estendidas de objeto de tipos, matriz de objeto, erro ou nulo.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Esse erro ocorre quando você está tentando recuperar ou definir o conteúdo MIME para um item diferente de um objeto [PostItem](postitem.md), [Message](message-ex15websvcsotherref.md)ou [CalendarItem](calendaritem.md) .  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Esse erro ocorre quando o chamador passa uma propriedade que é inválida para uma consulta. Isso pode ocorrer quando Propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Esse erro ocorre quando o chamador passa uma propriedade que é inválida para uma Propriedade Sort ou Group by. Isso pode ocorrer quando Propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Esse erro indica que a restrição de pasta de pesquisa pode ser válida, mas não é suportada pelo EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Esse erro indica que a recorrência especificada não é suportada para tarefas.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Esse erro indica que os serviços Web do Exchange localizaram um tipo de propriedade no repositório, mas não podem gerar XML para o tipo de propriedade.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Esse erro indica que a lista de representantes não pôde ser salva após os delegados serem atualizados.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Esse erro ocorre quando o único caminho de propriedade que está listado em uma descrição de alteração não corresponde à propriedade única que está sendo definida no objeto [Item](item.md) ou [Folder](folder.md) real.  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Esse erro indica que o solicitante não está habilitado.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões em seu calendário ou pasta de contatos para um usuário externo, mas a política de compartilhamento atribuída ao solicitante indica que o domínio do usuário externo não está listado na política.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indica que a organização do solicitante tem um conjunto de domínios federados, mas a organização do solicitante não tem nenhum endereço de proxy SMTP com um dos domínios federados.  <br/> |
|ErrorValueOutOfRange  <br/> |Esse erro indica que uma data de início ou de término da exibição do calendário foi definida como 1/1/0001 12:00:00 AM ou 12/31/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Esse erro indica que o repositório do Exchange detectou um vírus na mensagem.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Esse erro indica que o repositório do Exchange detectou um vírus na mensagem e o excluiu.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWin32InteropError  <br/> |Esse erro indica que houve uma falha interna durante a comunicação com o código não gerenciado.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWrongServerVersion  <br/> |Esse erro indica que uma solicitação só pode ser feita para um servidor que seja a mesma versão do servidor de caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Esse erro indica que uma solicitação foi feita por um representante que tem uma versão de servidor diferente do servidor de caixa de correio da entidade de segurança.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Este código de erro nunca é retornado.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Especifica que há cabeçalhos SOAP duplicados.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Especifica que uma tentativa de sincronização de uma pasta de compartilhamento falhou.<br/><br/> Este código de erro deve ser retornado quando:<br/><br/>– A assinatura de uma pasta de compartilhamento não foi encontrada.  <br/>-A pasta de compartilhamento não foi encontrada.  <br/>-O usuário de diretório correspondente não foi encontrado.  <br/>-O usuário não existe mais.  <br/>-O compromisso é inválido.  <br/>-O item de contato é inválido.  <br/>-Houve uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Especifica que a propriedade de URL externa não foi definida no banco de dados do Active Directory. Este código de erro deve ser retornado se a propriedade de URL externa não tiver sido definida no banco de dados do Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Especifica que a contagem de membros do grupo máximo foi atingida para obter informações de disponibilidade de uma lista de distribuição. Este erro deve ser retornado quando a contagem de membros do grupo máximo tiver sido atingida para obter informações de disponibilidade de uma lista de distribuição.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Especifica que o tipo de dados e o elemento ShareFolderId estão presentes em uma solicitação. Esse código de erro deve ser retornado se o elemento DataType e ShareFolderId estão presentes em uma solicitação.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Especifica que o chamador tentou conceder permissões em sua pasta de contatos ou calendário a um usuário em outra organização e a tentativa falhou. Este código de erro deve ser retornado quando a política de compartilhamento estiver desabilitada para o chamador ou quando a política de compartilhamento atribuída ao chamador não permitir o compartilhamento para o nível solicitado ou o tipo de pasta solicitada.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Especifica que o solicitante tentou conceder permissões em sua pasta de contatos ou calendário a um usuário externo, mas a política de compartilhamento atribuída ao solicitante especifica que o domínio do usuário externo não está listado na política.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Especifica que o solicitante tentou conceder permissões em sua pasta de contatos ou calendário para um usuário externo, mas a política de compartilhamento atribuída ao solicitante especifica que o nível de permissão solicitado é maior do que o permitido pela política de compartilhamento.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Especifica que a organização do solicitante não é federada para que o solicitante não possa criar mensagens de compartilhamento para enviar para um usuário externo ou não pode aceitar mensagens de compartilhamento recebidas de um usuário externo. Este código de erro deve ser retornado se a organização do solicitante não é federada.  <br/> |
|ErrorMailboxFailover  <br/> |Especifica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Especifica que o remetente do convite de compartilhamento não criou os metadados do convite de compartilhamento. Este código de erro deve ser retornado se o remetente do convite de compartilhamento não tiver criado os metadados de convite de compartilhamento.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Especifica que o serviço de controle de mensagens não pode rastrear a mensagem.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Especifica que o serviço de controle de mensagens está inoperante ou ocupado. Este código de erro especifica um erro transitório. Os clientes podem repetir a conexão com o servidor quando esse erro é recebido.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Especifica que o domínio fornecido não pode ser encontrado.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Especifica que a organização do solicitante tem um conjunto de domínios federados, mas a organização do solicitante não tem nenhum endereço de proxy SMTP com um dos domínios federados.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Especifica que um chamador solicitou informações de disponibilidade para um usuário em outra organização, mas a relação organizacional não tem disponibilidade habilitada.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Especifica que os objetos de Federação da organização do solicitante não estão configurados corretamente.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Especifica que uma mensagem de compartilhamento não se destina ao chamador.  <br/> |
|ErrorInvalidSharingData  <br/> |Especifica que os metadados de compartilhamento não são válidos. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Esse erro deve ser retornado se uma ação não pode ser aplicada a um ou mais itens na conversa.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Este erro deve ser retornado se qualquer regra não for validada.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Este erro deve ser retornado quando uma tentativa de gerenciar regras de caixa de entrada ocorre após outro cliente ter acessado as regras de caixa de entrada.  <br/> |
|ErrorRulesOverQuota  <br/> |Este erro deve ser retornado quando a cota da regra de um usuário foi excedida.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Esse erro deve ser retornado para a primeira conexão de assinatura se uma segunda conexão de assinatura for aberta.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Este erro deve ser retornado quando notificações de eventos estão ausentes.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Esse erro é retornado quando há nomes distintos herdados duplicados nos serviços de domínio do Active Directory (AD DS). Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Esse erro indica que uma solicitação para obter um token de acesso do cliente não era válida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Esse erro será retornado se o cabeçalho [ManagementRole](managementrole.md) no cabeçalho SOAP estiver incorreto. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Este erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Esse erro é retornado quando uma tentativa de pesquisa com escopo é realizada sem usar um elemento [QueryString (cadeia de caracteres)](querystring-string.md) para uma pesquisa de indexação de conteúdo. Isso é aplicável às operações **SearchMailboxes** e **FindConversation** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Este erro é retornado quando uma pesquisa de caixa de correio de arquivo morto não é bem-sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Este erro é retornado quando a URL de uma caixa de correio de arquivo morto não é detectável. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Esse erro ocorre quando a operação para obter a pasta de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Este erro ocorre quando a operação para localizar a pasta de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Esse erro ocorre quando a operação para obter o item de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Esse erro ocorre quando a operação para exportar itens de caixa de correio de arquivo morto remoto falhou.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Esse erro será retornado se um tamanho de foto inválido for solicitado a partir do servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Esse erro é retornado quando um tamanho de foto inesperado é solicitado em uma solicitação de operação **GetUserPhoto** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Este erro é retornado quando uma solicitação de operação **SearchMailboxes** contém muitas caixas de correio para pesquisa. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Esse erro indica que nenhuma marca de retenção foi encontrada para este usuário. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Este erro é retornado quando pesquisas de descoberta estão desabilitadas em um locatário ou servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Este erro ocorre ao tentar invocar a [operação FindItem](finditem-operation.md) com um [SeekToConditionPageItemView](seektoconditionpageitemview.md) para buscar itens de calendário, o que não é suportado.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Este erro é destinado apenas para uso interno.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |O locatário está marcado para remoção.  <br/> |
|ErrorInvalidLicense  <br/> |O usuário não tem uma licença válida.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |A cota de recebimento de mensagens por pasta foi excedida.  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento não é obrigatório e não está incluído em todas as respostas. 
  
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

