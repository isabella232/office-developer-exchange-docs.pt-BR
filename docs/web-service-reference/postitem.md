---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: O elemento PostItem representa um item de postagem no armazenamento do Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824866"
---
# <a name="postitem"></a>PostItem

O elemento **PostItem** representa um item de postagem no armazenamento do Exchange. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo de email extensões MIME (Multipurpose Internet) nativo de um objeto que é representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange. Esta propriedade é somente leitura.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta. Esta propriedade é somente leitura.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para armazenar itens do Exchange e objetos de resposta. O assunto é limitado a 255 caracteres.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica o nível de sensibilidade de um item.  <br/> |
|[Corpo](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e hora em que um item em uma caixa de correio foi recebido.  <br/> |
|[Size](size.md) <br/> |Representa o tamanho em bytes de um item. Esta propriedade é somente leitura.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam as categorias para o qual um item na caixa de correio pertence.  <br/> |
|[Importância](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Representa o identificador do item ao qual este item é uma resposta.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indica se um item foi enviado à pasta padrão caixa de saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indica se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviada a um item para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item anteriormente foi enviado.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e hora quando o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento, quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da caixa para. Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo. Esta propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta. Este elemento é somente leitura.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contém o nome de exibição do último usuário para modificar um item.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indica quando um item da última modificação.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indica se o item está associado a uma pasta.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Representa uma URL para concatenar no ponto de extremidade do Microsoft Office Outlook Web App para ler um item no Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Representa uma URL para concatenar no ponto de extremidade do Outlook Web App para editar um item no Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador de um item ou conversa.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Representa um fragmento HTML ou texto sem formatação que representa um único corpo da conversa.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Contém uma ID binária que representa o segmento ao qual esta mensagem pertence.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Representa o identificador de conversa.  <br/> |
|[From](from.md) <br/> |Representa o endereço do qual o item de postagem foi enviado. O elemento **de** só pode ser definido no momento da criação.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Representa o identificador de mensagem da Internet de um item.  <br/> |
|[Foi lido](isread.md) <br/> |Indica se uma mensagem foi lido.  <br/> |
|[PostedTime](postedtime.md) <br/> |Representa a hora em que um [PostItem](postitem.md) postado.  <br/> |
|[Referências](references.md) <br/> |Representa o cabeçalho Usenet que é usado para associar respostas a mensagens originais.  <br/> |
|[Sender](sender.md) <br/> |Identifica o remetente de um item.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange que está anexado a outro item do Exchange.  <br/> |
|[Criar (ItemSync)](create-itemsync.md) <br/> |Identifica um único item para criar no repositório de cliente local.  <br/> |
|[Atualização (ItemSync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no repositório de cliente local.  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |Retornados em respostas [SyncFolderItems](syncfolderitems.md) quando um item foi lido. Esta propriedade é somente leitura. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[Items](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que estão em conflito com um tempo de reunião.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário que são adjacentes para um horário de reunião.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

