---
title: Item
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: O elemento item representa um item genérico no repositório do Exchange.
ms.openlocfilehash: 72d8b1344bea3bcd105a0e293365b17f37193ac3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460313"
---
# <a name="item"></a>Item

O elemento **Item** representa um item genérico no repositório do Exchange. 
  
```xml
<Item>
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
</Item>
```

 **ItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange. Essa propriedade é somente leitura.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta. Essa propriedade é somente leitura.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto de itens do repositório do Exchange e objetos de resposta. O assunto está limitado a 255 caracteres.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indica o nível de sensibilidade de um item.  <br/> |
|[Body](body.md) <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item no repositório do Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e a hora em que um item foi recebido em uma caixa de correio.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho em bytes de um item. Essa propriedade é somente leitura.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam a quais categorias um item da caixa de correio pertence.  <br/> |
|[Importance](importance.md) <br/> |Descreve a importância de um item.  <br/> |
|[Inresponderto](inreplyto.md) <br/> |Representa o identificador do item para o qual este item é uma resposta.  <br/> |
|[Isenviado](issubmitted.md) <br/> |Indica se um item foi enviado para a pasta padrão da pasta de saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Indica se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviou um item para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item foi enviado anteriormente.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[Propriedadeinternetmessageheaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagens da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item da caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no repositório do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa CC. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da caixa para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem anexos de pelo menos um anexo visível. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um determinado item em uma caixa de correio.  <br/> |
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
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[Setitemfield](setitemfield.md) <br/> |Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Atualização (issync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no repositório do cliente local.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

É importante observar que **ItemType** é o tipo base para [Task](task.md), [CalendarItem](calendaritem.md), [Contact](contact.md), [DistributionList](distributionlist.md)e [Message](message-ex15websvcsotherref.md).
  
Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema dos serviços Web do Exchange (EWS). Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de **mensagem** . O Microsoft Exchange Server 2010 não retorna o elemento de **Item** base nas respostas. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
  
[Referência do EWS para Exchange](ews-reference-for-exchange.md)

