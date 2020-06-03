---
title: Pastas e itens no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: Saiba mais sobre pastas e itens de caixa de correio e como a API gerenciada EWS ou o cliente EWS as representa.
localization_priority: Priority
ms.openlocfilehash: 5e206d6973d148c6f70a17a8e7891bf3de7c1533
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44455974"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Pastas e itens no EWS no Exchange

Saiba mais sobre pastas e itens de caixa de correio e como a API gerenciada EWS ou o cliente EWS as representa.
  
As pastas são o elemento de organização de uma caixa de correio do Exchange. As pastas podem conter itens de caixa de correio, como mensagens de email, contatos, compromissos, reuniões e tarefas, ou podem conter outras pastas. O Exchange inclui diferentes tipos de pastas, mas os tipos de pasta são semelhantes uns dos outros. A principal diferença entre eles é o tipo de item que eles contêm.
  
No entanto, os itens têm tipos exclusivos. Cada tipo de item tem um conjunto diferente de propriedades ou esquema para defini-lo. Neste artigo, discutiremos os tipos de pastas e itens que estão disponíveis e as diferenças entre eles.

<a name="bk_folders"> </a>

## <a name="folders"></a>Folders

Todas as pastas derivam da mesma classe base ou tipo base, a classe [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) na API gerenciada do EWS ou o tipo de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) no EWS. A figura a seguir mostra as classes da API gerenciada do EWS e os tipos de EWS. 
  
**Figura 1. Classes de pasta de API gerenciada por EWS e tipos de pasta do EWS**

![Uma ilustração que mostra as classes derivadas da classe Pasta de API Gerenciada do EWS e os tipos derivados do tipo de Pasta do EWS, todos nomeados CalendarFolder, ContactsFolder, SearchFolder e TasksFolder.](media/Ex2013_Folder_OverviewTypes.png)
  
A principal diferença entre cada uma das classes de pasta e os tipos de pasta é que você só pode criar um determinado tipo de item em cada tipo de pasta. Outra diferença é como o cliente exibe informações em uma pasta. Por exemplo, o Exchange permite que você crie compromissos na pasta calendário. Você pode mover outros tipos de itens para a pasta calendário depois de criá-los, mas o Outlook não os exibirá. O Outlook exibe apenas itens de calendário, como compromissos e reuniões na pasta calendário, [mesmo se outro tipo de item existir na pasta](folders-and-items-in-ews-in-exchange.md#bk_item). 
  
**Tabela 1. Classes de pasta de API gerenciada por EWS e tipos de pasta do EWS**

|**Classe de API gerenciada do EWS**|**Tipo de EWS**|**Valor FolderClass**|**Contém**|**Anotações**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |IPF. Observação  <br/> |Pastas ou mensagens de email.  <br/> | Esta é a classe de pasta genérica ou o tipo das seguintes pastas do EWS Managed API [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e pastas EWS [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) : <ul><li>  Raiz (sub-árvore IPM)</li><li>NonIpmSubtree</li><li>Caixa de Entrada</li><li>Itens excluídos</li><li>Rascunhos</li><li>Diário</li><li>Observações  </li><li>Enviada</li><li>Itens enviados</li><li>Pasta de mensagens</li><li>Lixo eletrônico</li><li>Caixa Postal</li></ul> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |IPF. Compromisso  <br/> |Compromissos e reuniões.  <br/> |Quando um usuário responde a uma solicitação de reunião, o compromisso é adicionado à API gerenciada do EWS [WellKnownFolderName. Calendar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou somente ao EWS [DistinguishedFolderId. CalendarFolder](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Estas são as únicas pastas que dão suporte à interação automática com solicitações de reunião e respostas.  <br/><br/>Essa classe de pasta ou tipo de pasta suporta o uso de modos de exibição de calendário para retornar compromissos e reuniões com base em uma data de início e uma data de término usando o método Folder de API gerenciada do EWS [. FindItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) e a classe [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou a operação do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) e o elemento [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |IPF. Amostra  <br/> |Contatos e listas de distribuição.  <br/> |Nenhum  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |IPF. Observação  <br/> |O conteúdo é determinado por uma restrição ou filtro. As pastas de pesquisa não têm subpastas.  <br/> |Os itens que atendem aos critérios de pesquisa não estão realmente contidos na pasta de pesquisa; em vez disso, eles estão localizados em qualquer lugar na caixa de correio.  <br/> Para garantir que as pastas de pesquisa estejam disponíveis no Outlook, crie-as na pasta localizador.  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |IPF. Tarefa  <br/> |Contém itens de trabalho para concluir.  <br/> |Nenhum  <br/> |
   
### <a name="folder-structure"></a>Estrutura de pastas

As pastas fornecem uma estrutura de caixa de correio. Isso inclui a sub-árvore IPM, conhecida como a parte superior do armazenamento de informações no EWS, onde a maioria dos usuários interagem com a caixa de correio, bem como as pastas do sistema que a maioria dos usuários nunca vê, que estão na raiz não-IPM ou na raiz do EWS. A figura a seguir mostra a estrutura de pastas de um usuário e indica quais pastas são para os itens do usuário e quais são pastas de sistema.
  
**Figura 2. Pastas de item e de sistema em uma caixa de correio**

![Uma ilustração que mostra as pastas do sistema raiz, que inclui Favoritos, Localizador, Dados de disponibilidade, Início do repositório de informações e muito mais. O Início do repositório de informações contém as pastas do usuário, que incluem Calendário, Contatos e mais.](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>Pastas conhecidas

Das pastas em uma caixa de correio, algumas são pastas especiais. Eles são equivalentes a pastas conhecidas na API gerenciada do EWS ou pastas diferenciadas no EWS. Algumas dessas pastas têm restrições no nome da pasta, onde elas estão localizadas na estrutura de pastas e se podem ser excluídas. Outras pastas "genéricas" (não especiais) não têm as mesmas restrições. É importante que você esteja familiarizado com as seguintes pastas conhecidas ou diferenciadas, pois elas são o sistema raiz, o usuário e as pastas de pesquisa e são aplicáveis à maioria das implementações. 
  
**Tabela 2. Principais pastas conhecidas e diferenciadas**

|**Nome amigável**|**Valores de **WellKnownFolderName** da API gerenciada do EWS**|**Valores do EWS **DistinguishedFolderId****|**Descrição**|
|:-----|:-----|:-----|:-----|
|Raiz (sub-árvore não-IPM)  <br/> |WellKnownFolderName. root  <br/> |DistinguishedFolderId. root  <br/> |Contém a pasta raiz de uma caixa de correio, também conhecida como subárvore não-IPM. Esta pasta não tem pai e você não pode movê-la, copiá-la, renomear ou excluí-la. Cada repositório de mensagens contém apenas uma pasta raiz.  <br/> |
|Início do repositório de informações (sub-árvore IPM)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |Contém a caixa de entrada e outras pastas de usuário.  <br/> |
|Localizador (pastas de pesquisa)  <br/> |WellKnownFolderName. SearchFolders  <br/> |DistinguishedFolderId. SearchFolders.  <br/> |Contém pastas de pesquisa que estão visíveis no Outlook.  <br/> |
   
Para obter uma lista completa dos valores da propriedade [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) da API gerenciada do EWS, consulte a enumeração [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) . Para obter uma lista completa dos valores do EWS **DistinguishedFolderId** , consulte [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx).
  
### <a name="folder-properties"></a>Propriedades de pasta

Na API gerenciada do EWS, as [Propriedades da pasta](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx) são derivadas da classe de [pasta](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) base. E no EWS, todas as pastas usam os elementos de pasta que estão disponíveis no tipo de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) . A maioria das propriedades e dos elementos relacionados à pasta é direta (ID da pasta pai, nome de exibição e assim por diante), mas alguns precisam de uma explicação um pouco mais. 
  
As seguintes advertências se aplicam à propriedade [Folder. FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) da API gerenciada do EWS ou ao elemento EWS [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) : 
  
- Se definido, o valor da propriedade ou elemento deve concordar com a classe derivada ou tipo da pasta. Por exemplo, a propriedade **FolderClass** ou o elemento não indica que a pasta é uma pasta de contatos enquanto a classe ou o tipo da pasta indica que a pasta é uma pasta de calendário. 
    
- Você pode [criar pastas](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) de um tipo específico sem definir o elemento ou a propriedade **FolderClass** , ou você pode criar uma pasta com o tipo de pasta genérico e especificar o elemento ou a propriedade **FolderClass** . Ambas as opções criam o mesmo resultado. 
    
- Depois de definir o valor **FolderClass** criando um tipo específico de pasta ou definindo a propriedade **FolderClass** ou o próprio elemento, você não pode alterá-lo. Por exemplo, não é possível alterar um IPF. Pasta de anotações para um IPF. Pasta de contatos. No entanto, você pode alterá-lo para um IPF. Pasta note. contoso. 
    
- Qualquer valor **FolderClass** que não use um dos prefixos predefinidos é tratado como um IPF. Pasta de anotações. Por exemplo, um valor de **FolderClass** de IAmAFolderClass é tratado como um IPF. Pasta de anotações. 
    
O valor da classe Folder é extensível. Isso significa que os valores padrão de **FolderClass** listados na tabela 1 são tratados como prefixos e você pode adicionar valores personalizados. Por exemplo, você pode criar uma pasta com um valor **FolderClass** de IPF. Contact. contoso e ele é tratado como uma pasta de contatos. 
  
Você pode determinar quais permissões o cliente tem nas pastas, como excluir, ler e modificar, usando a propriedade [Folder. EffectiveRights](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) da API gerenciada do EWS ou o elemento EWS [EffectiveRights](https://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) . 
  
### <a name="public-folders"></a>Pastas públicas

As pastas públicas são feitas para acesso compartilhado e oferecem um jeito fácil e eficaz de coletar, organizar e compartilhar informações com outros pessoas no seu grupo de trabalho ou organização. Você também pode usar pastas públicas para arquivar o conteúdo do grupo de distribuição. Para obter informações detalhadas sobre pastas públicas, consulte [acesso a pastas públicas com o EWS no Exchange](public-folder-access-with-ews-in-exchange.md).

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>Pastas ocultas

Todas as pastas que o Exchange cria na raiz da caixa de correio estão ocultas e você pode usar a API gerenciada do EWS ou o EWS para ocultar pastas adicionais na parte superior do repositório de informações. Para obter mais informações sobre pastas ocultas, consulte [trabalhar com pastas ocultas usando o EWS no Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md). 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>Pastas de pesquisa

Pastas de pesquisa são exatamente como pastas normais, exceto pelo fato de terem uma propriedade ou elemento que define o filtro de pesquisa. Você pode criar pastas de pesquisa em qualquer pasta de uma caixa de correio do Exchange e criá-las da mesma maneira que você cria qualquer outra pasta. No entanto, para que uma pasta de pesquisa apareça no Outlook, no Outlook Web App ou no Outlook Live, os objetos do [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) que você cria usando a API gerenciada do EWS devem estar localizados na pasta [WellKnownFolderName. SearchFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e os tipos [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) que você cria usando o EWS devem estar localizados na pasta [DistinguishedFolderId. SearchFolders](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Se a pasta de pesquisa for criada em um local diferente, ela ainda estará disponível e você poderá exibi-la em aplicativos cliente personalizados. 

<a name="bk_item"> </a>

## <a name="items"></a>Itens

O EWS no Exchange usa **itens** para representar mensagens de email, compromissos, reuniões, contatos, listas de distribuição, tarefas, postagens e outros itens individuais em uma caixa de correio. Os itens têm rigidez de tipos, o que significa que eles têm uma classe ou esquema associado específico ou não digitados de forma alta, também conhecidas como itens genéricos. Os itens genéricos são objetos de [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) na API gerenciada do EWS e nos tipos de [Item](https://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) do EWS. Itens comuns como mensagens de email, contatos, listas de distribuição, postagens e tarefas são digitados com rigidez, e você pode definir propriedades ou elementos específicos do esquematizado. 
  
**Tabela 3. Itens fortemente tipados**

|**Tipo de item de API gerenciada do EWS**|**Elemento de item do EWS**|
|:-----|:-----|
|[Compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contato](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Contato](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Mensagem](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Item de postagem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[Item de postagem](https://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Tarefa](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Tarefa](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Os itens fortemente tipados da API gerenciada do EWS derivam da classe de [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) base. No entanto, geralmente você trabalha com um dos tipos derivados listados na tabela 3 e não com a classe de **Item** diretamente. No entanto, quando você trabalha com a classe [ItemCollection](https://msdn.microsoft.com/library/dd634001%28v=EXCHG.80%29.aspx) , pode trabalhar diretamente com instâncias da classe **Item** . Nesse caso, você deve implementar a lógica que determina o tipo de item no repositório que a instância da classe de **Item** representa. Para trabalhar com esse item, você deve associar ao item usando uma instância da classe que representa o item. 
  
### <a name="items-in-folders"></a>Itens em pastas

Algumas pastas têm restrições sobre os tipos de itens que podem conter. Essas são as restrições que o banco de dados de caixa de correio do Exchange aplica às pastas, não às limitações de exibição do cliente. 
  
**Tabela 4. Restrições de itens para pastas**

|**Classe de pasta de API gerenciada do EWS**|**Tipo de pasta do EWS**|**Restriction**|
|:-----|:-----|:-----|
|[Classe de pasta base](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) de API gerenciada do EWS e objetos [PostItem](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) ou tipos de [mensagem](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) do EWS ou tipos de **Item** , nas pastas genéricas. Você pode mover outros tipos de item para pastas genéricas, mas o cliente pode não exibi-los.  <br/> |
|[CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](https://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de [compromisso](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) da API gerenciada do EWS e tipos do EWS [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) na pasta calendário. Você pode mover outros tipos de item para a pasta calendário, mas o cliente pode não exibi-los.  <br/> |
|[ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](https://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Você só pode criar [novos objetos](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) [de contato da API](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) gerenciada do EWS e os tipos de [contato](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) do EWS ou tipos de [distribuiçãolist](https://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) na pasta contatos. Você pode mover outros tipos de item para a pasta contatos, mas o cliente pode não exibi-los  <br/> |
|[SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Sem restrições. Na verdade, os itens não estão localizados na pasta de pesquisa; Eles estão localizados em qualquer lugar na caixa de correio.  <br/> |
|[TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](https://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos [Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) do EWS Managed API ou tipos de [tarefa](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) do EWS na pasta tarefas. Você pode mover outros tipos de item para a pasta tarefas, mas o cliente pode não exibi-los  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>Atualizando de versões anteriores do produto

As pastas têm a maior parte permaneceram inalteradas nas versões anteriores e atuais do produto. No entanto, observe que as versões anteriores do Exchange usam pastas gerenciadas para executar o gerenciamento de registros de mensagens (MRM). O Exchange Online, o Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013 usam políticas de retenção para o MRM. Você pode [Atualizar pastas gerenciadas para usar políticas de retenção](https://technet.microsoft.com/library/dd298032%28v=exchg.150%29.aspx). 
  
Os itens não foram alterados nas versões anteriores e atuais do produto.

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>Nesta seção

- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com pastas ocultas usando o EWS no Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Exportar e importar itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

