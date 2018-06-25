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
description: O elemento de contato representa um item de contato no armazenamento do Exchange.
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751441"
---
# <a name="contact"></a>Contato

O elemento **Contatos** representa um item de contato no armazenamento do Exchange. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Contém o fluxo de email extensões MIME (Multipurpose Internet) nativo de um objeto que é representado no formato base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém o item ou a pasta.  <br/> |
|[ItemClass](itemclass.md) <br/> |Representa a classe de mensagem de um item.  <br/> |
|[Assunto](subject.md) <br/> |Representa o assunto para armazenar itens do Exchange e objetos de resposta.  <br/> |
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
|[IsFromMe](isfromme.md) <br/> |Indica se um usuário enviada a um item para si mesmo ou por conta própria.  <br/> |
|[IsResend](isresend.md) <br/> |Indica se o item anteriormente foi enviado.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Indica se o item foi modificado.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Representa a data e hora em que um item em uma caixa de correio foi enviado.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Representa a data e hora em que um determinado item na caixa de correio foi criado.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contém uma coleção de todos os objetos de resposta que estão associados um item no armazenamento do Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Representa a data e hora quando o evento ocorre. Isso é usado pelo elemento [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) para determinar quando o lembrete é exibido.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Indica se um lembrete tiver sido definido para um item no armazenamento do Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Representa o número de minutos antes de um evento, quando um lembrete é exibido.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da linha Cc. Esta é a cadeia de caracteres concatenada de todos os nomes de exibição destinatários Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Representa a cadeia de caracteres de exibição que é usada para o conteúdo da linha para. Esta é a cadeia de caracteres concatenada de todos os aos nomes de exibição do destinatário.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Representa uma propriedade que é definida como **true** se um item tem pelo menos um anexo visível. Esta propriedade é somente leitura.  <br/> |
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
|[FileAs](fileas.md) <br/> |Representa como um contato é arquivado na pasta Contatos.  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |Define como construir o que é exibido para um contato.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Define o nome de exibição de um contato.  <br/> |
|[GivenName](givenname.md) <br/> |Contém o nome do contato.  <br/> |
|[Iniciais](initials.md) <br/> |Representa as iniciais de um contato.  <br/> |
|[MiddleName](middlename.md) <br/> |Representa o nome do meio de um contato.  <br/> |
|[Apelido](nickname.md) <br/> |Representa o apelido de um contato.  <br/> |
|[CompleteName](completename.md) <br/> |Representa o nome completo de um contato.  <br/> |
|[CompanyName](companyname.md) <br/> |Representa o nome da empresa que é associado a um contato.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Representa uma coleção de endereços de email de um contato.  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |Contém uma coleção de endereços físicos que estão associados um contato.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Representa uma coleção de números de telefone de um contato.  <br/> |
|[AssistantName](assistantname.md) <br/> |Representa um Assistente para um contato.  <br/> |
|[Aniversário](birthday.md) <br/> |Representa a data de nascimento de um contato.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Representa a Home page (endereço da Web) para o contato.  <br/> |
|[Filhos](children.md) <br/> |Contém os nomes dos filhos de um contato.  <br/> |
|[Empresas](companies.md) <br/> |Representa a coleção de empresas que estão associados um contato.  <br/> |
|[ContactSource](contactsource.md) <br/> |Descreve como se o contato está localizado no armazenamento do Exchange ou o serviço de diretório do Active Directory.  <br/> |
|[Departamento](department.md) <br/> |Representa o departamento do contato no trabalho.  <br/> |
|[Geração](generation.md) <br/> |Representa uma abreviatura gerações que segue o nome completo de um contato.  <br/> |
|[ImAddresses](imaddresses.md) <br/> |Representa uma coleção de endereços de mensagens instantâneas de um contato.  <br/> |
|[JobTitle](jobtitle.md) <br/> |Representa o cargo de um contato.  <br/> |
|[Manager](manager.md) <br/> |Representa o gerente do contato.  <br/> |
|[Mileage](mileage.md) <br/> |Representa mileage para um item de contato.  <br/> |
|[Local do escritório](officelocation.md) <br/> |Representa o local do escritório de um contato.  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |Representa os tipos de exibição para endereços físicos.  <br/> |
|[Profession](profession.md) <br/> |Representa o profession de um contato.  <br/> |
|[NomeDoCônjuge](spousename.md) <br/> |Representa o nome do cônjuge um contato.  <br/> |
|[Sobrenome](surname.md) <br/> |Representa o sobrenome de um contato.  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |Contém o aniversário de chá de um contato.  <br/> |
|[HasPicture](haspicture.md) <br/> |Indica se o item de contato tem um anexo de arquivo que representa a imagem do contato.  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |Contém o nome completo de um contato, incluindo o nome e sobrenome, escrito foneticamente.  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |Contém o nome de um contato, escritas foneticamente.  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |Contém o sobrenome de um contato, escritas foneticamente.  <br/> |
|[Alias](alias.md) <br/> |Contém o alias de email de um contato.  <br/> |
|[Notas (contato)](notes-contact.md) <br/> |Contém informações de contato suplementares.  <br/> |
|[Foto](photo.md) <br/> |Contém um valor que codifica a foto de um contato.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Contém um valor que codifica o certificado SMIME de um contato.  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |Contém um valor que codifica o certificado do Microsoft Exchange de um contato.  <br/> |
|[DirectoryId](directoryid.md) <br/> |Contém a ID do diretório de um contato.  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |Contém informações de SMTP que identifica a caixa de correio do gerente do contato.  <br/> |
|[DirectReports](directreports.md) <br/> |Contém informações de SMTP que identifica os funcionários subordinados de um contato.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Nome do elemento**|**Descrição**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Descreve todos os itens de calendário que são adjacentes para um horário de reunião.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item ou pasta durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Identifica todos os itens que estão em conflito com um tempo de reunião  <br/> |
|[Criar (ItemSync)](create-itemsync.md) <br/> |Identifica uma única pasta para criar no repositório de cliente local.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Representa um item do Exchange que está anexado a outro item do Exchange.  <br/> |
|[Items](items.md) <br/> |Contém uma matriz de itens.  <br/> |
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[Resolução](resolution.md) <br/> |Contém uma única entidade resolvida.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Atualização (ItemSync)](update-itemsync.md) <br/> |Identifica um único item a ser atualizado no repositório de cliente local.  <br/> |
   
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
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criação de contatos (serviços Web do Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Atualizar contatos](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Excluindo contatos](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

