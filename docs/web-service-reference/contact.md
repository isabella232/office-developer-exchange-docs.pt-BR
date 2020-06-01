---
title: Contato
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: O elemento Contact representa um item de contato no repositório do Exchange.
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44445647"
---
# <a name="contact"></a>Contato

O elemento **Contact** representa um item de contato no repositório do Exchange. 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 **ContactItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo MIME (Multipurpose Internet Mail Extensions) nativo de um objeto representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto de itens do repositório do Exchange e objetos de resposta.  <br/> |
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
|[Propriedadeinternetmessageheaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e a hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e a hora em que um determinado item da caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos Response associados a um item no repositório do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e a hora em que o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete foi definido para um item no repositório do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha CC. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários CC.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição usada para o conteúdo da linha para. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição de destinatários.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível. Essa propriedade é somente leitura.  <br/> |
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
|[FileAs](fileas.md) <br/> |Representa como um contato é arquivado na pasta contatos.  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |Define como construir o que é exibido para um contato.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Define o nome de exibição de um contato.  <br/> |
|[GivenName](givenname.md) <br/> |Contém o nome fornecido de um contato.  <br/> |
|[Iniciais](initials.md) <br/> |Representa as iniciais de um contato.  <br/> |
|[MiddleName](middlename.md) <br/> |Representa o nome do meio de um contato.  <br/> |
|[Apelido](nickname.md) <br/> |Representa o apelido de um contato.  <br/> |
|[CompleteName](completename.md) <br/> |Representa o nome completo de um contato.  <br/> |
|[CompanyName](companyname.md) <br/> |Representa o nome da empresa que está associada a um contato.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Representa uma coleção de endereços de email de um contato.  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contém uma coleção de endereços físicos associados a um contato.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Representa uma coleção de números de telefone de um contato.  <br/> |
|[AssistantName](assistantname.md) <br/> |Representa um assistente para um contato.  <br/> |
|[Aniversário](birthday.md) <br/> |Representa a data de nascimento de um contato.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Representa a Home Page (endereço da Web) do contato.  <br/> |
|[Filhos](children.md) <br/> |Contém os nomes dos filhos de um contato.  <br/> |
|[Companies](companies.md) <br/> |Representa a coleção de empresas que estão associadas a um contato.  <br/> |
|[Contato](contactsource.md) <br/> |Descreve se o contato está localizado no repositório do Exchange ou no serviço de diretório do Active Directory.  <br/> |
|[Departamento](department.md) <br/> |Representa o departamento do contato no trabalho.  <br/> |
|[Várias](generation.md) <br/> |Representa uma abreviatura de geração que segue o nome completo de um contato.  <br/> |
|[Imendereços](imaddresses.md) <br/> |Representa uma coleção de endereços de mensagens instantâneas de um contato.  <br/> |
|[JobTitle](jobtitle.md) <br/> |Representa o cargo de um contato.  <br/> |
|[Manager](manager.md) <br/> |Representa o gerente de um contato.  <br/> |
|[Mileage](mileage.md) <br/> |Representa a quilometragem de um item de contato.  <br/> |
|[OfficeLocation](officelocation.md) <br/> |Representa o local do escritório de um contato.  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |Representa os tipos de exibição de endereços físicos.  <br/> |
|[Profissão](profession.md) <br/> |Representa a profissão de um contato.  <br/> |
|[Maridoname](spousename.md) <br/> |Representa o nome do cônjuge/parceiro de um contato.  <br/> |
|[Sobrenome](surname.md) <br/> |Representa o sobrenome de um contato.  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |Contém o aniversário de casamento de um contato.  <br/> |
|[HasPicture](haspicture.md) <br/> |Indica se o item de contato tem um anexo de arquivo que representa a imagem do contato.  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |Contém o nome completo de um contato, incluindo o nome e o sobrenome, grafo foneticamente.  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |Contém o primeiro nome de um contato, escrito foneticamente.  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |Contém o sobrenome de um contato, escrito foneticamente.  <br/> |
|[Alias](alias.md) <br/> |Contém o alias de email de um contato.  <br/> |
|[Observações (contato)](notes-contact.md) <br/> |Contém informações de contato suplementares.  <br/> |
|[Foto](photo.md) <br/> |Contém um valor que codifica a foto de um contato.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Contém um valor que codifica o certificado SMIME de um contato.  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |Contém um valor que codifica o certificado do Microsoft Exchange de um contato.  <br/> |
|[Directoryid](directoryid.md) <br/> |Contém a ID de diretório de um contato.  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |Contém informações SMTP que identificam a caixa de correio do gerente do contato.  <br/> |
|[DirectReports](directreports.md) <br/> |Contém informações SMTP que identificam os subordinados diretos de um contato.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário adjacentes a um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que entram em conflito com um horário de reunião  <br/> |
|[Create (issync)](create-itemsync.md) <br/> |Identifica uma única pasta a ser criada no armazenamento do cliente local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange anexado a outro item do Exchange.  <br/> |
|[Itens](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
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


[Criando contatos (serviços Web do Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Atualizando contatos](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Excluindo contatos](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

