---
title: Propriedades e propriedades estendidas em EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Descubra como você pode definir e acessar propriedades em pastas e itens usando o EWS no Exchange.
ms.openlocfilehash: 0c01d9bd21cbef0a3536c8dbd85e192199b7b8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750950"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Propriedades e propriedades estendidas em EWS no Exchange

Descubra como você pode definir e acessar propriedades em pastas e itens usando o EWS no Exchange.
  
Uma caixa de correio do Exchange contém um grande número de itens, incluindo mensagens de email, compromissos, reuniões e assim por diante. Os itens são compostos de propriedades; as propriedades descrevem os itens. Você pode usar as propriedades do item para executar uma [pesquisa](search-and-ews-in-exchange.md), [sincronizar as alterações de item](mailbox-synchronization-and-ews-in-exchange.md)e [criar tipos de propriedade personalizada](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). Este artigo fornece uma visão geral das propriedades e como você pode trabalhar com propriedades em seu aplicativo.
  
## <a name="exchange-item-properties"></a>Propriedades de item do Exchange
<a name="ItemsAreProperties"> </a>

Itens e pastas do Exchange são basicamente linhas nas tabelas. A propriedade principal que identifica um item ou pasta é seu [identificador do EWS](ews-identifiers-in-exchange.md). Embora existam outras propriedades relacionadas ao identificador no banco de dados Exchange, para o EWS, o identificador do EWS atua como a chave primária para a coleção de propriedades que descrevem um item. A propriedade de identificador do EWS contém duas partes:
  
- Uma propriedade [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ou [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) que identifica o item 
    
- Uma propriedade **ChangeKey** que contém informações com informações de estado sobre se um item ou pasta mudou 
    
Todos os itens em uma caixa de correio são armazenados no mesmo banco de dados do Exchange e usam o mesmo esquema de banco de dados. Itens são diferenciados por uma combinação das camadas de lógica de negócios que afetam o modo como eles são gerenciados no Exchange, restrições de propriedade e a propriedade [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) armazenar. A tabela 1 mostra como as propriedades são aplicadas nos tipos de itens diferentes; em itens neste exemplo, email e compromisso. Ambos os itens tiverem um valor para a propriedade [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Mas, observe que a propriedade [IsAllDayEvent](http://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) não estiver definida no item de email e a propriedade **IsReadReceiptRequested** não estiver definida no compromisso. Felizmente, você não precisa saber quais propriedades são aplicáveis para cada classe de item; EWS manipula isso para você. 
  
**Tabela 1. Comparação das propriedades de compromisso e email**

|**Tipo de item**|**Classe de item**|**Assunto**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|Email  <br/> |IPM. Observação  <br/> |Relatório de status: conclusão do projeto X  <br/> |NULL  <br/> |true  <br/> |
|Compromisso  <br/> |IPM.Appointment  <br/> |Reunião da empresa Contoso  <br/> |false  <br/> |NULL  <br/> |
   
O esquema do EWS oferece suporte a várias das restrições gerenciadas pelo banco de dados do Exchange e as camadas de lógica de negócios entre EWS e o banco de dados do Exchange. O esquema do EWS aplica um definido um conjunto de propriedades para cada tipo de item. Estes são os itens de banco de dados Exchange fortemente tipadas fornecidos pelo EWS: 
  
- Mensagens de email
    
- Compromissos
    
- Contatos
    
- Listas de distribuição
    
- Mensagens de reunião
    
- Solicitações de reunião
    
- Respostas de reunião
    
- Cancelamentos de reunião
    
- Tarefas
    
- Postar itens
    
Itens genéricos são retornados pelo EWS como mensagens de email. A API gerenciada de EWS implementa todos esses tipos de item.
  
> [!NOTE]
> Objetos de resposta serão enviados somente pelo cliente para o servidor em resposta a itens recebidos de outras pessoas. Eles não existem no banco de dados do Exchange. 
  
## <a name="what-are-properties-in-ews"></a>Cite propriedades no EWS.
<a name="WhatAreEWSProperties"> </a>

O esquema do EWS descreve os dados que são enviados entre um cliente do EWS e Exchange. Uma grande parte do esquema descreve as propriedades de item e a pasta que você pode acessar o banco de dados do Exchange. O esquema do EWS descreve a representação XML das propriedades de banco de dados do Exchange que estão disponíveis para seu aplicativo. As propriedades reais, em termos de quais propriedades estão disponíveis, o que formam eles take e os valores de retorno, variar com base nas quais você está tentando fazer. Por exemplo, a propriedade **Body** retornará apenas os primeiros 512 caracteres em uma operação **FindItem** , mas a operação **GetItem** retorna o texto completo do item. Embora a maioria das propriedades são configuráveis e recuperáveis, algumas propriedades só são definidas pelo Exchange. Cada propriedade existe no esquema em um formato XML que um reflete a propriedade conforme ele está armazenado no banco de dados do Exchange ou é computado de propriedades armazenadas no banco de dados do Exchange. A propriedade **Subject** é um exemplo de uma propriedade configurável; a propriedade **UnreadCount** em uma pasta é um exemplo de uma propriedade calculada. Um conjunto básico de propriedades são comuns para os tipos de item principal. 
  
Os seguintes fatores determinarão que a propriedade definida que seu aplicativo obtém do Exchange: 
  
- A operação que está chamando o seu aplicativo
    
- A forma de resposta de base
    
- O tipo de item
    
- Os caminhos de propriedade especificado
    
É importante compreender como esses fatores diferentes afetam os dados que você pode acessar. Como o exemplo da propriedade **corpo** mencionado anteriormente, algumas informações estão condicionalmente disponíveis, dependendo de diversos fatores. Noções básicas sobre esses fatores podem economizar tempo, ajudando você escolher as opções corretas para acessar as informações que você deseja. Para descobrir quais propriedades podem ser acessadas, você precisará testar esses fatores para determinar como acessar as propriedades suas necessidades de aplicativo. Esta seção descreve como esses fatores diferentes afetam a quais propriedades são retornadas em respostas do EWS. 
  
### <a name="ews-response-shapes"></a>Formas de resposta EWS

O Exchange armazena muita informação sobre os itens. Às vezes, seu aplicativo não precisa todas essas informações e em muitos casos, é melhor não fazer tudo. [Formas de resposta do EWS](property-sets-and-response-shapes-in-ews-in-exchange.md), também chamado de formas de propriedade, indicar quais propriedades são retornadas do servidor. O elemento de núcleo da forma resposta é a forma de base. Uma forma de base é um recipiente de propriedades predefinido de padrão para itens fortemente tipadas. O equivalente do EWS Managed API da forma base é o [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). EWS inclui três formas de resposta padrão.
  
**Tabela 2. Formas de resposta padrão**

|**Nome da forma resposta padrão**|**API gerenciada de EWS equivalente**|**Descrição**|
|:-----|:-----|:-----|
|IdOnly  <br/> |Valor de BasePropertySet.IdOnly  <br/> |Somente o identificador do EWS e alterar chave são retornadas. A menos que o cliente usa todas as propriedades retornadas pela forma AllProperties ou padrão, use a forma de IdOnly e especificar propriedades adicionais usando o caminho de propriedade definido na classe **PropertySet** . A maioria dos aplicativos deve usar a forma de resposta IdOnly com propriedades adicionais especificadas. Isso reduz a quantidade de dados não utilizados que são solicitados pelos clientes.  <br/> |
|Default  <br/> |N/A  <br/> |Um conjunto de propriedades padrão do tipo de item. Só use esta forma de resposta se seu aplicativo usa todas as propriedades.  <br/> |
|AllProperties  <br/> |Valor de BasePropertySet.FirstClassProperties  <br/> |Um conjunto maior de propriedades que a forma padrão. Embora o nome implica-lo, essa opção não retorna todas as propriedades em um item. Definir essa propriedade retorna as propriedades que aplicativos clientes usam com mais frequência. Se você precisar propriedades adicionais, você poderá solicitá-los pelo seu caminho de propriedade.  <br/> Se seu aplicativo não usa todas as propriedades retornadas com esta forma de resposta, use a forma de resposta IdOnly com propriedades adicionais especificadas.  <br/> |
   
Muitas operações de EWS retornam itens e suas propriedades. As formas de resposta que você especificar, independentemente de operações diferentes podem retornar conjuntos de propriedade diferentes. Tipos de itens diferentes também retornam propriedades diferentes, dependendo da operação e a forma de resposta especificado. As seguintes operações usam formas de resposta para identificar quais propriedades para retornar.
  
**Tabela 3. Operações que usam a formas de resposta**

|**Operação do EWS**|**Método API gerenciada de EWS**|
|:-----|:-----|
|[GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Método ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Método Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Método Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Método ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Método Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Método Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Não foi implementado.  <br/> |
|[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Método ExchangeService.ResolveNames](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Método ExchangeService.SearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BeginSearchMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Método ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Método ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
As formas de propriedade são um, rudimentar maneira de identificar as propriedades que você deseja que o aplicativo para retornar. Às vezes, no entanto, o seu aplicativo precisa um conjunto mais refinado das propriedades específicas. Para isso, você pode usar o caminho de propriedade.
  
### <a name="choose-properties-by-their-property-path"></a>Escolha Propriedades pelo seu caminho de propriedade

Um caminho de propriedade do EWS é os metadados que é usado para identificar as propriedades em uma solicitação ou resposta. 
  
**Tabela 4. Tipos de caminho de propriedade**

|**Tipo de caminho de propriedade**|**Tipo de esquema**|**Implementação da API gerenciada de EWS**|**Descrição**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |Tipos que herdam [ServiceObjectSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |O caminho da propriedade mais comuns. Caminhos de propriedade FieldUri são especificados em um objeto **PropertySet** na API gerenciada do EWS. A maioria das propriedades do EWS podem ser especificadas pelo caminho FieldUri propriedade. Isso é descrito pelo UnindexedFieldURIType no esquema do EWS.  <br/> O caminho da propriedade FieldUri XML tem esta aparência:  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Este caminho de propriedade é o equivalente do ItemSchema.Subject na API gerenciada do EWS.  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |Tipos que herdam [ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Identifica as propriedades de dicionário que exigem um índice de propriedade para especificar o valor a ser retornado. Use esse caminho quando uma propriedade pode ter mais de um valor. Isso é descrito pela propriedade **DictionaryURIType** no esquema do EWS. Caminhos de propriedade **DictionaryURIType** são especificados em um objeto **PropertySet** na API gerenciada do EWS.  <br/> O caminho da propriedade IndexedFieldUri XML tem esta aparência:  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Identifica uma definição de propriedade estendida que identifica as propriedades personalizadas ou não esquematizado nos itens.  <br/> O caminho da propriedade ExtendedFieldUri XML tem esta aparência:  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[ServiceResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Especifica as propriedades que estão associadas um erro em uma resposta EWS. Isso é descrito pelo tipo **ExceptionPropertyURIType** no esquema do EWS. Isso ocorre apenas no elemento **MessageXml** do respostas de erros que ocorrem quando você estiver trabalhando com os padrões de recorrência de calendário.  <br/> |
   
Como prática recomendada, ao solicitar propriedades, use a forma de base IdOnly ([BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) na API gerenciada do EWS) e, em seguida, solicitar apenas as propriedades de seu aplicativo precisa especificando os caminhos de propriedade. 
  
### <a name="schematized-properties"></a>Propriedades esquematizadas

A maioria das propriedades que precisa de seu cliente EWS é descrita pelo esquema do EWS. A pasta principal e definições de tipo de item, que contêm as definições de propriedade, são encontradas no esquema types.xsd. Os tipos de esquema a seguir contêm as definições de propriedade para a maioria dos objetos que podem ser usados.
  
**Tabela 5. Tipos de esquema que contêm as definições de propriedade**

|**Tipo de esquema EWS**|**Equivalente do tipo de API gerenciada de EWS**|**Define o …**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Classe de item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo de item base. Este tipo pode ser criado a partir de um cliente, mas nunca será retornado pelo Exchange. Exchange retorna um objeto MessageType para todos os objetos genéricos.  <br/> |
|**MessageType** <br/> |[Classe de EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do objeto de mensagem de email e a propriedade definida para todos os objetos genéricos.  <br/> |
|**CalendarItemType** <br/> |[Classe de compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Definir a propriedade de item de calendário; Isso inclui compromissos de único e recorrentes.  <br/> |
|**ContactItemType** <br/> |[Entre em contato com a classe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades de item de contato.  <br/> |
|**DistributionListType** <br/> |[Classe de ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades da lista de distribuição pessoal.  <br/> |
|**MeetingMessageType** <br/> |[Classe de MeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Defina a propriedade type de mensagem da reunião.  <br/> |
|**MeetingRequestMessageType** <br/> |[Classe de MeetingRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades de tipo de solicitação de reunião.  <br/> |
|**MeetingResponseMessageType** <br/> |[Classe MeetingResponse](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Defina a propriedade type de resposta de reunião.  <br/> |
|**MeetingCancellationMessageType** <br/> |[Classe de MeetingCancellation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Defina a propriedade type de cancelamento de reunião.  <br/> |
|**TaskType** <br/> |[Classe de tarefa](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo de tarefa.  <br/> |
|**PostItemType** <br/> |[Classe postItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo PostItem.  <br/> |
|**FolderType** <br/> |[Classe de pasta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo de pasta.  <br/> |
|**CalendarFolderType** <br/> |[Classe de CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo SearchFolder.  <br/> |
|**ContactsFolderType** <br/> |[Classe de ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo ContactsFolder.  <br/> |
|**SearchFolderType** <br/> |[Classe SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo SearchFolder.  <br/> |
|**TasksFolderType** <br/> |[Classe de TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo TasksFolder.  <br/> |
|**UserConfigurationType** <br/> |[Classe de UserConfiguration](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do tipo UserConfiguration.  <br/> |
   
Enquanto as propriedades no esquema do EWS são suficientes para muitos aplicativos, você não pode implementar alguns cenários usando apenas o que está descrito no esquema. Para esses cenários, você pode propriedades estendidas. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Propriedades estendidas (também conhecido como propriedades não esquematizado)

Propriedades estendidas permitem criar propriedades personalizadas, que fornecem acesso às propriedades de itens e pastas que não são definidas no esquema do EWS no armazenamento do Exchange. Você pode usá-los para acessar os MAPI item e pasta propriedades nativas do banco de dados do Exchange. Você pode usar propriedades estendidas para acessar todas as propriedades esquematizadas, pois nos bastidores, essas propriedades esquematizadas são nada mais que propriedades MAPI do banco de dados do Exchange. 
  
O tipo de esquema PathToExtendedFieldType, localizado no esquema types.xsd, define o XML que representa uma propriedade estendida. Esse tipo de esquema define o elemento [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) em instâncias XML; em outras palavras, ele define o XML que é enviado entre o cliente e o serviço. O tipo de esquema de ExtendedPropertyType define tanto o elemento [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) e o valor ou matriz de valores que contém uma propriedade estendida. A tabela a seguir mostra o mapeamento aproximado da propriedade estendida XML e como ela é implementada em itens o EWS Managed API. 
  
**Tabela 6. Propriedade estendida XML como implementada na API gerenciada de EWS**

|**Implementação da API gerenciada de EWS**|**O que ele contém**|**Ele mapeia para**|
|:-----|:-----|:-----|
|[Propriedade Item.ExtendedProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Uma coleção de propriedades estendidas em um item.  <br/> |Uma ou mais instâncias das propriedades estendidas em um item.  <br/> |
|[Classe de ExtendedProperty](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |A definição da propriedade estendida e valores.  <br/> |O tipo de esquema ExtendedPropertyType.  <br/> |
|[Classe de ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Uma definição de propriedade estendida.  <br/> |O tipo de esquema PathToExtendedFieldType.  <br/> |
   
Se você deseja saber mais sobre como você pode usar propriedades estendidas em seu aplicativo, você pode explorar os exemplos de código a seguir: 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013: Provisionar cabeçalhos X personalizados programaticamente](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013: Acessar uma propriedade por sua marca de propriedade](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013: Acessar uma propriedade nomeada por seu identificador](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013: Acessar uma propriedade nomeada por seu nome](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013: Acessar um nome e o GUID do conjunto de propriedade por propriedade](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013: Criar personalizados por meio de programação de propriedades estendidas](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Cabeçalhos x provisão usando o EWS no Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Erros relacionados a propriedade do EWS](ews-property-related-errors.md)
    
## <a name="see-also"></a>Confira também


- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

