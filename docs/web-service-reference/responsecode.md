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
ms.openlocfilehash: 7baeb0ab87ffb43ba9d6b4016477888aa4ed613e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825294"
---
# <a name="responsecode"></a>ResponseCode

O elemento **ResponseCode** fornece informações de status sobre a solicitação. 
  
- [ResponseMessage](responsemessage.md) 
- [ResponseCode](responsecode.md)
  
```XML
<ResponseCode/>
```

**ResponseCodeType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|Elemento|Descrição|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | Fornece informações descritivas sobre o status de resposta.<br/><br/>  A seguir estão as expressões XPath possíveis para esse elemento:<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação DeleteItem](deleteitem-operation.md) solicitação.  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação SendItem](senditem-operation.md) solicitação.  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação DeleteFolder](deletefolder-operation.md) solicitação.  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação DeleteAttachment](deleteattachment-operation.md) solicitação.  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação de cancelamento da assinatura](unsubscribe-operation.md) .  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CreateFolder](createfolder-operation.md) solicitação.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação GetFolder](getfolder-operation.md) solicitação.  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação UpdateFolder](updatefolder-operation.md) solicitação.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação MoveFolder](movefolder-operation.md) solicitação.  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CopyFolder](copyfolder-operation.md)solicitação.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CreateManagedFolder](createmanagedfolder-operation.md) solicitação.  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação FindFolder](findfolder-operation.md) solicitação.  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação CreateItem](createitem-operation.md) .  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação GetItem](getitem-operation.md) solicitação.  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação UpdateItem](updateitem-operation.md) solicitação.  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação MoveItem](moveitem-operation.md) solicitação.  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CopyItem](copyitem-operation.md) solicitação.  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CreateAttachment](createattachment-operation.md) solicitação.  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação GetAttachment](getattachment-operation.md) solicitação.  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação FindItem](finditem-operation.md) solicitação.  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação ResolveNames](resolvenames-operation.md) .  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação ExpandDL](expanddl-operation.md) solicitação.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação [Subscribe operação](subscribe-operation.md) .  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação GetEvents](getevents-operation.md) solicitação.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de operação SendNotification.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação SyncFolderHierarchy](syncfolderhierarchy-operation.md) .  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação SyncFolderItems](syncfolderitems-operation.md) .  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação ConvertId](convertid-operation.md) .  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação AddDelegate](adddelegate-operation.md) .  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetDelegate](getdelegate-operation.md) .  <br/> |
|[RemoveDelegateResponse](removedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação RemoveDelegate](removedelegate-operation.md) .  <br/> |
|[UpdateDelegateResponse](updatedelegateresponse.md) <br/> |Contém o status e o resultado de uma solicitação de [operação UpdateDelegate](updatedelegate-operation.md) .  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação de [operação GetSharingFolder](getsharingfolder-operation.md) .  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |Define uma resposta a uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |Define uma resposta a uma solicitação de [operação RefreshSharingFolder](refreshsharingfolder-operation.md) .  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |Contém o status e os resultados de uma [operação de FindConversation](findconversation-operation.md) de resposta.  <br/> |
|[ApplyConversationActionResponseMessage](applyconversationactionresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação de [operação ApplyConversationAction](applyconversationaction-operation.md) .  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação EmptyFolder](emptyfolder-operation.md) .  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |Contém um resultado de uma solicitação de [operação UpdateInboxRules](updateinboxrules-operation.md) e status.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém um resultado de uma solicitação de [operação UploadItems](uploaditems-operation.md) e status.  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Contém uma resposta a uma [operação de GetInboxRules](getinboxrules-operation.md) * * * solicitação.  <br/> |
|[GetServiceConfigurationResponse](getserviceconfigurationresponse.md) <br/> |Contém uma resposta a uma solicitação de [operação GetServiceConfiguration](getserviceconfiguration-operation.md) .  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |Contém as definições de configuração de serviço.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto. A tabela a seguir descreve os valores que são retornados com esse elemento.
  
|Value|Descrição|
|:-----|:-----|
|NoError  <br/> |Nenhum erro ocorreu para a solicitação.  <br/> |
|ErrorAccessDenied  <br/> |Este erro ocorre quando a conta de chamada não tem os direitos para executar a ação solicitada.  <br/> |
|ErrorAccessModeSpecified  <br/> |Esse erro é apenas para uso interno. Esse erro não será retornado.  <br/> |
|ErrorAccountDisabled  <br/> |Este erro ocorre quando a conta em questão tiver sido desativada.  <br/> |
|ErrorAddDelegatesFailed  <br/> |Este erro ocorre quando uma lista com representantes adicionados não pode ser salvos.  <br/> |
|ErrorAddressSpaceNotFound  <br/> |Este erro ocorre quando o registro de espaço de endereço ou nome de domínio do sistema de nome de domínio (DNS), para disponibilidade entre florestas não pôde ser encontrado no banco de dados do Active Directory.  <br/> |
|ErrorADOperation  <br/> |Este erro ocorre quando a operação falhou devido a problemas de comunicação com os serviços de domínio Active Directory (AD DS).  <br/> |
|ErrorADSessionFilter  <br/> |Esse erro é retornado quando uma solicitação de operação **ResolveNames** Especifica um nome que não é válido.  <br/> |
|ErrorADUnavailable  <br/> |Este erro ocorre quando o AD DS não está disponível. Tente a solicitação novamente mais tarde.  <br/> |
|ErrorAffectedTaskOccurrencesRequired  <br/> |Esse erro indica que o atributo **AffectedTaskOccurrences** não foi especificado. Quando o elemento [DeleteItem](deleteitem.md) é usado para excluir a pelo menos um item que é uma tarefa e independentemente se essa tarefa for recorrente ou não, o atributo **AffectedTaskOccurrences** deve ser especificadas para que possa determinar a **DeleteItem** se Para excluir a ocorrência atual ou a série inteira.  <br/> |
|ErrorArchiveFolderPathCreation  <br/> |Indica um erro na criação de caminho de pasta de arquivamento.  <br/> |
|ErrorArchiveMailboxNotEnabled  <br/> |Indica que a caixa de correio de arquivo morto não foi ativada.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Indica a falha de descoberta do serviço de caixa de correio desse arquivo morto.  <br/> |
|ErrorAttachmentNestLevelLimitExceeded  <br/> |Especifica o que foi feita uma tentativa de criar um item com mais de 10 anexos aninhados. Esse valor foi introduzido no Exchange Server 2010 Service Pack 2 (SP2).  <br/> |
|ErrorAttachmentSizeLimitExceeded  <br/> |O elemento [CreateAttachment](createattachment.md) retorna este erro, se for feita uma tentativa para criar um anexo com tamanho excedendo Int32.MaxValue, em bytes.  <br/> O elemento [GetAttachment](getattachment.md) retorna este erro se tentar recuperar um anexo existente com tamanho excedendo Int32.MaxValue, em bytes.  <br/> |
|ErrorAutoDiscoverFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentou determinar o local de um computador entre florestas que está executando o Exchange 2010 que tem a função de servidor acesso para cliente instalada usando o serviço de descoberta automática, mas a chamada para o serviço Descoberta automática Falha.  <br/> |
|ErrorAvailabilityConfigNotFound  <br/> |Esse erro indica que as informações de configuração de disponibilidade para a floresta local estão ausentes do AD DS.  <br/> |
|ErrorBatchProcessingStopped  <br/> | Esse erro indica que ocorreu uma exceção durante o processamento de um item e exceção é provável que ocorram para os itens que seguem. Solicitações podem incluir vários itens; Por exemplo, uma solicitação de operação GetItem pode incluir vários identificadores. Em geral, os itens são processadas uma de cada vez. Se ocorrer uma exceção durante o processamento de um item e essa exceção é provável que ocorra para os itens que seguem, itens que seguem não serão processados.  <br/><br/>  A seguir estão exemplos de erros que irá parar o processamento de itens que seguem:<br/>  <br/>-ErrorAccessDenied  <br/>-ErrorAccountDisabled  <br/>-ErrorADUnavailable  <br/>-ErrorADOperation  <br/>-ErrorConnectionFailed  <br/>-ErrorMailboxStoreUnavailable  <br/>-ErrorMailboxMoveInProgress  <br/>-ErrorPasswordChangeRequired  <br/>-ErrorPasswordExpired  <br/>-ErrorQuotaExceeded  <br/>-ErrorInsufficientResources  <br/> |
|ErrorCalendarCannotMoveOrCopyOccurrence  <br/> |Este erro ocorre quando é feita uma tentativa para mover ou copiar uma ocorrência de um item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> | Este erro ocorre quando é feita uma tentativa para atualizar um item de calendário que está localizado na pasta Itens excluídos e quando cancelamentos ou atualizações de reunião devem ser enviados de acordo com o valor do atributo **SendMeetingCancellations** . <br/><br/>Estes são os valores possíveis para este atributo:  <br/><br/>-SendToAllAndSaveCopy  <br/>-SendToChangedAndSaveCopy  <br/>-SendOnlyToAll  <br/>-SendOnlyToChanged  <br/>  <br/>No entanto, tal atualização é permitida apenas quando o valor deste atributo é definido como SendToNone.  <br/> |
|ErrorCalendarCannotUseIdForOccurrenceId  <br/> |Este erro ocorre quando a operação UpdateItem, GetItem, DeleteItem, MoveItem, CopyItem ou SendItem é chamada e a ID especificada não é uma ID de ocorrência de qualquer item de calendário recorrente.  <br/> |
|ErrorCalendarCannotUseIdForRecurringMasterId  <br/> |Este erro ocorre quando a operação **UpdateItem**, **GetItem**, **DeleteItem**, **MoveItem**, **CopyItem**ou **SendItem** é chamada e a ID especificada não é uma ID de qualquer item mestre recorrente.  <br/> |
|ErrorCalendarDurationIsTooLong  <br/> |Esse erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando uma duração de item de calendário for maior que o máximo permitido, que está sendo 5 anos.  <br/> |
|ErrorCalendarEndDateIsEarlierThanStartDate  <br/> |Este erro ocorre quando uma hora de término do calendário está definida ao mesmo tempo ou após a hora de início.  <br/> |
|ErrorCalendarFolderIsInvalidForCalendarView  <br/> |Este erro ocorre quando a pasta especificada para uma operação **FindItem** com um elemento de [exibição de calendário](calendarview.md) não é do tipo de pasta de calendário.  <br/> |
|ErrorCalendarInvalidAttributeValue  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidDayForTimeChangePattern  <br/> |Este erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando valores inválidos do dia, WeekendDay e Weekday são usados para definir o padrão de alteração de tempo.  <br/> |
|ErrorCalendarInvalidDayForWeeklyRecurrence  <br/> |Este erro ocorre durante uma operação **CreateItem** ou **UpdateItem** quando valores inválidos do dia, dia da semana e WeekendDay são usados para especificar a recorrência semanal.  <br/> |
|ErrorCalendarInvalidPropertyState  <br/> |Este erro ocorre quando o estado de um calendário item recorrência objeto binário grande (BLOB) no armazenamento do Exchange é inválido.  <br/> |
|ErrorCalendarInvalidPropertyValue  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorCalendarInvalidRecurrence  <br/> |Este erro ocorre quando a recorrência especificada não pode ser criada.  <br/> |
|ErrorCalendarInvalidTimeZone  <br/> |Este erro ocorre quando um fuso horário inválido for encontrado.  <br/> |
|ErrorCalendarIsCancelledForAccept  <br/> |Esse erro indica que um item do calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForDecline  <br/> |Esse erro indica que um item do calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForRemove  <br/> |Esse erro indica que um item do calendário foi cancelado.  <br/> |
|ErrorCalendarIsCancelledForTentative  <br/> |Esse erro indica que um item do calendário foi cancelado.  <br/> |
|ErrorCalendarIsDelegatedForAccept  <br/> |Esse erro indica que o elemento [AcceptItem](acceptitem.md) é inválido para uma solicitação de reunião ou de item de calendário em um cenário delegada.  <br/> |
|ErrorCalendarIsDelegatedForDecline  <br/> |Esse erro indica que o elemento de [DeclineItem](declineitem.md) é inválido para uma solicitação de reunião ou de item de calendário em um cenário delegada.  <br/> |
|ErrorCalendarIsDelegatedForRemove  <br/> |Esse erro indica que o elemento [RemoveItem](removeitem.md) é inválido para o cancelamento da reunião em um cenário delegado.  <br/> |
|ErrorCalendarIsDelegatedForTentative  <br/> |Esse erro indica que o elemento [TentativelyAcceptItem](tentativelyacceptitem.md) é inválido para uma solicitação de reunião ou de item de calendário em um cenário delegada.  <br/> |
|ErrorCalendarIsNotOrganizer  <br/> |Esse erro indica que a operação (atualmente CancelItem) no item de calendário não é válida para um participante. Somente o organizador da reunião pode cancelar a reunião.  <br/> |
|ErrorCalendarIsOrganizerForAccept  <br/> |Esse erro indica que [AcceptItem](acceptitem.md) é inválida para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForDecline  <br/> |Esse erro indica que o [DeclineItem](declineitem.md) é inválido para o item de calendário do organizador.  <br/> |
|ErrorCalendarIsOrganizerForRemove  <br/> |Esse erro indica que [RemoveItem](removeitem.md) é inválida para o item de calendário do organizador. Para remover uma reunião do calendário, o organizador deve usar CancelCalendarItem.  <br/> |
|ErrorCalendarIsOrganizerForTentative  <br/> |Esse erro indica que [TentativelyAcceptItem](tentativelyacceptitem.md) é inválida para o item de calendário do organizador.  <br/> |
|ErrorCalendarMeetingRequestIsOutOfDate  <br/> |Esse erro indica que uma solicitação de reunião está desatualizada e não pode ser atualizada.  <br/> |
|ErrorCalendarOccurrenceIndexIsOutOfRecurrenceRange  <br/> |Esse erro indica que o índice de ocorrência não aponta para uma ocorrência na recorrência atual. Por exemplo, se seu padrão de recorrência define um conjunto de três ocorrências de reunião e tentar acessar a ocorrência quinta, resultará este código de resposta.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Esse erro indica que qualquer operação em uma ocorrência excluída (endereçada via recorrente índice ID e a ocorrência mestre) é inválida.  <br/> |
|ErrorCalendarOutOfRange  <br/> |Esse erro é relatado nas operações de CreateItem e UpdateItem para itens de calendário ou propriedades de recorrência da tarefa, quando o valor da propriedade estiver fora do intervalo. Por exemplo, especificar a décimo quinta semana do mês resultará neste código de resposta.  <br/> |
|ErrorCalendarViewRangeTooBig  <br/> |Este erro ocorre quando inicia a gama de fim para o elemento [CalendarView](calendarview.md) é maior do que o máximo permitido, atualmente 2 anos.  <br/> |
|ErrorCallerIsInvalidADAccount  <br/> |Esse erro indica que a conta solicitante não é uma conta válida do banco de dados do diretório.  <br/> |
|ErrorCannotArchiveCalendarContactTaskFolderException  <br/> |Indica que foi feita uma tentativa para arquivar uma pasta de contato de tarefa do calendário.  <br/> |
|ErrorCannotArchiveItemsInPublicFolders  <br/> |Indica que foi feita uma tentativa arquivem itens em pastas públicas.  <br/> |
|ErrorCannotArchiveItemsInArchiveMailbox  <br/> |Indica que houve tentativa para arquivar os itens na caixa de correio de arquivo morto.  <br/> |
|ErrorCannotCreateCalendarItemInNonCalendarFolder  <br/> |Este erro ocorre quando um item do calendário está sendo criado e o atributo **SavedItemFolderId** refere-se a uma pasta de calendário não.  <br/> |
|ErrorCannotCreateContactInNonContactFolder  <br/> |Este erro ocorre quando um contato está sendo criado e o atributo **SavedItemFolderId** refere-se a uma pasta de contatos não.  <br/> |
|ErrorCannotCreatePostItemInNonMailFolder  <br/> |Esse erro indica que um item de postagem não pode ser criado em uma pasta diferente de uma pasta de email, como calendário, contatos, tarefas, anotações e assim por diante.  <br/> |
|ErrorCannotCreateTaskInNonTaskFolder  <br/> |Este erro ocorre quando uma tarefa está sendo criada e o atributo **SavedItemFolderId** refere-se para uma pasta não-tarefa.  <br/> |
|ErrorCannotDeleteObject  <br/> |Este erro ocorre quando o item ou a pasta a ser excluída não pode ser excluída.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |A [operação DeleteItem](deleteitem-operation.md) retorna este erro quando ele falhar ao excluir a ocorrência atual de uma tarefa recorrente. Isso só pode acontecer se o atributo **AffectedTaskOccurrences** tiver sido definido como SpecifiedOccurrenceOnly.  <br/> |
|ErrorCannotDisableMandatoryExtension  <br/> |Indica que foi feita uma tentativa para desabilitar uma extensão de mandatorty.  <br/> |
|ErrorCannotEmptyFolder  <br/> |Esse erro deve ser retornado quando o servidor não é possível esvaziar a uma pasta.  <br/> |
|ErrorCannotGetSourceFolderPath  <br/> |Indica que o caminho da pasta de origem não pôde ser recuperado.  <br/> |
|ErrorCannotGetExternalEcpUrl  <br/> |Especifica que o servidor não pôde recuperar a URL externa para as opções do Outlook Web App.  <br/> |
|ErrorCannotOpenFileAttachment  <br/> |A operação **GetAttachment** retorna este erro se não for possível recuperar o corpo de um anexo de arquivo.  <br/> |
|ErrorCannotSetCalendarPermissionOnNonCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões de calendário em uma pasta de calendário não.  <br/> |
|ErrorCannotSetNonCalendarPermissionOnCalendarFolder  <br/> |Esse erro indica que o chamador tentou definir permissões de calendário não em uma pasta de calendário.  <br/> |
|ErrorCannotSetPermissionUnknownEntries  <br/> |Esse erro indica que você não pode definir permissões desconhecidas em um conjunto de permissões.  <br/> |
|ErrorCannotSpecifySearchFolderAsSourceFolder  <br/> |Indica que foi feita uma tentativa para especificar a pasta de pesquisa como a pasta de origem.  <br/> |
|ErrorCannotUseFolderIdForItemId  <br/> |Este erro ocorre quando uma solicitação que exige um identificador de item recebe um identificador de pasta.  <br/> |
|ErrorCannotUseItemIdForFolderId  <br/> |Este erro ocorre quando uma solicitação que exige um identificador de pasta recebe um identificador de item.  <br/> |
|ErrorChangeKeyRequired  <br/> |Este código de resposta foi substituído pelo **ErrorChangeKeyRequiredForWriteOperations** <br/> |
|ErrorChangeKeyRequiredForWriteOperations  <br/> |Esse erro é retornado quando a chave de alteração para um item está ausente ou obsoletos. <br/><br/>Para operações SendItem, UpdateItem e UpdateFolder, o chamador deve passar em uma chave de alteração atual e corretos para o item. Observe que esse é o caso com UpdateItem mesmo quando a resolução de conflito está definida como overwrite sempre.  <br/> |
|ErrorClientDisconnected  <br/> |Especifica que o cliente foi desconectado.  <br/> |
|ErrorClientIntentInvalidStateDefinition  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorClientIntentNotFound  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorConnectionFailed  <br/> |Este erro ocorre quando os serviços Web do Exchange não pode se conectar à caixa de correio.  <br/> |
|ErrorContainsFilterWrongType  <br/> |Esse erro indica que a propriedade que foi inspecionada para um filtro contém não é um tipo de cadeia de caracteres.  <br/> |
|ErrorContentConversionFailed  <br/> |A operação de **GetItem** retorna este erro quando os serviços Web do Exchange não é capaz de recuperar o conteúdo MIME para o item solicitado. <br/><br/>A operação **CreateItem** retorna este erro quando os serviços Web do Exchange não é capaz de criar o item de conteúdo MIME fornecido. Geralmente, essa é uma indicação de que a propriedade item está corrompida ou truncada.  <br/> |
|ErrorContentIndexingNotEnabled  <br/> |Este erro ocorre quando uma solicitação de pesquisa é feita usando a opção de sequência de consulta e indexação de conteúdo não está habilitada para a caixa de correio de destino.  <br/> |
|ErrorCorruptData  <br/> |Este erro ocorre quando os dados estão corrompidos e não podem ser processados.  <br/> |
|ErrorCreateItemAccessDenied  <br/> |Este erro ocorre quando o chamador não tem permissão para criar o item.  <br/> |
|ErrorCreateManagedFolderPartialCompletion  <br/> |Este erro ocorre quando um ou mais das pastas gerenciadas que foram especificadas na solicitação de operação CreateManagedFolder falhou ao ser criado. Procure cada pasta determinar as pastas que foram criadas e as pastas que não existem.  <br/> |
|ErrorCreateSubfolderAccessDenied  <br/> |Este erro ocorre quando a conta de chamada não tem as permissões necessárias para criar a subpasta.  <br/> |
|ErrorCrossMailboxMoveCopy  <br/> |Este erro ocorre quando é feita uma tentativa de mover um item ou pasta de uma caixa de correio para outro. Se a caixa de correio de origem e a caixa de correio de destino forem diferentes, você receberá esse erro.  <br/> |
|ErrorCrossSiteRequest  <br/> |Esse erro indica que a solicitação não é permitida porque o servidor de acesso para cliente que deve atender a solicitação está em um site diferente.  <br/> |
|ErrorDataSizeLimitExceeded  <br/> |Esse erro pode ocorrer nos seguintes cenários:<br/>  <br/>-Uma tentativa de acessar ou gravar uma propriedade em um item e o valor da propriedade é muito grande.<br/>-O base64 codificado em MIME comprimento na solicitação XML excede o limite de conteúdo.<br/>-O tamanho do corpo de um corpo do item existente excede o limite.<br/>-Consumidor tenta definir um corpo de texto HTML ou cujo comprimento (ou comprimento combinado no caso de append) excede o limite. |
|ErrorDataSourceOperation  <br/> |Este erro ocorre quando o provedor de dados subjacente falha concluir a operação.  <br/> |
|ErrorDelegateAlreadyExists  <br/> |Este erro ocorre em uma operação de **AddDelegate** quando o usuário especificado já existe na lista de representantes.  <br/> |
|ErrorDelegateCannotAddOwner  <br/> |Este erro ocorre em uma operação de **AddDelegate** quando o usuário especificado a ser adicionado é o proprietário da caixa de correio.  <br/> |
|ErrorDelegateMissingConfiguration  <br/> |Este erro ocorre em uma operação **GetDelegate** quando ou não há nenhuma informação de representante na mensagem FreeBusy local ou nenhum delegado público do Active Directory (nenhum "representante público" ou nenhuma entrada de "Enviar em nome" no AD DS).  <br/> |
|ErrorDelegateNoUser  <br/> |Este erro ocorre quando um usuário especificado não pode ser mapeado para um usuário no AD DS.  <br/> |
|ErrorDelegateValidationFailed  <br/> |Este erro ocorre na operação **AddDelegate** quando um usuário delegado adicionado não é válido.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Este erro ocorre quando é feita uma tentativa para excluir uma pasta distinta.  <br/> |
|ErrorDeleteItemsFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorDeleteUnifiedMessagingPromptFailed  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorDistinguishedUserNotSupported  <br/> |Esse erro indica que uma ID de usuário distinto não é válida para a operação. **DistinguishedUserType** não deve estar presente na solicitação.  <br/> |
|ErrorDistributionListMemberNotExist  <br/> |Esse erro indica que um membro de lista de distribuição de solicitação não existir na lista de distribuição.  <br/> |
|ErrorDuplicateInputFolderNames  <br/> |Este erro ocorre quando os nomes de pasta duplicados são especificados no elemento [nomes de pastas](foldernames.md) da solicitação de operação **CreateManagedFolder** .  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Esse erro indica que não existem duplicados cabeçalhos SOAP.  <br/> |
|ErrorDuplicateUserIdsSpecified  <br/> |Esse erro indica que uma ID de usuário duplicado foi encontrado em um conjunto de permissões, há SIDs ou destinatários duplicados ou padrão ou anônimo são definidos em mais de uma vez.  <br/> |
|ErrorEmailAddressMismatch  <br/> |Este erro ocorre quando uma solicitação tenta criar/atualizar os parâmetros de pesquisa de uma pasta de pesquisa. Por exemplo, isso pode ocorrer quando uma pasta de pesquisa é criada na caixa de correio, mas a pasta de pesquisa seja direcionada para procurar na outra caixa de correio.  <br/> |
|ErrorEventNotFound  <br/> |Este erro ocorre quando o evento que é associado a uma marca d'água é excluído antes que o evento seja retornado. Quando esse erro é retornado, a inscrição também é excluída.  <br/> |
|ErrorExceededConnectionCount  <br/> |Este erro - indica que há mais simultânea solicitações com base no servidor que o permitido pela política do usuário.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |Esse erro indica que um usuário da contagem de assinatura máximo foi excedida de política de limitação.  <br/> |
|ErrorExceededFindCountLimit  <br/> |Esse erro indica que uma chamada de operação de pesquisa excedeu o número total de itens que podem ser retornadas.  <br/> |
|ErrorExpiredSubscription  <br/> |Este erro ocorre se a [operação GetEvents](getevents-operation.md) for chamado como uma assinatura está sendo excluída porque ele expirou.  <br/> |
|ErrorExtensionNotFound  <br/> |Indica que a extensão não foi localizada.  <br/> |
|ErrorFolderCorrupt  <br/> |Este erro ocorre quando a pasta está corrompida e não pode ser salvos.  <br/> |
|ErrorFolderExists  <br/> |Este erro ocorre quando é feita uma tentativa para criar uma pasta que tem o mesmo nome como outra pasta no mesmo pai. Nomes de pasta duplicados não são permitidos.  <br/> |
|ErrorFolderNotFound  <br/> |Esse erro indica que o ID da pasta que foi especificado não corresponde a uma pasta válida ou que o representante não tem permissão para acessar a pasta.  <br/> |
|ErrorFolderPropertRequestFailed  <br/> |Esse erro indica que a propriedade solicitada não pôde ser recuperada. Isso não indica que a propriedade não existe, mas que a propriedade foi corrompida de alguma maneira para que a recuperação falha.  <br/> |
|ErrorFolderSave  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSaveFailed  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a um estado inválido.  <br/> |
|ErrorFolderSavePropertyError  <br/> |Esse erro indica que a pasta não pôde ser criada ou atualizada devido a valores de propriedade inválido. O código de resposta lista as propriedades que causou o problema.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Esse erro indica que a contagem de membro do grupo máximo foi atingida para obtenção de informações de disponibilidade para obter uma lista de distribuição.  <br/> |
|ErrorFreeBusyGenerationFailed  <br/> |Esse erro é retornado quando informações de disponibilidade não podem ser recuperadas por causa de uma falha intermediário.  <br/> |
|ErrorGetServerSecurityDescriptorFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorImContactLimitReached  <br/> |Esse erro é retornado quando nova contatos (IM) de mensagens instantâneas não podem ser adicionadas, porque foi atingido o número máximo de contatos. Esse erro foi introduzido no Exchange Server 2013.  <br/> |
|ErrorImGroupDisplayNameAlreadyExists  <br/> |Esse erro é retornado quando é feita uma tentativa para adicionar um nome de exibição do grupo quando um grupo existente já tem o mesmo nome de exibição. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImGroupLimitReached  <br/> |Esse erro é retornado quando novos grupos de mensagens Instantâneas não podem ser adicionados porque o número máximo de grupos foi atingido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorImpersonateUserDenied  <br/> |O erro será retornado no caso de autorização de servidor-para-servidor para representação do Exchange quando o chamador não tem os direitos adequados para representar o usuário específico em questão. Esse erro é mapeado para o ms-Exch-EPI-May-Impersonate estendido à direita do Active Directory.  <br/> |
|ErrorImpersonationDenied  <br/> |Esse erro é retornado na autorização de servidor-para-servidor para a representação do Exchange quando o chamador não tem os direitos adequados para representar através do servidor de acesso para cliente que eles estão fazendo a solicitação em relação. Mapeia para o ms-Exch-EPI-Impersonation estendido à direita do Active Directory.  <br/> |
|ErrorImpersonationFailed  <br/> |Esse erro indica que houve um erro inesperado quando foi feita uma tentativa de executar a autenticação de servidor-para-servidor. Este código de resposta normalmente um dos que indica a conta de serviço que está executando o pool de aplicativos está configurado incorretamente, o Exchange Web Services que os serviços Web do Exchange não é possível falar com o diretório ou se uma relação de confiança entre florestas não está corretamente configurado.  <br/> |
|ErrorIncorrectSchemaVersion  <br/> |Esse erro indica que a solicitação era válida para a versão atual do Exchange Server, mas era inválida para a versão do servidor de solicitação que foi especificada.  <br/> |
|ErrorIncorrectUpdatePropertyCount  <br/> |Esse erro indica que a descrição de cada alteração nos elementos [UpdateItem](updateitem.md) ou [UpdateFolder](updatefolder.md) deve listar apenas uma propriedade a ser atualizada.  <br/> |
|ErrorIndividualMailboxLimitReached  <br/> |Este erro ocorre quando a solicitação contém participantes em excesso para resolver. Por padrão, o número máximo de participantes para resolver é 100.  <br/> |
|ErrorInsufficientResources  <br/> |Este erro ocorre quando o servidor de caixa de correio está sobrecarregado. Tente a solicitação novamente mais tarde.  <br/> |
|ErrorInternalServerError  <br/> |Esse erro indica que o Exchange Web Services encontrou um erro dizendo que ele não pode se recuperar e não existir um código de resposta mais específico que está associado com o erro que ocorreu.  <br/> |
|ErrorInternalServerTransientError  <br/> |Esse erro indica que ocorreu um erro interno do servidor e que você deve tentar sua solicitação novamente mais tarde.  <br/> |
|ErrorInvalidAccessLevel  <br/> |Esse erro indica que o nível de acesso que o chamador tem sobre os dados de disponibilidade é inválido.  <br/> |
|ErrorInvalidArgument  <br/> |Esse erro indica um erro causado por todos os argumentos inválidos passados para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).<br/><br/> Esse erro é retornado nos seguintes cenários: <br/><br/>-O usuário especificado no _enviando-como_ parâmetro não existir no diretório. <br/>-O usuário especificado no _enviando-como_ parâmetro não é exclusivo no diretório. <br/>-Os _enviando-como_ endereço está vazio.<br/>-Os _enviando-como_ endereço não é um endereço de email válido.  <br/> |
|ErrorInvalidAttachmentId  <br/> |Esse erro é retornado pela [operação GetAttachment](getattachment-operation.md) ou a [operação DeleteAttachment](deleteattachment-operation.md) quando um anexo que corresponde à ID especificada não for encontrado.  <br/> |
|ErrorInvalidAttachmentSubfilter  <br/> |Este erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexo complexos. Serviços Web do Exchange apenas suporta simples contém filtros contra a tabela de anexos. Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexo (um subfiltro) mais complexa, serviços Web do Exchange não pode renderizar o XML para esse filtro e retorna este código de resposta. <br/><br/>Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitam o elemento [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAttachmentSubfilterTextFilter  <br/> |Este erro ocorre quando você tenta vincular a uma pasta de pesquisa existente usando uma restrição de tabela de anexo complexos. Serviços Web do Exchange apenas suporta simples contém filtros contra a tabela de anexos. <br/><br/>Se você tentar vincular a uma pasta de pesquisa existente que tenha uma restrição de tabela de anexo mais complexa, serviços Web do Exchange não pode renderizar o XML para esse filtro. Nesse caso, o subfiltro anexo contiver um filtro de texto, mas ele não está olhando o nome de exibição do anexo.<br/><br/> Observe que você ainda pode chamar a operação GetFolder na pasta, mas não solicitam o elemento [SearchParameters](searchparameters.md) .  <br/> |
|ErrorInvalidAuthorizationContext  <br/> | Esse erro indica que o procedimento de autorização para o solicitante falhou.  <br/> |
|ErrorInvalidChangeKey  <br/> |Este erro ocorre quando um consumidor passa em uma pasta ou um identificador de item com uma chave de alteração que não pode ser analisada. Por exemplo, isso poderia ser conteúdo base64 inválida ou uma sequência vazia.  <br/> |
|ErrorInvalidClientSecurityContext  <br/> |Esse erro indica que houve um erro interno quando foi feita uma tentativa para resolver a identidade do chamador.  <br/> |
|ErrorInvalidCompleteDate  <br/> |Esse erro é retornado quando é feita uma tentativa para definir o valor do elemento [CompleteDate](completedate.md) de uma tarefa para um horário no futuro. Quando ele é convertido em hora local do servidor acesso para cliente, o [CompleteDate](completedate.md) de uma tarefa não pode ser definida como um valor que é posterior a hora local no servidor de acesso para cliente.  <br/> |
|ErrorInvalidContactEmailAddress  <br/> |Esse erro indica que um endereço de email inválido foi fornecido para um contato.  <br/> |
|ErrorInvalidContactEmailIndex  <br/> |Esse erro indica que um valor de índice do email inválido foi fornecido para uma entrada de email.  <br/> |
|ErrorInvalidCrossForestCredentials  <br/> |Este erro ocorre quando as credenciais que são usadas para proxy uma solicitação para uma floresta de serviço de diretório diferente Falha na autenticação.  <br/> |
|ErrorInvalidDelegatePermission  <br/> |Esse erro indica que as permissões da pasta especificada são inválidas.  <br/> |
|ErrorInvalidDelegateUserId  <br/> |Esse erro indica que a ID de usuário delegado especificado é inválida.  <br/> |
|ErrorInvalidExchangeImpersonationHeaderData  <br/> |Este erro ocorre durante a representação do Exchange quando um chamador não especifica um UPN, um endereço de email ou um SID de usuário. Isso também ocorrerá se o chamador Especifica uma ou mais daqueles e os valores são vazios.  <br/> |
|ErrorInvalidExcludesRestriction  <br/> |Este erro ocorre quando o bitmask que foi passado para uma restrição de elemento [exclusões](excludes.md) não pode ser analisado.  <br/> |
|ErrorInvalidExpressionTypeForSubFilter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidExtendedProperty  <br/> | Este erro ocorre quando os seguintes eventos ocorrem: <br/> <br/>-O chamador tenta usar uma propriedade estendida que não é suportada pelos serviços Web do Exchange.  <br/>-O chamador passa uma combinação de valores de atributo para uma propriedade estendida inválida. Isso também ocorre se nenhum atributos são passados. Somente determinadas combinações são permitidas.  <br/> |
|ErrorInvalidExtendedPropertyValue  <br/> |Este erro ocorre quando a seção de valor de uma propriedade estendida não coincide com o tipo da propriedade. <br/><br/>Por exemplo, a definição de uma propriedade estendida que tem PropertyType = "Cadeia de caracteres" para uma matriz de números inteiros resultará neste erro. Qualquer representação de cadeia de caracteres que não é conversível no tipo que é especificado para a propriedade estendida fornecerá a esse erro.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Esse erro indica que o remetente do convite de compartilhamento não criou os metadados de convite de compartilhamento.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Esse erro indica que uma mensagem de compartilhamento não foi destinada para o chamador.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Esse erro indica que objetos de Federação da organização do solicitador não estão configurados corretamente.  <br/> |
|ErrorInvalidFolderId  <br/> |Este erro ocorre quando o ID da pasta está corrompido.  <br/> |
|ErrorInvalidFolderTypeForOperation  <br/> |Esse erro indica que o tipo da pasta especificada é inválido para a operação atual. Por exemplo, é possível criar uma pasta de pesquisa em uma pasta pública.  <br/> |
|ErrorInvalidFractionalPagingParameters  <br/> | Este erro ocorre em paginação fracional quando o usuário tiver especificado um destes procedimentos: <br/> <br/>-Um numerador que for maior que o denominador  <br/>-Um numerador que é menor do que zero  <br/>-Um denominador que seja menor ou igual a zero  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Esse erro indica que os elementos de [tipo de dados](datatype.md) e ShareFolderId são ambos presentes em uma solicitação.  <br/> |
|ErrorInvalidFreeBusyViewType  <br/> |Este erro ocorre quando a [operação GetUserAvailability](getuseravailability-operation.md) é chamado com um [FreeBusyViewType](freebusyviewtype.md) None.  <br/> |
|ErrorInvalidId  <br/> |Esse erro indica que a chave de ID e/ou alteração é mal formada.  <br/> |
|ErrorInvalidIdEmpty  <br/> |Este erro ocorre quando o chamador Especifica um atributo de **identificação** que está vazio.  <br/> |
|ErrorInvalidLikeRequest  <br/> |Este erro ocorre quando o item não pode ser curtido. Versões do Exchange, começando com o número de compilação 15.00.0913.09 incluem esse valor.  <br/> |
|ErrorInvalidIdMalformed  <br/> |Este erro ocorre quando o chamador Especifica um atributo de **identificação** que está mal formado.  <br/> |
|ErrorInvalidIdMalformedEwsLegacyIdFormat  <br/> |Esse erro indica que uma ID de pasta ou item que está usando o formato do Exchange 2007 foi especificado para uma solicitação com uma versão do Exchange 2007 SP1 ou posterior. Você não pode usar as IDs de 2007 do Exchange no Exchange 2007 SP1 ou posteriores solicitações. Você precisa usar a [operação ConvertId](convertid-operation.md) para convertê-los primeiro.  <br/> |
|ErrorInvalidIdMonikerTooLong  <br/> |Este erro ocorre quando o chamador Especifica um atributo de **Id** é muito longo.  <br/> |
|ErrorInvalidIdNotAnItemAttachmentId  <br/> |Esse erro é retornado sempre que uma ID que não é um anexo do item que ID é passado para um método de serviço Web que espera um ID de anexo.  <br/> |
|ErrorInvalidIdReturnedByResolveNames  <br/> |Este erro ocorre quando um contato na sua caixa de correio está corrompido.  <br/> |
|ErrorInvalidIdStoreObjectIdTooLong  <br/> |Este erro ocorre quando o chamador Especifica um atributo de **Id** é muito longo.  <br/> |
|ErrorInvalidIdTooManyAttachmentLevels  <br/> |Esse erro é retornado quando a hierarquia de anexo em um item excede o máximo de 255 níveis de profundidade.  <br/> |
|ErrorInvalidIdXml  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidImContactId  <br/> |Esse erro é retornado quando o identificador de contato de mensagens Instantâneas especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImDistributionGroupSmtpAddress  <br/> |Esse erro é retornado quando o grupo de distribuição da IM especificado SMTP endereço identificador não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidImGroupId  <br/> |Esse erro é retornado quando o identificador do grupo de mensagens Instantâneas especificado não representa um identificador válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidIndexedPagingParameters  <br/> |Este erro ocorre se o deslocamento de paginação indexado for negativo.  <br/> |
|ErrorInvalidInternetHeaderChildNodes  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidItemForOperationArchiveItem  <br/> |Indica que o item foi inválido para uma operação de **ArchiveItem** .  <br/> |
|ErrorInvalidItemForOperationAcceptItem  <br/> |Esse erro ocorre quando é feita uma tentativa para usar um objeto de resposta de AcceptItem para um tipo de item que não seja uma solicitação de reunião ou um item de calendário ou quando é feita uma tentativa para aceitar uma ocorrência de item de calendário que está na pasta Itens excluídos.  <br/> |
|ErrorInvalidItemForOperationCancelItem  <br/> |Este erro ocorre quando é feita uma tentativa para usar um objeto de resposta CancelItem em um tipo de item que não seja um item do calendário.  <br/> |
|ErrorInvalidItemForOperationCreateItemAttachment  <br/> | Esse erro é retornado quando é feita uma tentativa para criar um anexo de item de um tipo não suportado.  <br/><br/>  Tipos de item com suporte para anexos de item incluem os seguintes objetos:  <br/><br/>- [Item](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Contato](contact.md) <br/> <br/> Por exemplo, se você tentar criar um anexo [MeetingMessage](meetingmessage.md) , você encontrará este código de resposta.  <br/> |
|ErrorInvalidItemForOperationCreateItem  <br/> | Esse erro será retornado de uma [operação de CreateItem](createitem-operation.md) , se a solicitação contém um tipo de item sem suporte. <br/><br/>Itens com suporte incluem os seguintes objetos:<br/>  <br/>- [Item](item.md) <br/>- [Mensagem](message-ex15websvcsotherref.md) <br/>- [CalendarItem](calendaritem.md) <br/>- [Tarefa](task.md) <br/>- [Contato](contact.md) <br/><br/>  Certos tipos são criados como um efeito de fazer algo diferente. Por exemplo, mensagens de reunião, são criados quando você envia um item de calendário aos participantes; eles não são criados explicitamente.  <br/> |
|ErrorInvalidItemForOperationDeclineItem  <br/> |Esse erro ocorre quando é feita uma tentativa para usar um objeto de resposta de DeclineItem para um tipo de item que não seja uma solicitação de reunião ou um item de calendário ou quando é feita uma tentativa para recusar uma ocorrência de item de calendário que está na pasta Itens excluídos.  <br/> |
|ErrorInvalidItemForOperationExpandDL  <br/> |Esse erro indica que a [operação ExpandDL](expanddl-operation.md) é válida apenas para listas de distribuição privada.  <br/> |
|ErrorInvalidItemForOperationRemoveItem  <br/> |Esse erro é retornado de um objeto de resposta RemoveItem se a solicitação especifica um item que não é uma reunião de item de cancelamento.  <br/> |
|ErrorInvalidItemForOperationSendItem  <br/> |Esse erro será retornado de uma [operação SendItem](senditem-operation.md) , se a solicitação especifica um item que não é um item de mensagem.  <br/> |
|ErrorInvalidItemForOperationTentative  <br/> |Esse erro ocorre quando é feita uma tentativa para usar [TentativelyAcceptItem](tentativelyacceptitem.md) para um tipo de item que não seja uma solicitação de reunião ou um item de calendário ou quando é feita uma tentativa para aceitar provisoriamente uma ocorrência de item de calendário que está na pasta Itens excluídos.  <br/> |
|ErrorInvalidLogonType  <br/> |Esse erro é apenas para uso interno. Esse erro não será retornado.  <br/> |
|ErrorInvalidMailbox  <br/> |Esse erro indica que a [operação CreateItem](createitem-operation.md) ou a [operação UpdateItem](updateitem-operation.md) falhou ao criar ou atualizar uma lista de distribuição pessoal.  <br/> |
|ErrorInvalidManagedFolderProperty  <br/> |Este erro ocorre quando a estrutura de pasta gerenciada está corrompida e não pode ser renderizada.  <br/> |
|ErrorInvalidManagedFolderQuota  <br/> |Este erro ocorre quando a cota que está definida na pasta gerenciada é menor do que zero, o que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidManagedFolderSize  <br/> |Este erro ocorre quando o tamanho definido na pasta gerenciada for menor do que zero, o que indica uma pasta gerenciada corrompida.  <br/> |
|ErrorInvalidMergedFreeBusyInterval  <br/> |Este erro ocorre quando o mesclado livre/ocupado interno valor fornecido é inválido. O valor mínimo de padrão é 5 minutos. O valor máximo padrão é 1440 minutos.  <br/> |
|ErrorInvalidNameForNameResolution  <br/> |Este erro ocorre quando o nome é inválido para a [operação ResolveNames](resolvenames-operation.md). Por exemplo, uma sequência de comprimento zero, um espaço simples, uma vírgula e um traço são todos os nomes inválidos.  <br/> |
|ErrorInvalidNetworkServiceContext  <br/> |Esse erro indica um erro na conta do serviço de rede no servidor de acesso para cliente.  <br/> |
|ErrorInvalidOofParameter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidOperation  <br/> | Este é um erro geral que é usado quando a operação solicitada é inválida. <br/><br/>Por exemplo, você não pode fazer o seguinte: <br/> <br/>-Execute uma passagem "Detalhada" usando a [operação FindFolder](findfolder-operation.md) em uma pasta pública.  <br/>-Mover ou copiar a raiz da pasta pública.  <br/>-Exclua um item associado usando qualquer modo, exceto excluir "Rígido".  <br/>-Mover ou copiar um item associado.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Esse erro indica que um chamador solicitou informações de disponibilidade para um usuário de outra organização, mas a relação organizacional não tem livre/ocupado habilitado.  <br/> |
|ErrorInvalidPagingMaxRows  <br/> |Este erro ocorre quando um consumidor passa em um zero ou um valor negativo para o máximo de linhas a ser retornado.  <br/> |
|ErrorInvalidParentFolder  <br/> |Este erro ocorre quando um consumidor passa em uma pasta pai inválido para uma operação. Por exemplo, esse erro será retornado se você tentar criar uma pasta dentro de uma pasta de pesquisa.  <br/> |
|ErrorInvalidPercentCompleteValue  <br/> |Esse erro é retornado quando é feita uma tentativa para definir uma porcentagem de conclusão de tarefa como um valor inválido. O valor deve estar entre 0 e 100 (inclusive).  <br/> |
|ErrorInvalidPermissionSettings  <br/> |Esse erro indica que o nível de permissão está inconsistente com as configurações de permissão.  <br/> |
|ErrorInvalidPhoneCallId  <br/> |Esse erro indica que o identificador do chamador não é válido.  <br/> |
|ErrorInvalidPhoneNumber  <br/> |Esse erro indica que o número de telefone não está correto ou não se ajusta as regras de plano de discagem.  <br/> |
|ErrorInvalidPropertyAppend  <br/> | Este erro ocorre quando a propriedade que você está tentando acrescentar ao não oferece suporte para anexar. <br/><br/>Estes são as únicas propriedades que suportam acrescentando: <br/> <br/>-Coleções destinatários (ToRecipients, CcRecipients, BccRecipients)  <br/>-Conjuntos de attendee (RequiredAttendees, OptionalAttendees, recursos)  <br/>-Corpo  <br/>-ReplyTo  <br/><br/>  Além disso, este erro ocorre quando um corpo da mensagem foi acrescentado, se o formato especificado na solicitação não coincide com o formato do item no repositório.  <br/> |
|ErrorInvalidPropertyDelete  <br/> |Este erro ocorre se a operação de exclusão for especificada em uma chamada de [operação de UpdateItem](updateitem-operation.md) ou [UpdateFolder](updatefolder-operation.md) para uma propriedade que não oferece suporte a operação de exclusão. Por exemplo, você não pode excluir o elemento [ItemId](itemid.md) do objeto de [Item](item.md) .  <br/> |
|ErrorInvalidPropertyForExists  <br/> |Este erro ocorre se o consumidor passa em uma das propriedades em um filtro [Exists](exists.md) sinalizador. Por exemplo, este erro ocorre se os sinalizadores [foi lido](isread.md) ou [IsFromMe](isfromme.md) forem especificados no elemento [Exists](exists.md) . A solicitação deverá usar o elemento [IsEqualTo](isequalto.md) para esses como são sinalizadores e, portanto, a parte de uma única propriedade.  <br/> |
|ErrorInvalidPropertyForOperation  <br/> |Este erro ocorre quando a propriedade que você está tentando manipular não oferece suporte a operação que está sendo realizada nele.  <br/> |
|ErrorInvalidPropertyRequest  <br/> | Este erro ocorre se uma propriedade que é especificada na solicitação não está disponível para o tipo de item. Por exemplo, esse erro será retornado se uma propriedade que está disponível somente em itens de calendário for solicitada em uma [operação de GetItem](getitem-operation.md) chamada de uma mensagem ou é atualizado em uma [operação UpdateItem](updateitem-operation.md) telefonar para uma mensagem. <br/> <br/>  Isso ocorre nas seguintes operações: <br/> <br/>- [Operação GetItem](getitem-operation.md) <br/>- [Operação GetFolder](getfolder-operation.md) <br/>- [Operação UpdateItem](updateitem-operation.md) <br/>- [Operação UpdateFolder](updatefolder-operation.md) <br/> |
|ErrorInvalidPropertySet  <br/> |Esse erro indica que a propriedade que você está tentando manipular não oferece suporte a operação que está sendo realizada nele. Por exemplo, esse erro será retornado se a propriedade que você está tentando definir é somente leitura.  <br/> |
|ErrorInvalidPropertyUpdateSentMessage  <br/> | Este erro ocorre durante uma [operação UpdateItem](updateitem-operation.md) quando um cliente tentar atualizar determinadas propriedades de uma mensagem que já foi enviada.<br/><br/> Por exemplo, as propriedades a seguir não podem ser atualizadas em uma mensagem enviada: <br/> <br/>- [IsReadReceiptRequested](isreadreceiptrequested.md) <br/>- [IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |
|ErrorInvalidProxySecurityContext  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidPullSubscriptionId  <br/> |Este erro ocorre se você chamar a [operação GetEvents](getevents-operation.md) ou a [operação de cancelamento da assinatura](unsubscribe-operation.md) usando uma ID de assinatura push. Para cancelar a assinatura de uma inscrição de envio, responder a uma solicitação de push com uma resposta de cancelamento da assinatura, ou desconectar o seu serviço da Web e aguarde as notificações por push do tempo limite.  <br/> |
|ErrorInvalidPushSubscriptionUrl  <br/> | Este erro será retornado pela [operação Subscribe](subscribe-operation.md) quando ele cria uma assinatura de "push" e indica que a URL que está incluída na solicitação é inválida.<br/><br/>As seguintes condições devem ser atendidas para serviços Web do Exchange aceitar a URL: <br/> <br/>-String comprimento \> 0 e \< 2083.  <br/>-Protocolo é http ou https.  <br/>-A URL pode ser analisada pela classe URI Microsoft .NET Framework.  <br/> |
|ErrorInvalidRecipients  <br/> |Esse erro indica que a coleção de destinatários na sua mensagem ou a coleção de participante em seu item de calendário é inválida. Por exemplo, esse erro será retornado quando é feita uma tentativa de enviar um item que não tiver destinatários.  <br/> |
|ErrorInvalidRecipientSubfilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que não pode representar a serviços Web do Exchange. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterComparison  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que não pode representar a serviços Web do Exchange. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterOrder  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que não pode representar a serviços Web do Exchange. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidRecipientSubfilterTextFilter  <br/> |Esse erro indica que a pasta de pesquisa tem um filtro de tabela de destinatários que não pode representar a serviços Web do Exchange. Para contornar esse erro, recupere a pasta sem solicitar os parâmetros de pesquisa.  <br/> |
|ErrorInvalidReferenceItem  <br/> | Esse erro é retornado da [operação CreateItem](createitem-operation.md) para encaminhar e responder objetos de resposta nos seguintes cenários:<br/>  <br/>-O identificador do item referenciado não é um descendente de uma **mensagem** ou **CalendarItem**, um [CalendarItem](calendaritem.md)ou uma [mensagem](message-ex15websvcsotherref.md).  <br/>-O identificador do item de referência é para um **CalendarItem** e o organizador está tentando responder ou responder para si próprio.  <br/>-A mensagem é um rascunho e responder ou responder está selecionada.  <br/>-O item de referência, para [SuppressReadReceipt](suppressreadreceipt.md), não é um descendente de uma **mensagem**ou de uma **mensagem** .  <br/> |
|ErrorInvalidRequest  <br/> |Este erro ocorre quando a solicitação SOAP possui um cabeçalho de ação SOAP, mas nada no corpo SOAP. Observe que o cabeçalho de ação SOAP não é necessário, como serviços Web do Exchange pode determinar o método a ser chamado do nome do local do elemento raiz no corpo SOAP.  <br/> |
|ErrorInvalidRestriction  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidRetentionTagTypeMismatch  <br/> |Esse erro é retornado quando a marca de retenção especificado tem uma ação incorreta associada a ela. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInvisible  <br/> |Esse erro é retornado quando é feita uma tentativa para definir uma marca inexistente ou invisível em uma propriedade **PolicyTag** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagInheritance  <br/> |Esse erro é retornado quando é feita uma tentativa para definir uma marca implícita na propriedade **PolicyTag** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagIdGuid  <br/> |Indica que a marca de retenção GUID era inválida.  <br/> |
|ErrorInvalidRoutingType  <br/> |Este erro ocorre se o tipo de roteamento que é passado para um elemento [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) é inválido. Normalmente, o tipo de roteamento é definido para SMTP Simple Mail Transfer Protocol ().  <br/> |
|ErrorInvalidScheduledOofDuration  <br/> |Este erro ocorre se a hora de término do período especificado não for maior que a hora de início, ou se a hora de término não ocorrem no futuro.  <br/> |
|ErrorInvalidSchemaVersionForMailboxVersion  <br/> |Esse erro indica que uma solicitação de proxy que foi enviada para outro servidor não é capaz de atender à solicitação devido a uma incompatibilidade de controle de versão.  <br/> |
|ErrorInvalidSecurityDescriptor  <br/> |Esse erro indica que o descritor de segurança do Exchange na pasta de calendário no repositório está corrompido.  <br/> |
|ErrorInvalidSendItemSaveSettings  <br/> |Este erro ocorre durante uma tentativa de enviar um item onde o [SavedItemFolderId](saveditemfolderid.md) for especificado na solicitação, mas a propriedade **SaveItemToFolder** estiver definida como **false**.  <br/> |
|ErrorInvalidSerializedAccessToken  <br/> |Esse erro indica que o token passado no cabeçalho está incorreto, não se refere a uma conta válida no diretório ou está faltando o grupo primário **ConnectingSID**.  <br/> |
|ErrorInvalidSharingData  <br/> |Esse erro indica que os metadados de compartilhamento não são válido. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorInvalidSid  <br/> |Este erro ocorre quando uma SID é transmitido em uma solicitação de inválida.  <br/> |
|ErrorInvalidSIPUri  <br/> |Esse erro indica que o nome do SIP, plano de discagem ou o número de telefone são inválidos URIs do SIP.  <br/> |
|ErrorInvalidServerVersion  <br/> |Esse erro indica que uma versão do servidor de solicitação inválido foi especificada na solicitação.  <br/> |
|ErrorInvalidSmtpAddress  <br/> |Este erro ocorre quando o endereço SMTP não pode ser analisado.  <br/> |
|ErrorInvalidSubfilterType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotAttendeeType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubfilterTypeNotRecipientType  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidSubscription  <br/> |Esse erro indica que a assinatura não é mais válida. Isso poderia ser porque o servidor de acesso para cliente está reiniciando ou a assinatura expirou.  <br/> |
|ErrorInvalidSubscriptionRequest  <br/> |Esse erro indica que a solicitação subscribe incluídos vários IDs de pasta pública. Uma assinatura pode incluir várias pastas de mesma caixa de correio ou um ID de pasta pública.  <br/> |
|ErrorInvalidSyncStateData  <br/> |Esse erro será retornado por [SyncFolderItems](syncfolderitems.md) ou [SyncFolderHierarchy](syncfolderhierarchy.md) , se os dados de [estado de sincronização](syncstate-ex15websvcsotherref.md) que são passados são inválidos. Para corrigir esse erro, você deve sincronizar novamente sem o estado de sincronização. Certifique-se de que se você está mantendo sync estado BLOBs, você não é truncar o BLOB acidentalmente.  <br/> |
|ErrorInvalidTimeInterval  <br/> |Esse erro indica que o intervalo de tempo especificado é inválido. A hora de início deve ser maior ou igual à hora de término.  <br/> |
|ErrorInvalidUserInfo  <br/> |Esse erro indica que um internamente inconsistente [UserId](userid.md) foi especificado para uma operação de permissões. Por exemplo, se uma ID de usuário distinto for especificado (padrão ou anônimo), esse erro será retornado se você tentar também especificar uma SID ou o endereço SMTP principal ou o nome de exibição para este usuário.  <br/> |
|ErrorInvalidUserOofSettings  <br/> |Esse erro indica que as configurações de ausência temporária do usuário são inválidas devido a uma resposta interna ou externa ausente.  <br/> |
|ErrorInvalidUserPrincipalName  <br/> |Este erro ocorre durante a representação do Exchange. O chamador passadas em um UPN inválido no cabeçalho SOAP que não estava acessível no diretório.  <br/> |
|ErrorInvalidUserSid  <br/> |Este erro ocorre quando uma SID é transmitido em uma solicitação de inválida.  <br/> |
|ErrorInvalidUserSidMissingUPN  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorInvalidValueForProperty  <br/> |Esse erro indica que o valor de comparação na restrição é inválido para a propriedade que você está comparando contra.<br/><br/> Por exemplo, o valor de comparação da [DateTimeCreated](datetimecreated.md) > **true** retornaria este código de resposta. <br/><br/>Este código de resposta também será retornado se você especificar uma propriedade de enumeração na comparação, mas o valor que você está comparando contra não é um valor válido para essa enumeração.  <br/> |
|ErrorInvalidWatermark  <br/> |Esse erro é causado por uma marca d'água inválida.  <br/> |
|ErrorIPGatewayNotFound  <br/> |Esse erro indica que um gateway VoIP válido não está disponível.  <br/> |
|ErrorIrresolvableConflict  <br/> |Esse erro indica que a resolução de conflito não pôde resolver as alterações para as propriedades. Os itens no repositório de podem ter sido alterados e devem ser atualizados. Recuperar a chave de alteração de atualização e tente novamente.  <br/> |
|ErrorItemCorrupt  <br/> |Esse erro indica que o estado do objeto está corrompido e não pode ser recuperado. Quando estiver recuperando um item, apenas determinados elementos será nesse estado, como o [corpo](body.md) e [MimeContent](mimecontent.md). Omitir esses elementos e repita a operação.  <br/> |
|ErrorItemNotFound  <br/> |Este erro ocorre quando o item não foi encontrado ou você não tem permissão para acessar o item.  <br/> |
|ErrorItemPropertyRequestFailed  <br/> |Este erro ocorre se uma solicitação de propriedade em um item falhar. A propriedade pode existir, mas não pôde ser recuperado.  <br/> |
|ErrorItemSave  <br/> |Este erro ocorre quando há falhas tentativas de salvar o item ou a pasta.  <br/> |
|ErrorItemSavePropertyError  <br/> |Este erro ocorre quando tenta salvar o item ou pasta falha devido a valores de propriedade inválido. O código de resposta inclui o caminho das propriedades inválidos.  <br/> |
|ErrorLegacyMailboxFreeBusyViewTypeNotMerged  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorLocalServerObjectNotFound  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorLogonAsNetworkServiceFailed  <br/> |Esse erro indica que o serviço de disponibilidade não pôde fazer logon como o serviço de rede para solicitações de proxy para os sites apropriados ou florestas. Geralmente, essa resposta indica um erro de configuração.  <br/> |
|ErrorMailboxConfiguration  <br/> |Esse erro indica que as informações de caixa de correio no AD DS estão configuradas incorretamente.  <br/> |
|ErrorMailboxDataArrayEmpty  <br/> |Esse erro indica que o elemento [MailboxDataArray](mailboxdataarray.md) na solicitação está vazio. Você deve fornecer pelo menos um identificador de caixa de correio.  <br/> |
|ErrorMailboxDataArrayTooBig  <br/> |Este erro ocorre quando mais de 100 entradas são fornecidas em um elemento [MailboxDataArray](mailboxdataarray.md) ..  <br/> |
|ErrorMailboxFailover  <br/> |Esse erro indica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorMailboxHoldNotFound  <br/> |Indica que a retenção de caixa de correio não foi localizada.  <br/> |
|ErrorMailboxLogonFailed  <br/> |Este erro ocorre quando a conexão à caixa de correio para obter as informações de modo de exibição de calendário falhou.  <br/> |
|ErrorMailboxMoveInProgress  <br/> | Esse erro indica que a caixa de correio está sendo movida para um repositório de caixa de correio diferente ou um servidor. Esse erro também pode indicar que a caixa de correio está em outro banco de dados de caixa de correio ou servidor.  <br/> |
|ErrorMailboxStoreUnavailable  <br/> | Esse erro indica que uma das condições ocorreram o erro a seguir:  <br/><br/>-O armazenamento de caixa de correio está corrompido.  <br/>-O repositório de caixa de correio está sendo parado.  <br/>-O repositório de caixa de correio está offline.  <br/>-Um erro de rede quando foi feita uma tentativa para acessar o repositório de caixa de correio.  <br/>-O repositório de caixa de correio está sobrecarregado e não pode aceitar qualquer mais conexões.  <br/>-O repositório de caixa de correio foi pausado.  <br/> |
|ErrorMailRecipientNotFound  <br/> |Este erro ocorre se as informações do elemento [MailboxData](mailboxdata.md) não podem ser mapeadas para uma conta válida de caixa de correio.  <br/> |
|ErrorMailTipsDisabled  <br/> |Esse erro indica que as dicas de email estão desabilitadas.  <br/> |
|ErrorManagedFolderAlreadyExists  <br/> |Este erro ocorre se a pasta gerenciada que você está tentando criar já existir em uma caixa de correio.  <br/> |
|ErrorManagedFolderNotFound  <br/> |Este erro ocorre quando o nome da pasta que foi especificado na solicitação não é mapeado para uma definição de pasta gerenciada no AD DS. Você só pode criar instâncias de pastas gerenciadas para pastas que são definidas no AD DS. Verifique o nome e tente novamente.  <br/> |
|ErrorManagedFoldersRootFailure  <br/> |Esse erro indica que a raiz de pastas gerenciadas foi excluída da caixa de correio ou que existe uma pasta na mesma pasta pai que tem o nome da autoridade raiz de pasta gerenciada. Isso também ocorrerá se a tentativa de criar a raiz gerenciado pasta falhar.  <br/> |
|ErrorMeetingSuggestionGenerationFailed  <br/> |Esse erro indica que o mecanismo de sugestões encontrou um problema quando ele estava tentando gerar as sugestões.  <br/> |
|ErrorMessageDispositionRequired  <br/> | Este erro ocorre se o atributo **MessageDisposition** não estiver definido.<br/><br/> Este atributo é necessário para o seguinte: <br/> <br/>-A [operação CreateItem](createitem-operation.md) e a [operação UpdateItem](updateitem-operation.md) quando o item que está sendo criado ou atualizado é uma [mensagem](message-ex15websvcsotherref.md).  <br/>- Objetos de resposta [CancelCalendarItem](cancelcalendaritem.md), [AcceptItem](acceptitem.md), [DeclineItem](declineitem.md)ou [TentativelyAcceptItem](tentativelyacceptitem.md) .  <br/> |
|ErrorMessageSizeExceeded  <br/> |Esse erro indica que a mensagem que você está tentando enviar excede os limites permitidos.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Esse erro indica que o domínio indicado não foi encontrado.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Esse erro indica que o serviço de controle de mensagens não podem controlar a mensagem.  <br/> |
| ErrorMessageTrackingTransientError  <br/> |Esse erro indica que o serviço de controle de mensagens está inoperante ou ocupado. Este código de erro indica um erro transitório. Clientes podem tentar para se conectar ao servidor quando esse erro é recebido.  <br/> |
|ErrorMimeContentConversionFailed  <br/> |Este erro ocorre quando o conteúdo MIME não é válido para uma [operação CreateItem](createitem-operation.md)iCal. Para uma [operação de GetItem](getitem-operation.md), esta resposta indica que o conteúdo MIME não pôde ser gerado.  <br/> |
|ErrorMimeContentInvalid  <br/> |Este erro ocorre quando o conteúdo MIME é inválido.  <br/> |
|ErrorMimeContentInvalidBase64String  <br/> |Este erro ocorre quando o conteúdo MIME na solicitação é não uma base 64 cadeia de caracteres válida.  <br/> |
|ErrorMissingArgument  <br/> |Esse erro indica que um argumento necessário estava faltando da solicitação. O texto da mensagem de resposta indica qual argumento para verificar.  <br/> |
|ErrorMissingEmailAddress  <br/> |Esse erro indica que você especificou um ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um elemento de subsites de [caixa de correio](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md).  <br/> |
|ErrorMissingEmailAddressForManagedFolder  <br/> |Esse erro indica que você especificou um ID de pasta distinta na solicitação, mas a conta que fez a solicitação não tem uma caixa de correio no sistema. Nesse caso, você deve fornecer um elemento de subsites de [caixa de correio](mailbox.md) em [DistinguishedFolderId](distinguishedfolderid.md). Esta resposta é retornada da [operação CreateManagedFolder](createmanagedfolder-operation.md).  <br/> |
|ErrorMissingInformationEmailAddress  <br/> |Este erro ocorre se o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) está faltando.  <br/> |
|ErrorMissingInformationReferenceItemId  <br/> |Este erro ocorre se o [ReferenceItemId](referenceitemid.md) estiver faltando.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Este código de erro nunca será retornado.  <br/> |
|ErrorMissingItemForCreateItemAttachment  <br/> |Esse erro é retornado quando é feita uma tentativa para não incluir o item do elemento no elemento **ItemAttachment** de uma solicitação de [operação CreateAttachment](createattachment-operation.md) .  <br/> |
|ErrorMissingManagedFolderId  <br/> |Este erro ocorre quando a propriedade IDs de política, a marca de propriedade 0x6732, para a pasta está faltando. Isso deve ser considerado uma pasta corrompida.  <br/> |
|ErrorMissingRecipients  <br/> |Esse erro indica que você tentou enviar um item sem incluir destinatários. Observe que, se você chamar a [operação CreateItem](createitem-operation.md) com uma disposição de mensagem que faz com que a mensagem a ser enviada, você obterá o seguinte código de resposta: **ErrorInvalidRecipients**.  <br/> |
|ErrorMissingUserIdInformation  <br/> |Esse erro indica que um [ID de usuário](userid.md) não foi especificado totalmente em um conjunto de permissões.  <br/> |
|ErrorMoreThanOneAccessModeSpecified  <br/> |Esse erro indica que você especificou mais de um valor do elemento [ExchangeImpersonation](exchangeimpersonation.md) dentro de uma solicitação.  <br/> |
|ErrorMoveCopyFailed  <br/> |Esse erro indica que a operação de movimentação ou cópia falhou. Movendo ocorre na [operação CreateItem](createitem-operation.md) quando você aceita uma solicitação de reunião que está na pasta Itens excluídos. Além disso, se você recusa uma solicitação de reunião, cancelar um item de calendário ou remove uma reunião do seu calendário, ele é movido para a pasta Itens excluídos.  <br/> |
|ErrorMoveDistinguishedFolder  <br/> |Este erro ocorre se você tentar mover uma pasta diferenciada.  <br/> |
|ErrorMultiLegacyMailboxAccess  <br/> |Este erro ocorre quando uma solicitação tenta acessar vários servidores de caixa de correio. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNameResolutionMultipleResults  <br/> |Este erro ocorre se a [operação ResolveNames](resolvenames-operation.md) retorna mais de um resultado ou o nome ambíguo que você especificou corresponde a mais de um objeto no diretório. O código de resposta inclui os nomes correspondentes nos dados de resposta.  <br/> |
|ErrorNameResolutionNoMailbox  <br/> |Esse erro indica que o chamador não tem uma caixa de correio no sistema. A [operação de ResolveNames](resolvenames-operation.md) ou [ExpandDL](expanddl-operation.md) é inválido para se conectar a um usuário sem uma caixa de correio.  <br/> |
|ErrorNameResolutionNoResults  <br/> |Esse erro indica que a [operação ResolveNames](resolvenames-operation.md) não retornou resultados.  <br/> |
|ErrorNoApplicableProxyCASServersAvailable  <br/> |Este código de erro deve ser retornado quando o serviço da Web não consegue localizar um servidor para processar a solicitação.  <br/> |
|ErrorNoCalendar  <br/> |Este erro ocorre se não houver nenhuma pasta de calendário da caixa de correio.  <br/> |
|ErrorNoDestinationCASDueToKerberosRequirements  <br/> |Esse erro indica que a solicitação conhecido uma caixa de correio em outro site do Active Directory, mas nenhum servidor de acesso para cliente no site de destino foram configurados para autenticação do Windows e, portanto, a solicitação não pôde ser intermediadas por proxy.  <br/> |
|ErrorNoDestinationCASDueToSSLRequirements  <br/> |Esse erro indica que a solicitação conhecido uma caixa de correio em outro site do Active Directory, mas nenhum servidor de acesso para cliente no site de destino foram configurados para conexões SSL e, portanto, a solicitação não pôde ser intermediadas por proxy.  <br/> |
|ErrorNoDestinationCASDueToVersionMismatch  <br/> |Esse erro indica que a solicitação chamado uma caixa de correio em outro site do Active Directory, mas não há servidores de acesso para cliente no site de destino foram de uma versão de produto aceitável para receber a solicitação e, portanto, a solicitação não pôde ser intermediadas por proxy.  <br/> |
|ErrorNoFolderClassOverride  <br/> |Este erro ocorre se você definir o elemento [FolderClass](folderclass.md) quando você estiver criando um item que não seja uma pasta genérico. Para pastas digitadas como [CalendarFolder](calendarfolder.md) e [TasksFolder](tasksfolder.md), a classe de pasta estará implícito. Definindo a classe da pasta a um tipo de pasta diferente usando os resultados da [operação UpdateFolder](updatefolder-operation.md) na resposta **ErrorObjectTypeChanged** . Em vez disso, usar um tipo de pasta genérico, mas definir a classe de pasta para o valor que você precisar. Serviços Web do Exchange criará a pasta fortemente tipada correta.  <br/> |
|ErrorNoFreeBusyAccess  <br/> |Esse erro indica que o chamador não tem direitos de visualização de livre/ocupado na pasta de calendário em questão.  <br/> |
|ErrorNonExistentMailbox  <br/> | Este erro ocorre nos seguintes cenários: <br/> <br/>-O endereço de email está vazio no [CreateManagedFolder](createmanagedfolder.md).  <br/>-O endereço de email não se refere a uma conta válida em uma solicitação que utiliza um endereço de email no corpo ou no cabeçalho SOAP, tais como em uma chamada de representação do Exchange.  <br/> |
|ErrorNonPrimarySmtpAddress  <br/> |Este erro ocorre quando um chamador passa em um endereço de SMTP não principal. A resposta inclui o endereço SMTP correto para usar.  <br/> |
|ErrorNoPropertyTagForCustomProperties  <br/> |Esse erro indica que as propriedades MAPI no intervalo personalizado, 0x8000 e maiores, não pode ser referenciado por marcas de propriedade. Você deve usar a propriedade EWS Managed API [PropertySetId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition.propertysetid%28v=exchg.80%29.aspx)ou o elemento do EWS [ExtendedFieldURI](extendedfielduri.md) com o atributo PropertySetId.  <br/> |
|ErrorNoPublicFolderReplicaAvailable  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorNoPublicFolderServerAvailable  <br/> |Este código de erro deve ser retornado se nenhum servidor de pasta pública está disponível ou se o chamador não tiver um servidor público primário.  <br/> |
|ErrorNoRespondingCASInDestinationSite  <br/> |Esse erro indica que a solicitação mencionado uma caixa de correio em outro site do Active Directory, mas nenhum dos servidores de acesso para cliente em que os sites tiverem respondido e, portanto, a solicitação não pôde ser intermediadas por proxy.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Esse erro indica que o chamador tentou conceder permissões em sua pasta de calendário ou contatos para um usuário de outra organização e a tentativa falhou.  <br/> |
|ErrorNotDelegate  <br/> |Esse erro indica que o usuário não é um representante da caixa de correio. Ele é retornado pela [operação GetDelegate](getdelegate-operation.md), a [operação RemoveDelegate](removedelegate-operation.md)e a [operação UpdateDelegate](updatedelegate-operation.md) quando o usuário delegado especificado não for encontrado na lista de representantes.  <br/> |
|ErrorNotEnoughMemory  <br/> |Esse erro indica que a operação não pôde ser concluída devido a memória insuficiente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Esse erro indica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorObjectTypeChanged  <br/> |Este erro ocorre se o tipo de objeto é alterado.  <br/> |
|ErrorOccurrenceCrossingBoundary  <br/> |Este erro ocorre quando a hora de [início](start.md) ou [fim](end-ex15websvcsotherref.md) de uma ocorrência é atualizada para que a ocorrência esteja programada para acontecer anteriormente ou mais recente do que a ocorrência anterior ou seguinte correspondente.  <br/> |
|ErrorOccurrenceTimeSpanTooBig  <br/> |Esse erro indica que a alocação de tempo para uma determinada ocorrência sobrepõe outra ocorrência do mesmo item recorrente. Essa resposta também ocorre quando a duração em minutos de uma determinada ocorrência for maior do que Int32.MaxValue.  <br/> |
|ErrorOperationNotAllowedWithPublicFolderRoot  <br/> |Esse erro indica que a operação atual não é válida para a raiz da pasta pública.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Esse erro indica que a organização do solicitante não é federada para que o solicitante não é possível criar o compartilhamento de mensagens para enviar a um usuário externo ou não pode aceitar mensagens de compartilhamento recebida de um usuário externo.  <br/> |
|ErrorParentFolderIdRequired  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorParentFolderNotFound  <br/> |Este erro ocorre na [operação CreateFolder](createfolder-operation.md) quando a pasta pai não for encontrada.  <br/> |
|ErrorPasswordChangeRequired  <br/> |Esse erro indica que você deve alterar sua senha antes de poder acessar essa caixa de correio. Esse problema ocorre quando uma nova conta foi criada e o administrador indicado que o usuário deve alterar a senha no primeiro logon. É possível atualizar a senha usando serviços Web do Exchange. Você deve usar uma ferramenta como o Microsoft Office Outlook Web App para alterar sua senha.  <br/> |
|ErrorPasswordExpired  <br/> |Esse erro indica que a senha expirou. Você não pode alterar a senha usando serviços Web do Exchange. Você deve usar uma ferramenta como o Outlook Web App para alterar sua senha.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões no seu calendário ou pasta de contatos para um usuário externo, mas a política de compartilhamento atribuído ao solicitante indica o nível de permissão solicitada é maior que permite que a política de compartilhamento.  <br/> |
|ErrorPhoneNumberNotDialable  <br/> |Esse erro indica que o número de telefone não estava no formato correto.  <br/> |
|ErrorPropertyUpdate  <br/> |Esse erro indica que a atualização falhou devido a valores de propriedade inválido. A mensagem de resposta inclui os caminhos de propriedade inválido.  <br/> |
|ErrorPromptPublishingOperationFailed  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPropertyValidationFailure  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorProxiedSubscriptionCallFailure  <br/> |Esse erro indica que a solicitação conhecido uma assinatura que existe em outro servidor de acesso para cliente, mas falha na tentativa de proxy a solicitação para esse servidor de acesso para cliente.  <br/> |
|ErrorProxyCallFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorProxyGroupSidLimitExceeded  <br/> |Esse erro indica que a solicitação de uma caixa de correio em outro site do Active Directory chamado e o chamador original é um membro dos grupos de mais de 3.000.  <br/> |
|ErrorProxyRequestNotAllowed  <br/> |Esse erro indica que a solicitação de serviços Web do Exchange são enviados para outro servidor de acesso para cliente ao tentar completar uma solicitação de [GetUserAvailabilityRequest](getuseravailabilityrequest.md) era inválida. Normalmente, este código de resposta indica que ocorreu um erro de configuração ou direitos ou que alguém tentou sem sucesso imitar uma solicitação de proxy de disponibilidade.  <br/> |
|ErrorProxyRequestProcessingFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentou proxy uma solicitação de disponibilidade para outro servidor de acesso para cliente para o preenchimento, mas a solicitação falhou. Essa resposta pode ser causada por problemas de conectividade de rede ou problemas de tempo limite de solicitação.  <br/> |
|ErrorProxyServiceDiscoveryFailed  <br/> |Este código de erro deve ser retornado se o serviço da Web não puder determinar se a solicitação é executada no servidor de destino ou será intermediadas por proxy para outro servidor.  <br/> |
|ErrorProxyTokenExpired  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorPublicFolderMailboxDiscoveryFailed  <br/> |Este erro ocorre quando a caixa de correio de pasta pública URL não pode ser encontrado. Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorPublicFolderOperationFailed  <br/> |Este erro ocorre quando é feita uma tentativa de acessar uma pasta pública e a tentativa for bem sucedida. Esse erro foi introduzido no 2013Exchange do Exchange Server 2013.  <br/> |
|ErrorPublicFolderRequestProcessingFailed  <br/> |Este erro ocorre quando o destinatário que foi passado para a [operação GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server que é anterior ao Exchange 2007 e a solicitação para recuperar informações de disponibilidade para o Falha de destinatário a partir do servidor de pasta pública.  <br/> |
|ErrorPublicFolderServerNotFound  <br/> |Este erro ocorre quando o destinatário que foi passado para a [operação GetUserAvailability](getuseravailability-operation.md) está localizado em um computador que está executando uma versão do Exchange Server que é anterior ao Exchange 2007 e a solicitação para recuperar informações de disponibilidade para o destinatário do servidor de pasta pública falhou porque a unidade organizacional não tinha um servidor de pasta pública associado.  <br/> |
|ErrorPublicFolderSyncException  <br/> |Este erro ocorre quando uma operação de sincronização for bem-sucedido contra a caixa de correio de pasta pública principal, mas não tiver êxito contra a caixa de correio de pasta pública secundário. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorQueryFilterTooLong  <br/> |Esse erro indica que a restrição da pasta de pesquisa pode ser válida, mas ela não é suportada pelo EWS. Restrições para conter um máximo de 255 expressões de filtro de limites de serviços Web do Exchange. Se você tentar vincular a uma pasta de pesquisa existente que exceda 255, este código de resposta é retornado.  <br/> |
|ErrorQuotaExceeded  <br/> |Este erro ocorre quando a cota de caixa de correio é excedida.  <br/> |
|ErrorReadEventsFailed  <br/> |Este erro será retornado pelas notificações de push [GetEvents operação](getevents-operation.md) quando ocorre uma falha ao recuperar as informações de evento. Quando esse erro é retornado, a assinatura é excluída. Crie novamente a sincronização de evento com base em uma marca d'água conhecida a última.  <br/> |
|ErrorReadReceiptNotPending  <br/> |Esse erro será retornado pela [operação de CreateItem](createitem-operation.md) , se foi feita uma tentativa para suprimir uma confirmação de leitura quando o remetente da mensagem não solicitou uma confirmação de leitura na mensagem ou se a mensagem está na pasta Lixo eletrônico.  <br/> |
|ErrorRecurrenceEndDateTooBig  <br/> |Este erro ocorre quando a data de término para a recorrência está após 9/1/4500.  <br/> |
|ErrorRecurrenceHasNoOccurrence  <br/> |Este erro ocorre quando a recorrência especificada não tem quaisquer instâncias de ocorrência no intervalo especificado.  <br/> |
|ErrorRemoveDelegatesFailed  <br/> |Esse erro indica que a lista de representantes não puderam ser salvas após representantes foram removidos.  <br/> |
|ErrorRequestAborted  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorRequestStreamTooBig  <br/> | Este erro ocorre quando o fluxo de solicitação é maior que 400 KB.  <br/> |
|ErrorRequiredPropertyMissing  <br/> |Esse erro é retornado quando uma propriedade necessária está ausente em uma solicitação de [operação CreateAttachment](createattachment-operation.md) . A propriedade ausente URI é incluída na resposta.  <br/> |
|ErrorResolveNamesInvalidFolderType  <br/> |Esse erro indica que o chamador tenha especificado uma pasta que não é uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResolveNamesOnlyOneContactsFolderAllowed  <br/> |Esse erro indica que o chamador tenha especificado mais de uma pasta de contatos para a [operação ResolveNames](resolvenames-operation.md).  <br/> |
|ErrorResponseSchemaValidation  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorRestrictionTooLong  <br/> |Este erro ocorre se a restrição contiver mais de 255 nós.  <br/> |
|ErrorRestrictionTooComplex  <br/> |Este erro ocorre quando a restrição não pode ser avaliada pelos serviços Web do Exchange.  <br/> |
|ErrorResultSetTooBig  <br/> |Esse erro indica que o número de entradas de calendário para um determinado destinatário excede o limite permitido de 1000. Reduzir a janela e tente novamente.  <br/> |
|ErrorSavedItemFolderNotFound  <br/> |Este erro ocorre quando o [SavedItemFolderId](saveditemfolderid.md) não for encontrado.  <br/> |
|ErrorSchemaValidation  <br/> | Este erro ocorre quando a solicitação não pode ser validada em relação ao esquema.  <br/> |
|ErrorSearchFolderNotInitialized  <br/> |Esse erro indica que a pasta de pesquisa foi criada, mas os critérios de pesquisa nunca foram definidos na pasta. Isso ocorre apenas quando você acessar pastas de pesquisa corrompido que foram criadas usando a API de outro ou cliente. Para corrigir esse erro, use a [operação UpdateFolder](updatefolder-operation.md) para definir o elemento [SearchParameters](searchparameters.md) para incluir a restrição que deverá estar ligado a pasta.  <br/> |
|ErrorSendAsDenied  <br/> | Este erro ocorre quando as seguintes condições ocorrerem: <br/> <br/>-Um usuário tem permissões CanActAsOwner, mas não recebeu direitos representante da caixa de correio do principal.  <br/>-O mesmo usuário tenta criar e enviar uma mensagem de email na caixa de correio da entidade de segurança usando a opção SendAndSaveCopy.<br/>  <br/>  O resultado é um erro de ErrorSendAsDenied e a criação da mensagem de email na pasta Rascunhos do principal.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Esse erro será retornado pela [operação DeleteItem](deleteitem-operation.md) , se o atributo **SendMeetingCancellations** está ausente da solicitação e excluir o item é um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsOrCancellationsRequired  <br/> |Esse erro será retornado pela [operação UpdateItem](updateitem-operation.md) , se o atributo **SendMeetingCancellations** está ausente da solicitação e o item a ser atualizado é um item de calendário.  <br/> |
|ErrorSendMeetingInvitationsRequired  <br/> |Esse erro será retornado pela [operação de CreateItem](createitem-operation.md) , se o atributo **SendMeetingInvitations** está ausente da solicitação e o item para criar é um item de calendário.  <br/> |
|ErrorSentMeetingRequestUpdate  <br/> |Esse erro indica que, depois que o organizador envia uma solicitação de reunião, a solicitação não pode ser atualizada. Para modificar a reunião, modifique o item de calendário, não a solicitação de reunião.  <br/> |
|ErrorSentTaskRequestUpdate  <br/> |Esse erro indica que, depois que o iniciador de tarefa envia uma solicitação de tarefa, que a solicitação não pode ser atualizada.  <br/> |
|ErrorServerBusy  <br/> |Este erro ocorre quando o servidor está ocupado.  <br/> |
|ErrorServiceDiscoveryFailed  <br/> |Esse erro indica que os serviços Web do Exchange tentou proxy uma solicitação de disponibilidade do usuário para a floresta apropriada para o destinatário, mas ele não foi possível determinar para onde enviar a solicitação por causa de uma falha de descoberta do serviço.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Esse erro indica que a propriedade de URL externa não tiver sido definida no banco de dados do Active Directory.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> |Esse erro indica que uma tentativa de sincronização de uma pasta de compartilhamento falhou. <br/><br/>Este código de erro é retornado quando ocorre o seguinte:<br/><br/>-A assinatura de uma pasta de compartilhamento não for encontrada.<br/>-A pasta de compartilhamento não for encontrada.<br/>-O usuário correspondente do diretório não foi encontrado.<br/>-O usuário não existe mais.<br/>-O compromisso é inválido.<br/>-O item de contato é inválido.<br/>-Não há uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorStaleObject  <br/> |Este erro ocorre em uma [operação UpdateItem](updateitem-operation.md) ou uma [operação SendItem](senditem-operation.md) quando a chave de alteração não está atualizada ou não foi fornecida. Chame a [operação GetItem](getitem-operation.md) para recuperar uma chave de alteração de atualização e, em seguida, tente a operação novamente.  <br/> |
|ErrorSubmissionQuotaExceeded  <br/> |Esse erro indica que um usuário imediatamente não pode enviar solicitações mais porque a cota de envio foi atingida.  <br/> |
|ErrorSubscriptionAccessDenied  <br/> |Este erro ocorre quando você tenta acessar uma assinatura usando uma conta que não criou essa assinatura. Cada inscrição só pode ser acessada pelo criador da assinatura.  <br/> |
|ErrorSubscriptionDelegateAccessNotSupported  <br/> |Esse erro indica que não é possível criar uma assinatura se você não for o proprietário ou não têm acesso de proprietário à caixa de correio.  <br/> |
|ErrorSubscriptionNotFound  <br/> |Este erro ocorre se a assinatura que corresponde à especificado [SubscriptionId (GetEvents)](subscriptionid-getevents.md) não for encontrada. A assinatura pode ter expirado, o processo de serviços Web do Exchange pode ter sido reiniciado ou uma assinatura inválida foi passada. Se a assinatura for válida, recriar a assinatura com a marca d'água mais recente. Isso é retornado pelas respostas de [operação GetEvents](getevents-operation.md) ou a [operação de cancelamento da assinatura](unsubscribe-operation.md) .  <br/> |
|ErrorSubscriptionUnsubsribed  <br/> |Este código de erro deve ser retornado quando for feita uma solicitação para uma inscrição que foi cancelada.  <br/> |
|ErrorSyncFolderNotFound  <br/> |Esse erro será retornado pela [operação SyncFolderItems](syncfolderitems-operation.md) , se a pasta pai especificado não pode ser encontrada.  <br/> |
|ErrorTeamMailboxNotFound  <br/> |Esse erro indica que uma caixa de correio de equipe não foi localizada. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotLinkedToSharePoint  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas não estiver vinculada a um servidor do SharePoint. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxUrlValidationFailed  <br/> |Esse erro indica que uma caixa de correio de equipe foi encontrada, mas o link para o SharePoint Server não é válido. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxNotAuthorizedOwner  <br/> |Este código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxActiveToPendingDelete  <br/> |Este código de erro não é usado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxFailedSendingNotifications  <br/> |Esse erro indica que uma tentativa de enviar uma notificação para os proprietários de caixa de correio de equipe não foi bem-sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTeamMailboxErrorUnknown  <br/> |Esse erro indica um erro geral que pode ocorrer ao tentar acessar uma caixa de correio de equipe. Tente enviar a solicitação mais tarde. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorTimeIntervalTooBig  <br/> |Esse erro indica que a janela de tempo especificada for maior do que o limite permitido. Por padrão, o limite permitido é 42.  <br/> |
|ErrorTimeoutExpired  <br/> | Este erro ocorre quando não há tempo suficiente para concluir o processamento da solicitação.  <br/> |
|ErrorTimeZone  <br/> |Esse erro indica que há um erro de fuso horário.  <br/> |
|ErrorToFolderNotFound  <br/> |Esse erro indica que a pasta de destino não existe.  <br/> |
|ErrorTokenSerializationDenied  <br/> |Este erro ocorre se o chamador tenta fazer uma solicitação de serialização de Token, mas não tem o ms-Exch-EPI-TokenSerialization direita no servidor acesso para cliente.  <br/> |
|ErrorTooManyObjectsOpened  <br/> |Este erro ocorre quando o limite interno em objetos open foi excedido.  <br/> |
|ErrorUnifiedMessagingDialPlanNotFound  <br/> |Esse erro indica que o plano de discagem de um usuário não está disponível.  <br/> |
|ErrorUnifiedMessagingReportDataNotFound  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingPromptNotFound  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnifiedMessagingRequestFailed  <br/> |Esse erro indica que o usuário não pôde ser encontrado.  <br/> |
|ErrorUnifiedMessagingServerNotFound  <br/> |Esse erro indica que um servidor válido para o plano de discagem pode ser encontrado deverá para processar a solicitação.  <br/> |
|ErrorUnableToGetUserOofSettings  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnableToRemoveImContactFromGroup  <br/> |Este erro ocorre quando uma tentativa malsucedida para remover um contato de mensagens Instantâneas de um grupo. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUnsupportedCulture  <br/> |Este erro ocorre quando você tenta definir a propriedade de **cultura** como um valor que não é passível de análise por classe **System.Globalization.CultureInfo** .  <br/> |
|ErrorUnsupportedMapiPropertyType  <br/> |Este erro ocorre quando um chamador tenta usar propriedades estendidas do objeto tipos, matriz de objeto, erro ou nulo.  <br/> |
|ErrorUnsupportedMimeConversion  <br/> |Este erro ocorre quando você está tentando recuperar ou definir o conteúdo MIME para um item que não seja um objeto [PostItem](postitem.md), uma [mensagem](message-ex15websvcsotherref.md)ou [CalendarItem](calendaritem.md) .  <br/> |
|ErrorUnsupportedPathForQuery  <br/> |Este erro ocorre quando o chamador passa uma propriedade que é inválida para uma consulta. Isso pode ocorrer quando propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPathForSortGroup  <br/> |Este erro ocorre quando o chamador passa uma propriedade que não é válida para um grupo pela propriedade ou classificação. Isso pode ocorrer quando propriedades calculadas são usadas.  <br/> |
|ErrorUnsupportedPropertyDefinition  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnsupportedQueryFilter  <br/> |Esse erro indica que a restrição da pasta de pesquisa pode ser válida, mas ela não é suportada pelo EWS.  <br/> |
|ErrorUnsupportedRecurrence  <br/> |Esse erro indica que a recorrência especificada não é suportada para tarefas.  <br/> |
|ErrorUnsupportedSubFilter  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorUnsupportedTypeForConversion  <br/> |Esse erro indica que serviços Web do Exchange encontrado um tipo de propriedade no armazenamento, mas ele não é possível gerar XML para o tipo de propriedade.  <br/> |
|ErrorUpdateDelegatesFailed  <br/> |Esse erro indica que a lista de representantes não puderam ser salvas depois representantes foram atualizados.  <br/> |
|ErrorUpdatePropertyMismatch  <br/> |Este erro ocorre quando o caminho de única propriedade que está listado em uma descrição de alteração não corresponde a única propriedade que está sendo definida dentro do objeto de [Item](item.md) ou [pasta](folder.md) real.  <br/> |
|ErrorUserNotUnifiedMessagingEnabled  <br/> |Esse erro indica que o solicitante não está habilitado.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Esse erro indica que o solicitante tentou conceder permissões no seu calendário ou pasta de contatos para um usuário externo, mas a política de compartilhamento atribuído ao solicitante indica que o domínio de usuário externo não está listado na política.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Indica que a organização do solicitante tem um conjunto de domínios federados, mas a organização do solicitante não tem quaisquer endereços de proxy de SMTP com um dos domínios federados.  <br/> |
|ErrorValueOutOfRange  <br/> |Esse erro indica que a data de início de um modo de exibição de calendário ou data final foi definida como 1/1/0001 12:00:00 AM ou 31/12/9999 11:59:59 PM.  <br/> |
|ErrorVirusDetected  <br/> |Esse erro indica que o repositório do Exchange detectado um vírus na mensagem.  <br/> |
|ErrorVirusMessageDeleted  <br/> |Esse erro indica que o repositório do Exchange detectou um vírus na mensagem e excluídos-lo.  <br/> |
|ErrorVoiceMailNotImplemented  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWebRequestInInvalidState  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWin32InteropError  <br/> |Esse erro indica que houve uma falha interna durante a comunicação com o código não gerenciado.  <br/> |
|ErrorWorkingHoursSaveFailed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWorkingHoursXmlMalformed  <br/> |Este código de resposta não é usado.  <br/> |
|ErrorWrongServerVersion  <br/> |Esse erro indica que uma solicitação só pode ser feita em um servidor que é a mesma versão que o servidor de caixa de correio.  <br/> |
|ErrorWrongServerVersionDelegate  <br/> |Esse erro indica que uma solicitação foi feita por um delegado que tem uma versão de servidor diferente que o servidor de caixa de correio do principal.  <br/> |
|ErrorMissingInformationSharingFolderId  <br/> |Este código de erro nunca será retornado.  <br/> |
|ErrorDuplicateSOAPHeader  <br/> |Especifica que não existem duplicados cabeçalhos SOAP.  <br/> |
|ErrorSharingSynchronizationFailed  <br/> | Especifica que uma tentativa de sincronização de uma pasta de compartilhamento falhou.<br/><br/> Este código de erro deve ser retornado quando:<br/><br/>-A assinatura de uma pasta de compartilhamento não for encontrada.  <br/>-A pasta de compartilhamento não foi encontrada.  <br/>-O usuário correspondente do diretório não foi encontrado.  <br/>-O usuário não existe mais.  <br/>-O compromisso é inválido.  <br/>-O item de contato é inválido.  <br/>-Houve uma falha de comunicação com o servidor remoto.  <br/> |
|ErrorSharingNoExternalEwsAvailable  <br/> |Especifica que a propriedade de URL externa não tiver sido definida no banco de dados do Active Directory. Este código de erro deve ser retornado se a propriedade de URL externa não tiver sido definida no banco de dados do Active Directory.  <br/> |
|ErrorFreeBusyDLLimitReached  <br/> |Especifica que a contagem de membro do grupo máximo foi atingida para obtenção de informações de disponibilidade para obter uma lista de distribuição. Esse erro deve ser retornado quando a contagem de membro do grupo máximo foi atingida para obtenção de informações de disponibilidade para obter uma lista de distribuição.  <br/> |
|ErrorInvalidGetSharingFolderRequest  <br/> |Especifica que o elemento de tipo de dados e ShareFolderId são ambos presentes em uma solicitação. Este código de erro deve ser retornado se o elemento de tipo de dados e ShareFolderId estiverem presentes em uma solicitação.  <br/> |
|ErrorNotAllowedExternalSharingByPolicy  <br/> |Especifica que o chamador tentou conceder permissões em sua pasta de calendário ou contatos para um usuário em outra organização e a tentativa falhou. Este código de erro deve ser retornado quando a política de compartilhamento é desabilitada para o chamador ou quando a política de compartilhamento atribuída ao chamador proíbe o compartilhamento para o nível solicitado ou o tipo de pasta solicitada.  <br/> |
|ErrorUserNotAllowedByPolicy  <br/> |Especifica que o solicitante tentou conceder permissões no seu calendário ou pasta de contatos para um usuário externo, mas a política de compartilhamento atribuído ao solicitante Especifica que o domínio de usuário externo não está listado na política.  <br/> |
|ErrorPermissionNotAllowedByPolicy  <br/> |Especifica que o solicitante tentado conceder permissões em sua pasta de calendário ou contatos para um usuário externo, mas a política de compartilhamento atribuído ao solicitante Especifica que o nível de permissão solicitada é maior que a política de compartilhamento que permite.  <br/> |
|ErrorOrganizationNotFederated  <br/> |Especifica que a organização do solicitante não é federada para que o solicitante não é possível criar o compartilhamento de mensagens para enviar a um usuário externo ou não pode aceitar mensagens de compartilhamento recebida de um usuário externo. Este código de erro deve ser retornado se a organização do solicitante não é federada.  <br/> |
|ErrorMailboxFailover  <br/> |Especifica que uma tentativa de acessar uma caixa de correio falhou porque a caixa de correio está em um processo de failover.  <br/> |
|ErrorInvalidExternalSharingInitiator  <br/> |Especifica que o remetente do convite de compartilhamento não criou os metadados de convite de compartilhamento. Este código de erro deve ser retornado se o remetente do convite de compartilhamento não criou os metadados de convite de compartilhamento.  <br/> |
|ErrorMessageTrackingPermanentError  <br/> |Especifica que o serviço de controle de mensagens não podem controlar a mensagem.  <br/> |
|ErrorMessageTrackingTransientError  <br/> |Especifica que o serviço de controle de mensagens está inoperante ou ocupado. Este código de erro Especifica um erro transitório. Clientes podem tentar para se conectar ao servidor quando esse erro é recebido.  <br/> |
|ErrorMessageTrackingNoSuchDomain  <br/> |Especifica que o domínio indicado não foi encontrado.  <br/> |
|ErrorUserWithoutFederatedProxyAddress  <br/> |Especifica que a organização do solicitador tem um conjunto de domínios federados mas organização do solicitante não tem quaisquer endereços de proxy de SMTP com um dos domínios federados.  <br/> |
|ErrorInvalidOrganizationRelationshipForFreeBusy  <br/> |Especifica que um chamador solicitou informações de disponibilidade para um usuário de outra organização, mas a relação organizacional não tem livre/ocupado habilitado.  <br/> |
|ErrorInvalidFederatedOrganizationId  <br/> |Especifica se objetos de Federação da organização do solicitador não estão configurados corretamente.  <br/> |
|ErrorInvalidExternalSharingSubscriber  <br/> |Especifica que uma mensagem de compartilhamento não foi destinada para o chamador.  <br/> |
|ErrorInvalidSharingData  <br/> |Especifica se os metadados de compartilhamento não são válido. Isso pode ser causado por XML inválido.  <br/> |
|ErrorInvalidSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é válida. Isso pode ser causado por uma propriedade ausente.  <br/> |
|ErrorNotSupportedSharingMessage  <br/> |Especifica que a mensagem de compartilhamento não é suportada.  <br/> |
|ErrorApplyConversationActionFailed  <br/> |Esse erro deve ser retornado se uma ação não pode ser aplicada a um ou mais itens na conversa.  <br/> |
|ErrorInboxRulesValidationError  <br/> |Esse erro deve ser retornado se qualquer regra de validação não.  <br/> |
|ErrorOutlookRuleBlobExists  <br/> |Esse erro deve ser retornado quando uma tentativa de gerenciar regras de caixa de entrada ocorre após o outro cliente acessou as regras de caixa de entrada.  <br/> |
|ErrorRulesOverQuota  <br/> |Esse erro deve ser retornado quando a cota de regra de um usuário foi excedida.  <br/> |
|ErrorNewEventStreamConnectionOpened  <br/> |Esse erro deve ser retornado para a conexão de assinatura primeiro se uma conexão de inscrição a segunda é aberto.  <br/> |
|ErrorMissedNotificationEvents  <br/> |Esse erro deve ser retornado quando as notificações de evento são perdidas.  <br/> |
|ErrorDuplicateLegacyDistinguishedName  <br/> |Esse erro é retornado quando há nomes duplicados herdados nos serviços de domínio Active Directory (AD DS). Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidClientAccessTokenRequest  <br/> |Esse erro indica que uma solicitação para obter um acesso para cliente token não era válida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorNoSpeechDetected  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorUMServerUnavailable  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecipientNotFound  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorRecognizerNotInstalled  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSpeechGrammarError  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidManagementRoleHeader  <br/> |Esse erro será retornado se o cabeçalho [ManagementRole](managementrole.md) no cabeçalho SOAP está incorreto. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesDisabled  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestTimedOut  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesRequestFailed  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorLocationServicesInvalidRequest  <br/> |Esse erro é destinado apenas para uso interno. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorWeatherServiceDisabled  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorMailboxScopeNotAllowedWithoutQueryString  <br/> |Esse erro é retornado quando uma tentativa de pesquisa com escopo é executada sem usar um elemento [QueryString (String)](querystring-string.md) para um pesquisa de indexação de conteúdo. Isso é aplicável às operações **SearchMailboxes** e **FindConversation** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxSearchFailed  <br/> |Esse erro é retornado quando uma pesquisa de caixas de correio de arquivo morto é bem sucedida. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorArchiveMailboxServiceDiscoveryFailed  <br/> |Esse erro é retornado quando a URL de uma caixa de correio de arquivo morto não é detectável. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorGetRemoteArchiveFolderFailed  <br/> |Este erro ocorre quando a operação obter a pasta de caixa de correio de arquivamento remoto falhou.  <br/> |
|ErrorFindRemoteArchiveFolderFailed  <br/> |Este erro ocorre quando a operação localizar a pasta de caixa de correio de arquivamento remoto falhou.  <br/> |
|ErrorGetRemoteArchiveItemFailed  <br/> |Este erro ocorre quando a operação obter o item de caixa de correio de arquivamento remoto falhou.  <br/> |
|ErrorExportRemoteArchiveItemsFailed  <br/> |Este erro ocorre quando a operação para exportar itens de caixa de correio de arquivamento remoto falhou.  <br/> |
|ErrorInvalidPhotoSize  <br/> |Esse erro será retornado se for solicitado um tamanho de foto inválida do servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchQueryHasTooManyKeywords  <br/> |Esse erro é retornado quando for solicitado um tamanho de foto inesperada em uma solicitação de operação **GetUserPhoto** . Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorSearchTooManyMailboxes  <br/> |Esse erro é retornado quando uma solicitação de operação **SearchMailboxes** contém muitas caixas de correio a ser pesquisado. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorInvalidRetentionTagNone  <br/> |Esse erro indica que nenhuma marcas de retenção foram encontradas para este usuário. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorDiscoverySearchesDisabled  <br/> |Esse erro é retornado quando pesquisas de descoberta estão desabilitadas em um locatário ou servidor. Esse erro foi introduzido no Exchange 2013.  <br/> |
|ErrorCalendarSeekToConditionNotSupported  <br/> |Este erro ocorre ao tentar chamar a [operação FindItem](finditem-operation.md) com um [SeekToConditionPageItemView](seektoconditionpageitemview.md) de busca de itens de calendário, que não é suportada.  <br/> |
|ErrorCalendarIsGroupMailboxForAccept  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForDecline  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForTentative  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorCalendarIsGroupMailboxForSuppressReadReceipt  <br/> |Esse erro é destinado apenas para uso interno.  <br/> |
|ErrorOrganizationAccessBlocked  <br/> |O inquilino é marcado para remoção.  <br/> |
|ErrorInvalidLicense  <br/> |O usuário não tem uma licença válida.  <br/> |
|ErrorMessagePerFolderCountReceiveQuotaExceeded  <br/> |Receber a mensagem por pasta da cota foi excedida.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Este elemento não é necessário e não está incluído em todas as respostas. 
  
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

