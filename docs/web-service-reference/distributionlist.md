---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: O elemento DistributionList representa uma lista de distribuição.
ms.openlocfilehash: 1ca198543c6da62827f2f2b0fe2b7ec9c7e79615
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545269"
---
# <a name="distributionlist"></a>DistributionList

O **elemento DistributionList** representa uma lista de distribuição. 
  
```xml
<DistributionList>
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
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 **DistributionListType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo MIME nativo de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item de lista de distribuição no Exchange store.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item da lista de distribuição.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item de lista de distribuição.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para Exchange itens de armazenamento e objetos de resposta.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Contém o status da sensibilidade de um item de lista de distribuição.  <br/> |
|[Body](body.md) <br/> |Representa o conteúdo real do corpo de um item de lista de distribuição.  <br/> |
|[Anexos](attachments-ex15websvcsotherref.md) <br/> |Contém os itens ou arquivos anexados a um item de lista de distribuição no Exchange store.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Representa a data e a hora em que um item de lista de distribuição em uma caixa de correio foi recebido.  <br/> |
|[Tamanho](size.md) <br/> |Representa o tamanho, em bytes, de um item de lista de distribuição. Essa propriedade é somente leitura.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Representa uma coleção de cadeias de caracteres que identificam a quais categorias pertence um item de lista de distribuição na caixa de correio.  <br/> |
|[Importance](importance.md) <br/> |Descreve a importância de um item de lista de distribuição.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Representa o identificador do item que este item é uma resposta.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Indica se um item foi enviado para a pasta padrão da Caixa de Saída.  <br/> |
|[IsDraft](isdraft.md) <br/> |Representa se um item ainda não foi enviado.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviou um item para si mesmo.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item foi enviado anteriormente.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os headers de mensagens da Internet contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta associados a um item no Exchange store.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo [elemento ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no Exchange store.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatário Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha Para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição do destinatário Para.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade definida como **true se** um item tiver pelo menos um anexo visível. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica propriedades estendidas em um item de lista de distribuição.  <br/> |
|[Cultura](culture.md) <br/> |Representa a cultura de um item de lista de distribuição em uma caixa de correio.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão do item ou pasta. Esse elemento é somente leitura.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Contém o nome de exibição do último usuário para modificar um item.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Indica quando um item foi modificado pela última vez.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Indica se o item está associado a uma pasta.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Representa uma URL para concatenar ao ponto de extremidade Microsoft Office Outlook Web App para ler um item em Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Representa uma URL a ser concatenada ao ponto de extremidade Outlook Web App para editar um item em Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador de um item ou conversa.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Representa um fragmento HTML ou texto simples que representa o corpo exclusivo dessa conversa.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Define o nome de exibição de uma lista de distribuição.  <br/> |
|[FileAs](fileas.md) <br/> |Representa como uma lista de distribuição é arquivada na pasta Contatos.  <br/> |
|[ContactSource](contactsource.md) <br/> |Descreve se o contato está localizado no Exchange ou no Active Directory Domain Services (AD DS).  <br/> |
|[Members (MemberListType)](members-memberlisttype.md) <br/> |Contém uma lista de membros da lista de distribuição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica dados a ser anexados a uma única propriedade de uma lista de distribuição durante uma [operação UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que conflitam com um horário de reunião.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Identifica uma única lista de distribuição a ser criado no armazenamento de cliente local.  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Identifica uma única lista de distribuição a ser atualizada no armazenamento cliente local.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a ser criado na pasta identificada pelo [elemento ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item de lista de distribuição em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
   
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

