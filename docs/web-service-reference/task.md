---
title: Tarefa
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: O elemento Task representa uma tarefa no repositório do Exchange.
ms.openlocfilehash: 669f90dfa74cd085091e9836a1d31ca53bbf165e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458940"
---
# <a name="task"></a>Tarefa

O elemento **Task** representa uma tarefa no repositório do Exchange. 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

**TaskType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto de itens do repositório do Exchange e objetos de resposta.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Contém o status da sensibilidade de um item.  <br/> |
|[Body](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no repositório do Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e a hora em que um item foi recebido em uma caixa de correio.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho, em bytes, de um item. Essa propriedade é somente leitura.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.  <br/> |
|[Importance](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[Inresponderto](inreplyto.md) <br/> |Representa o identificador do item para o qual este item é uma resposta.  <br/> |
|[Isenviado](issubmitted.md) <br/> |Indica se um item foi enviado para a pasta padrão da pasta de saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indica se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviou um item para ele.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item foi enviado anteriormente.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[Propriedadeinternetmessageheaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item da caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no repositório do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
|[ActualWork](actualwork.md) <br/> |Representa o tempo real gasto em uma tarefa.  <br/> |
|[AssignedTime](assignedtime.md) <br/> |Representa a hora em que uma tarefa é atribuída a um contato.  <br/> |
|[BillingInformation](billinginformation.md) <br/> |Contém informações de cobrança de uma tarefa.  <br/> |
|[ChangeCount](changecount.md) <br/> |Especifica a versão da tarefa.  <br/> |
|[Companies](companies.md) <br/> |Representa a coleção de empresas que estão associadas a um contato ou a uma tarefa.  <br/> |
|[Concluído](completedate.md) <br/> |Representa a data na qual uma tarefa foi concluída.  <br/> |
|[Contatos](contacts-ex15websvcsotherref.md) <br/> |Contém uma lista de contatos que estão associados a uma tarefa.  <br/> |
|[DelegationState](delegationstate.md) <br/> |Representa o status de uma tarefa delegada.  <br/> |
|[Delegator](delegator.md) <br/> |Contém o nome do delegante que atribuiu a tarefa.  <br/> |
|[DueDate](duedate.md) <br/> |Representa a data de vencimento de um item de tarefa.  <br/> |
|[IsAssignmentEditable](isassignmenteditable.md) <br/> |Indica se a tarefa é editável ou não.  <br/> |
|[IsComplete](iscomplete.md) <br/> |Indica se a tarefa foi concluída ou não.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Indica se uma tarefa faz parte de um item recorrente. Este elemento é somente leitura.  <br/> |
|[IsTeamTask](isteamtask.md) <br/> |Indica se a tarefa pertence a uma equipe ou não.  <br/> |
|[Mileage](mileage.md) <br/> |Representa a quilometragem de um item de tarefa.  <br/> |
|[Owner](owner.md) <br/> |Representa o proprietário de uma tarefa.  <br/> |
|[PercentComplete](percentcomplete.md) <br/> |Descreve o status de conclusão de uma tarefa.  <br/> |
|[Recorrência (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contém informações de recorrência para tarefas recorrentes.  <br/> |
|[StartDate](startdate.md) <br/> |Representa a data de início de um item de tarefa.  <br/> |
|[Status](status.md) <br/> |Representa o status de um item de tarefa.  <br/> |
|[StatusDescription](statusdescription.md) <br/> |Contém uma explicação sobre o status da tarefa.  <br/> |
|[TotalWork](totalwork.md) <br/> |Contém uma descrição de quanto trabalho está associado a um item.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta. Este elemento é somente leitura.  <br/> |
|[LastModified](lastmodifiedname.md) <br/> |Contém o nome de exibição do último usuário a modificar um item.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indica quando um item foi modificado pela última vez.  <br/> |
|[Isassociated](isassociated.md) <br/> |Indica se o item está associado a uma pasta.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador de um item ou uma conversa.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Representa um fragmento HTML ou texto sem formatação que representa o corpo exclusivo desta conversa.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item/pasta durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que entram em conflito com um horário de reunião.  <br/> |
|[Create (issync)](create-itemsync.md) <br/> |Identifica um único item a ser criado no armazenamento do cliente local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange anexado a outro item do Exchange.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Setitemfield](setitemfield.md) <br/> |Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Atualização (issync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no repositório do cliente local.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [Excluir tarefas](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

