---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: O elemento PostItem representa um item post no Exchange store.
ms.openlocfilehash: 1d30c64482e4dbf9731141c3f5f2b30e4b9f9e5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516430"
---
# <a name="postitem"></a>PostItem

O **elemento PostItem** representa um item post no Exchange store. 
  
```xml
<PostItem>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 **PostItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo nativo de Extensões de Email da Internet (MIME) de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no Exchange store. Essa propriedade é somente leitura.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou pasta. Essa propriedade é somente leitura.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para Exchange itens de armazenamento e objetos de resposta. O assunto é limitado a 255 caracteres.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica o nível de sensibilidade de um item.  <br/> |
|[Body](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no Exchange store.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi recebido.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho em bytes de um item. Essa propriedade é somente leitura.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam as categorias às quais um item na caixa de correio pertence.  <br/> |
|[Importance](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Representa o identificador do item ao qual este item é uma resposta.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indica se um item foi enviado para a pasta padrão da Caixa de Saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Representa se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviou um item para ele ou para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item foi enviado anteriormente.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os headers de mensagens da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo [elemento ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no Exchange store.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatário Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa Para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição do destinatário Para.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade definida como **true se** um item tiver pelo menos um anexo. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contém o nome de exibição do último usuário para modificar um item.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indica quando um item foi modificado pela última vez.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indica se o item está associado a uma pasta.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade Microsoft Office Outlook Web App para ler um item em Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Representa uma URL a ser concatenada ao ponto de extremidade Outlook Web App para editar um item em Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador de um item ou conversa.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Representa um fragmento HTML ou texto simples que representa o corpo exclusivo dessa conversa.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Contém uma ID binária que representa o thread ao qual esta mensagem pertence.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Representa o identificador de conversa.  <br/> |
|[De](from.md) <br/> |Representa o endereço do qual o item post foi enviado. O **elemento From** só pode ser definido no momento da criação.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Representa o identificador de mensagem da Internet de um item.  <br/> |
|[IsRead](isread.md) <br/> |Indica se uma mensagem foi lida.  <br/> |
|[PostedTime](postedtime.md) <br/> |Representa a hora em que [um PostItem](postitem.md) foi postado.  <br/> |
|[Referências](references.md) <br/> |Representa o header Usenet usado para associar respostas às mensagens originais.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica dados a ser anexados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem.](updateitem-operation.md)  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um Exchange que está anexado a outro Exchange item.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Identifica um único item a ser criado no armazenamento do cliente local.  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no armazenamento cliente local.  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |Retornado em [respostas SyncFolderItems](syncfolderitems.md) quando um item foi lido. Essa propriedade é somente leitura. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que conflitam com um horário de reunião.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

