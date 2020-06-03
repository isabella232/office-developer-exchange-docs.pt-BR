---
title: Propriedades e propriedades estendidas no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Descubra como você pode definir e acessar propriedades em itens e pastas usando o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 0891cf6d6dddf74518fbbc8efbaebdd8eb0c706b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459332"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Propriedades e propriedades estendidas no EWS no Exchange

Descubra como você pode definir e acessar propriedades em itens e pastas usando o EWS no Exchange.
  
Uma caixa de correio do Exchange contém um grande número de itens, incluindo mensagens de email, compromissos, reuniões e assim por diante. Esses itens são compostos de propriedades; as propriedades descrevem os itens. Você pode usar as propriedades do item para executar uma [pesquisa](search-and-ews-in-exchange.md), [sincronizar alterações de item](mailbox-synchronization-and-ews-in-exchange.md)e [criar tipos de propriedades personalizadas](https://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a). Este artigo fornece uma visão geral das propriedades e como você pode trabalhar com propriedades em seu aplicativo.
  
## <a name="exchange-item-properties"></a>Propriedades de item do Exchange
<a name="ItemsAreProperties"> </a>

Itens e pastas no Exchange são essencialmente linhas em tabelas. A propriedade principal que identifica um item ou pasta é seu [identificador de EWS](ews-identifiers-in-exchange.md). Embora existam outras propriedades relacionadas ao identificador no banco de dados do Exchange, para o EWS, o identificador EWS atua como a chave primária para a coleção de propriedades que descreve um item. A propriedade do identificador EWS contém duas partes:
  
- Uma propriedade [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ou [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) que identifica o item 
    
- Uma propriedade **ChangeKey** que contém informações de estado sobre se um item ou pasta foi alterado 
    
Todos os itens em uma caixa de correio são armazenados no mesmo banco de dados do Exchange e usam o mesmo esquema de banco de dados. Os itens são diferenciados por uma combinação [da propriedade ItemProperty](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) , restrições de propriedade e as camadas de lógica de negócios que afetam o modo como são gerenciadas no repositório do Exchange. A tabela 1 mostra como as propriedades são aplicadas em diferentes tipos de item; Neste exemplo, itens de email e compromisso. Ambos os itens têm um valor para a propriedade [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) . Mas Observe que a propriedade [IsAllDayEvent](https://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) não está definida no item de email, e a propriedade **IsReadReceiptRequested** não está definida no compromisso. Felizmente, você não precisa saber quais propriedades são aplicáveis a cada classe de item; O EWS cuida disso para você. 
  
**Tabela 1. Comparação de propriedades de compromisso e email**

|**Tipo de item**|**Classe de item**|**Assunto**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|Email  <br/> |IPM. Observação  <br/> |Relatório de status: Project X Complete  <br/> |VAZIO  <br/> |verdadeiro  <br/> |
|Compromisso  <br/> |IPM. Compromisso  <br/> |Reunião da empresa contoso  <br/> |falso  <br/> |VAZIO  <br/> |
   
O esquema EWS oferece suporte a várias das restrições gerenciadas pelo banco de dados do Exchange e pelas camadas de lógica de negócios entre o EWS e o banco de dados do Exchange. O esquema EWS aplica um conjunto de propriedades definido para cada tipo de item. Estes são os itens de banco de dados do Exchange fortemente tipados fornecidos pelo EWS: 
  
- Mensagens de email
    
- Compromissos
    
- Contatos
    
- Listas de distribuição
    
- Mensagens de reunião
    
- Solicitações de reunião
    
- Respostas de reunião
    
- Cancelamentos de reunião
    
- Tarefas
    
- Itens post
    
Os itens genéricos são retornados pelo EWS como mensagens de email. A API gerenciada do EWS implementa todos esses tipos de item.
  
> [!NOTE]
> Os objetos Response são enviados pelo cliente para o servidor em resposta a itens recebidos de outras pessoas. Eles não existem no banco de dados do Exchange. 
  
## <a name="what-are-properties-in-ews"></a>O que são propriedades no EWS?
<a name="WhatAreEWSProperties"> </a>

O esquema EWS descreve os dados enviados entre um cliente EWS e o Exchange. Uma grande parte do esquema descreve as propriedades de item e pasta que você pode acessar no banco de dados do Exchange. O esquema EWS descreve a representação XML das propriedades do banco de dados do Exchange que estão disponíveis para seu aplicativo. As propriedades reais, em termos de quais propriedades estão disponíveis, qual forma eles levam, e os valores que eles retornam, variam com base no que você está tentando fazer. Por exemplo, a propriedade **Body** retornará somente os primeiros 512 caracteres em uma operação **FindItem** , mas a operação **GetItem** retornará o texto completo do item. Embora a maioria das propriedades seja configurável e seja recuperável, algumas propriedades são definidas apenas pelo Exchange. Cada propriedade existe no esquema em um formato XML que reflete a propriedade como armazenada no banco de dados do Exchange, ou é calculada das propriedades armazenadas no banco de dados do Exchange. A propriedade **Subject** é um exemplo de uma propriedade settable; a propriedade **UnreadCount** em uma pasta é um exemplo de uma propriedade computada. Um conjunto principal de propriedades é comum para os principais tipos de item. 
  
Os seguintes fatores determinam o conjunto de propriedades que seu aplicativo obtém do Exchange: 
  
- A operação que seu aplicativo está chamando
    
- A forma resposta base
    
- O tipo de item
    
- Os caminhos de propriedade especificados
    
É importante entender como esses fatores diferentes afetam os dados que você pode acessar. Assim como ocorre com o exemplo da propriedade **Body** mencionada anteriormente, algumas informações estão condicionalmente disponíveis, dependendo de vários fatores. A compreensão desses fatores pode poupar tempo, ajudando você a escolher as opções corretas para acessar as informações desejadas. Para descobrir quais propriedades estão acessíveis, você precisará testar esses fatores para determinar como acessar as propriedades de que seu aplicativo precisa. Esta seção descreve como esses fatores diferentes afetam quais propriedades são retornadas nas respostas do EWS. 
  
### <a name="ews-response-shapes"></a>Formas de resposta do EWS

O Exchange armazena muitas informações sobre itens. Às vezes, seu aplicativo não precisa de todas essas informações e, em muitos casos, é melhor não obter tudo. [Formas de resposta do EWS](property-sets-and-response-shapes-in-ews-in-exchange.md), também chamadas de formas de propriedade, indicam quais propriedades são retornadas do servidor. O elemento principal da forma de resposta é a forma base. Uma forma base é um conjunto de propriedades predefinidos padrão para itens fortemente tipados. O equivalente da API gerenciada do EWS da forma base é o [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx). O EWS inclui três formas de resposta padrão.
  
**Tabela 2. Formas de resposta padrão**

|**Nome da forma de resposta padrão**|**Equivalente à API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|
|IdOnly  <br/> |Valor BasePropertySet. IdOnly  <br/> |Somente o identificador de EWS e a chave de alteração são retornados. A menos que o cliente use todas as propriedades retornadas por propriedade ou forma padrão, use a forma IdOnly e especifique propriedades adicionais usando o caminho de propriedade definido na classe **PropertySet** . A maioria dos aplicativos deve usar a forma de resposta IdOnly com propriedades adicionais especificadas. Isso reduz a quantidade de dados não usados solicitados por clientes.  <br/> |
|Padrão  <br/> |N/A  <br/> |Um conjunto de propriedades padrão para o tipo de item. Use essa forma de resposta somente se o aplicativo usar todas as propriedades.  <br/> |
|Propriedades  <br/> |Valor BasePropertySet. FirstClassProperties  <br/> |Um conjunto maior de propriedades do que a forma padrão. Embora o nome detenha, essa opção não retorna todas as propriedades em um item. Essa propriedade Set retorna as propriedades que os aplicativos cliente usam com mais frequência. Se você precisar de propriedades adicionais, poderá solicitá-las por seu caminho de propriedade.  <br/> Se o aplicativo não usar todas as propriedades retornadas com esta forma de resposta, use a forma de resposta IdOnly com propriedades adicionais especificadas.  <br/> |
   
Muitas operações do EWS retornam itens e suas propriedades. Independentemente das formas de resposta que você especificar, operações diferentes podem retornar diferentes conjuntos de propriedades. Diferentes tipos de item também retornam propriedades diferentes, dependendo da operação e da forma de resposta especificada. As operações a seguir usam formas de resposta para identificar quais propriedades retornar.
  
**Tabela 3. Operações que usam formas de resposta**

|**Operação do EWS**|**Método de API gerenciada do EWS**|
|:-----|:-----|
|[GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[Método ExchangeService. GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Método Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Método item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[Método ExchangeService. FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Método Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Método Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](https://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |Não implementado.  <br/> |
|[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[Método ExchangeService. ResolveNames](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[Método ExchangeService. SearchMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. BeginSearchMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Método ExchangeService. SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Método ExchangeService. SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
As formas de propriedade são uma maneira rudimentar de identificar as propriedades que você deseja que seu aplicativo retorne. Às vezes, no entanto, seu aplicativo precisa de um conjunto mais refinado de propriedades específicas. Para isso, você pode usar o caminho da propriedade.
  
### <a name="choose-properties-by-their-property-path"></a>Escolha Propriedades por seu caminho de propriedade

Um caminho de Propriedade do EWS é Metadata que é usado para identificar as propriedades em uma solicitação ou resposta. 
  
**Tabela 4. Tipos de caminho de propriedade**

|**Tipo de caminho de propriedade**|**Tipo de esquema**|**Implementação da API gerenciada do EWS**|**Descrição**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |Tipos que herdam de [ServiceObjectSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx).  <br/> |O caminho de propriedade mais comum. Os caminhos da propriedade FieldUri são especificados em um objeto **PropertySet** na API gerenciada do EWS. A maioria das propriedades do EWS pode ser especificada pelo caminho da propriedade FieldUri. Isso é descrito pelo UnindexedFieldURIType no esquema do EWS.  <br/> O XML do caminho da propriedade FieldUri tem a seguinte aparência:  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```Este caminho de propriedade é o equivalente de doschema. Subject na API gerenciada do EWS.  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |Tipos que herdam de [doschema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx).  <br/> |Identifica as propriedades do dicionário que exigem um índice de propriedade para especificar o valor a ser retornado. Use este caminho quando uma propriedade puder ter mais de um valor. Isso é descrito pela propriedade **DictionaryURIType** no esquema do EWS. Os caminhos da propriedade **DictionaryURIType** são especificados em um objeto **PropertySet** na API gerenciada do EWS.  <br/> O XML do caminho da propriedade IndexedFieldUri tem a seguinte aparência:  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Identifica uma definição de propriedade estendida que identifica Propriedades personalizadas ou não esquematizado em itens.  <br/> O XML do caminho da propriedade ExtendedFieldUri tem a seguinte aparência:  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[Myresponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |Especifica as propriedades que estão associadas a um erro em uma resposta do EWS. Isso é descrito pelo tipo **ExceptionPropertyURIType** no esquema do EWS. Isso ocorre apenas no elemento **MessageXml** de respostas de erro que ocorrem quando você está trabalhando com padrões de recorrência do calendário.  <br/> |
   
Como prática recomendada, quando você solicita Propriedades, use a forma base IdOnly ([BasePropertySet. IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) na API gerenciada do EWS) e, em seguida, solicite apenas as propriedades que seu aplicativo precisa, especificando os caminhos de propriedade. 
  
### <a name="schematized-properties"></a>Propriedades esquematizado

A maioria das propriedades que seu cliente EWS precisa são descritas pelo esquema do EWS. A pasta principal e as definições de tipo de item, que contêm as definições de propriedade, são encontradas no esquema Types. xsd. Os tipos de esquema a seguir contêm as definições de propriedade para a maioria dos objetos que você pode usar.
  
**Tabela 5. Tipos de esquema que contêm definições de propriedade**

|**Tipo de esquema do EWS**|**Equivalência de tipo de API gerenciada do EWS**|**Define o...**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[Classe de item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades de tipo de item base. Este tipo pode ser criado a partir de um cliente, mas nunca é retornado pelo Exchange. O Exchange retorna um objeto MessageType para todos os objetos genéricos.  <br/> |
|**MessageType** <br/> |[Classe EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |Propriedade de objeto da mensagem de email definida e o conjunto de propriedades para todos os objetos genéricos.  <br/> |
|**CalendarItemType** <br/> |[Classe de compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do item de calendário; Isso inclui compromissos simples e recorrentes.  <br/> |
|**ContactItemType** <br/> |[Classe de contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades do item de contato.  <br/> |
|**DistributionListType** <br/> |[Classe de contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades de lista de distribuição pessoal.  <br/> |
|**MeetingMessageType** <br/> |[Classe MeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo de mensagem de reunião definida.  <br/> |
|**MeetingRequestMessageType** <br/> |[Classe MeetingRequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |Definição da propriedade de tipo de solicitação de reunião.  <br/> |
|**MeetingResponseMessageType** <br/> |[Classe MeetingResponse](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo de resposta da reunião definida.  <br/> |
|**MeetingCancellationMessageType** <br/> |[Classe MeetingCancellation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |Definição da propriedade de tipo de cancelamento de reunião.  <br/> |
|**TaskType** <br/> |[Classe de tarefa](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo de tarefa definida.  <br/> |
|**PostItem** <br/> |[Classe PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Propriedade do tipo PostItem definida.  <br/> |
|**FolderType** <br/> |[Classe Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |Conjunto de propriedades de tipo de pasta.  <br/> |
|**CalendarFolderType** <br/> |[Classe CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo SearchFolder definida.  <br/> |
|**ContactsFolderType** <br/> |[Classe ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo ContactsFolder definida.  <br/> |
|**SearchFolderType** <br/> |[Classe SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo SearchFolder definida.  <br/> |
|**TasksFolderType** <br/> |[Classe TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |Propriedade de tipo TasksFolder definida.  <br/> |
|**Userconfigurationtype** <br/> |[Classe userconfiguration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |Propriedade do tipo userconfiguration definida.  <br/> |
   
Enquanto as propriedades no esquema do EWS são suficientes para muitos aplicativos, não é possível implementar alguns cenários usando apenas o que está descrito no esquema. Para esses cenários, você pode estender Propriedades. 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>Propriedades estendidas (aka Propriedades não-esquematizado)

As propriedades estendidas permitem que você crie propriedades personalizadas, que dão acesso a propriedades em itens e pastas no armazenamento do Exchange que não estão definidos no esquema do EWS. Você pode usá-los para acessar as propriedades de item e de pasta MAPI nativo no banco de dados do Exchange. Você pode usar propriedades estendidas para acessar todas as propriedades de esquematizado, pois nas capas, essas propriedades esquematizado não são mais do que as propriedades MAPI no banco de dados do Exchange. 
  
O tipo de esquema PathToExtendedFieldType, localizado no esquema Types. xsd, define o XML que representa uma propriedade estendida. Este tipo de esquema define o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) em instâncias XML; em outras palavras, define o XML que é enviado entre o serviço e o cliente. O tipo de esquema ExtendedPropertyType define o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) e o valor ou a matriz de valores que uma propriedade estendida contém. A tabela a seguir mostra o mapeamento aproximado do XML da propriedade estendida e como ele é implementado em itens na API gerenciada do EWS. 
  
**Tabela 6. XML de propriedade estendida conforme implementado na API gerenciada do EWS**

|**Implementação da API gerenciada do EWS**|**O que ele contém**|**O que ele mapeia para**|
|:-----|:-----|:-----|
|[Propriedade Item. ExtendedProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |Uma coleção de propriedades estendidas em um item.  <br/> |Uma ou mais instâncias de propriedades estendidas em um item.  <br/> |
|[Classe estendiproperty](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |A definição e os valores da propriedade estendida.  <br/> |O tipo de esquema ExtendedPropertyType.  <br/> |
|[Classe ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |Uma definição de propriedade estendida.  <br/> |O tipo de esquema PathToExtendedFieldType.  <br/> |
   
Se quiser saber mais sobre como usar propriedades estendidas em seu aplicativo, você pode explorar os exemplos de código a seguir: 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013: provisionar cabeçalhos X personalizados de forma programática](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013: acessar uma propriedade por sua marca de propriedade](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013: acessar uma propriedade nomeada pelo identificador](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013: acessar uma propriedade nomeada pelo nome](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013: acessar uma propriedade por GUID e nome de conjunto de propriedades](https://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013: criar propriedades estendidas personalizadas de forma programática](https://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Provisionar cabeçalhos x usando o EWS no Exchange](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [Erros relacionados à propriedade do EWS](ews-property-related-errors.md)
    
## <a name="see-also"></a>Confira também


- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

