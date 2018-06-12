---
title: MeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingResponse
api_type:
- schema
ms.assetid: 9f798e79-dafd-4d4d-9967-95fd8e5c0502
description: O elemento MeetingResponse representa uma resposta de reunião no armazenamento do Exchange.
ms.openlocfilehash: c5f9f3ac2fcd12e9c95f663311c33cdd36783251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824446"
---
# <a name="meetingresponse"></a>MeetingResponse

O elemento **MeetingResponse** representa uma resposta de reunião no armazenamento do Exchange. 
  
```xml
<MeetingResponse>
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
   <Importance/>
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
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
</MeetingResponse>
```

 **MeetingResponseMessageType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo MIME nativo de um objeto que é representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange. Esta propriedade é somente leitura.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta. Esta propriedade é somente leitura.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para armazenar itens do Exchange e objetos de resposta. O assunto é limitado a 255 caracteres.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica o nível de sensibilidade de um item.  <br/> |
|[Corpo](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e hora em que um item em uma caixa de correio foi recebido.  <br/> |
|[Size](size.md) <br/> |Representa o tamanho em bytes de um item. Esta propriedade é somente leitura.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam a quais categorias de um item na caixa de correio pertence.  <br/> |
|[Importância](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Representa o identificador do item ao qual este item é uma resposta.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indica se um item foi enviado à pasta padrão caixa de saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indica se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviada a um item para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item anteriormente foi enviado.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagem da Internet que está contido dentro de um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e hora quando o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento, quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa para. Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível. Esta propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Contém um conjunto de destinatários de uma mensagem.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Representa uma coleção dos destinatários que receberão uma cópia da mensagem.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Representa uma coleção de destinatários para receber uma cópia oculta (Cco) de um email.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Indica se o remetente de um item solicita uma confirmação de leitura.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Indica se o remetente de um item solicita uma confirmação de entrega.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Contém uma ID binária que representa o segmento ao qual esta mensagem pertence.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Representa o identificador de conversa.  <br/> |
|[From](from.md) <br/> |Representa o destinatário de quem a mensagem foi enviada.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Representa o identificador de mensagem da Internet de um item.  <br/> |
|[Foi lido](isread.md) <br/> |Indica se uma mensagem foi lido.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Indica se uma resposta a uma mensagem de email é solicitada.  <br/> |
|[Referências](references.md) <br/> |Representa o cabeçalho de Usenet é usado para correlacionar respostas com suas mensagens originais.  <br/> |
|[ReplyTo](replyto.md) <br/> |Identifica um conjunto de endereços para o qual as respostas devem ser enviadas.  <br/> |
|[AssociatedCalendarItemId](associatedcalendaritemid.md) <br/> |Representa o item de calendário que está associado um [MeetingMessage](meetingmessage.md).  <br/> |
|[IsDelegated](isdelegated.md) <br/> |Indica se uma reunião foi tratada por uma conta com acesso de representante.  <br/> |
|[IsOutOfDate](isoutofdate.md) <br/> |Indica se uma mensagem de reunião desatualizada.  <br/> |
|[HasBeenProcessed](hasbeenprocessed.md) <br/> |Indica se uma mensagem de reunião item foi processada.  <br/> |
|[ResponseType](responsetype.md) <br/> |Representa o tipo de destinatário resposta recebida para uma reunião.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta. Este elemento é somente leitura. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Identifica o delegado em um cenário de acesso de representante. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Identifica a entidade em um cenário de acesso de representante. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UID](uid.md) <br/> |Identifica um item de calendário.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Usado para identificar uma instância específica de um item de calendário recorrente.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Indica a data e hora em que uma instância de um objeto iCalendar foi criada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Identifica todos os itens de calendário que são adjacentes para um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que estão em conflito com um tempo de reunião.  <br/> |
|[Criar (ItemSync)](create-itemsync.md) <br/> |Identifica um único item para criar no repositório de cliente local.  <br/> |
|[Items](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens para criar.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange que está anexado a outro item do Exchange.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Atualização (ItemSync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no repositório de cliente local.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

