---
title: Pastas e itens no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d8cf6fa-85a4-45ac-8165-e4d3ab92594e
description: Saiba mais sobre pastas e itens de caixa de correio e como seu EWS Managed API ou o cliente do EWS representa-los.
ms.openlocfilehash: a3358844f2317c9b0462456ff7d2f38442c98ee3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750686"
---
# <a name="folders-and-items-in-ews-in-exchange"></a>Pastas e itens no EWS no Exchange

Saiba mais sobre pastas e itens de caixa de correio e como seu EWS Managed API ou o cliente do EWS representa-los.
  
As pastas são o elemento organizador de uma caixa de correio do Exchange. As pastas podem conter itens de caixa de correio, como mensagens de email, contatos, compromissos, reuniões e tarefas, ou eles podem conter outras pastas. Exchange inclui tipos diferentes de pastas, mas os tipos de pasta são semelhantes uns aos outros. A principal diferença entre elas é o tipo de item que eles contêm.
  
Itens, no entanto, tem tipos exclusivos. Cada tipo de item tem um conjunto diferente de esquema para defini-la ou propriedades. Neste artigo, abordaremos os tipos de pastas e itens que estão disponíveis e as diferenças entre elas.

<a name="bk_folders"> </a>

## <a name="folders"></a>Pastas

Pastas todos os derivam do tipo base ou a mesma classe de base, a classe de [pasta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) na API gerenciada do EWS ou o tipo de [pasta](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) no EWS. A figura a seguir mostra as classes de API gerenciada de EWS e os tipos EWS. 
  
**Figura 1. Classes de pasta do EWS Managed API e tipos de pasta EWS**

![Uma ilustração que mostra as classes derivadas da classe Pasta de API Gerenciada do EWS e os tipos derivados do tipo de Pasta do EWS, todos nomeados CalendarFolder, ContactsFolder, SearchFolder e TasksFolder.](media/Ex2013_Folder_OverviewTypes.png)
  
A principal diferença entre cada uma das classes de pasta e tipos de pasta é que você só pode criar um determinado tipo de item em cada tipo de pasta. Uma diferença está em como o cliente exibe informações em uma pasta. Por exemplo, o Exchange permite que você crie compromissos na pasta Calendário. Você pode mover outros tipos de itens para a pasta Calendário, depois você criá-las, mas o Outlook não exibi-las. Outlook exibirá apenas os itens de calendário, como compromissos e reuniões na pasta Calendário, [mesmo se outro tipo de item existe na pasta](folders-and-items-in-ews-in-exchange.md#bk_item). 
  
**Tabela 1. Classes de pasta do EWS Managed API e tipos de pasta EWS**

|**Classe de API gerenciada de EWS**|**Tipo EWS**|**Valor de FolderClass**|**Contém**|**Notes**|
|:-----|:-----|:-----|:-----|:-----|
|[Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |FALHA DE PÁGINA INVÁLIDA. Observação  <br/> |Mensagens de email ou pastas.  <br/> | Este é o tipo para as seguintes pastas de API gerenciada de EWS [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e pastas do EWS [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) ou classe genérica pasta: <ul><li>  Raiz (IPM subárvore)</li><li>NonIpmSubtree</li><li>Caixa de Entrada</li><li>Itens excluídos</li><li>Rascunhos</li><li>Diário</li><li>Observações  </li><li>Caixa de saída</li><li>Itens enviados</li><li>Pasta de mensagem</li><li>Lixo eletrônico</li><li>Caixa Postal</li></ul> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |FALHA DE PÁGINA INVÁLIDA. Compromisso  <br/> |Compromissos e reuniões.  <br/> |Quando um usuário responde a uma solicitação de reunião, o compromisso é adicionado para a API gerenciada de EWS [WellKnownFolderName.Calendar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou apenas o EWS [DistinguishedFolderId.CalendarFolder](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Estas são as únicas pastas que suportam a interação automática com solicitações de reunião e respostas.  <br/><br/>Esta classe de pasta ou um tipo de pasta suporta o uso de exibições de calendário para retornar os compromissos e reuniões com base em uma data de início e uma data final, usando o método API gerenciada de EWS [Folder.FindItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) e a classe [CalendarView](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou o EWS [FindItem ](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)operação e o elemento de [exibição de calendário](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) .  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |FALHA DE PÁGINA INVÁLIDA. Contato  <br/> |Contatos e listas de distribuição.  <br/> |Nenhum.  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |FALHA DE PÁGINA INVÁLIDA. Observação  <br/> |Conteúdo é determinado por uma restrição ou filtro. Pastas de pesquisa não têm subpastas.  <br/> |Os itens que satisfazem os critérios de pesquisa, na verdade, não estão contidos na pasta de pesquisa; em vez disso, eles estão localizados em outro lugar na caixa de correio.  <br/> Para garantir que as pastas de pesquisa estão disponíveis no Outlook, criá-los na pasta Finder.  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |FALHA DE PÁGINA INVÁLIDA. Tarefa  <br/> |Contém os itens de trabalho para concluir.  <br/> |Nenhum.  <br/> |
   
### <a name="folder-structure"></a>Estrutura de pastas

As pastas fornecem uma estrutura de caixa de correio. Isso inclui a subárvore IPM, conhecido como a parte superior do armazenamento de informações no EWS, onde a maioria dos usuários interagem com suas caixas de correio, bem como pastas de sistema que nunca ver a maioria dos usuários, presentes na raiz no EWS ou subárvore Non-IPM. A figura a seguir mostra a estrutura de pastas de um usuário e indica quais pastas são para os itens do usuário e quais são as pastas do sistema.
  
**Figura 2. Pastas de sistema e o item em uma caixa de correio**

![Uma ilustração que mostra as pastas do sistema raiz, que inclui Favoritos, Localizador, Dados de disponibilidade, Início do repositório de informações e muito mais. O Início do repositório de informações contém as pastas do usuário, que incluem Calendário, Contatos e mais.](media/Ex2013_Folder_OverviewSampleHierarchy.png)
  
### <a name="well-known-folders"></a>Pastas conhecidas

As pastas de uma caixa de correio, algumas são pastas especiais. Esses correspondem aos conhecido pastas na API gerenciada do EWS, ou pastas diferenciadas no EWS. Algumas dessas pastas têm restrições sobre o nome da pasta onde estão localizados na estrutura de pasta e se eles podem ser excluídos. Outras pastas de (não-especial) "genéricas" não têm as mesmas restrições. É importante que você esteja familiarizado com as seguintes pastas conhecidas ou diferenciadas porque eles são o sistema de raiz, usuário e as pastas de pesquisa e são aplicáveis a maioria das implementações. 
  
**Tabela 2. Pastas de conhecido e diferenciadas principais**

|**Nome amigável**|**Valores de **WellKnownFolderName** API gerenciada de EWS**|**Valores de **DistinguishedFolderId** EWS**|**Descrição**|
|:-----|:-----|:-----|:-----|
|Raiz (não-IPM subárvore)  <br/> |WellKnownFolderName.Root  <br/> |DistinguishedFolderId.root  <br/> |Contém a pasta raiz de uma caixa de correio, também conhecida como a subárvore Non-IPM. Essa pasta não tem um pai, e você não pode mover, copiar, renomear ou excluí-lo. O armazenamento de cada mensagem contém apenas uma pasta raiz.  <br/> |
|Parte superior do armazenamento de informações (IPM subárvore)  <br/> |WellKnownFolderName.MsgFolderRoot  <br/> |DistinguishedFolderId.msgfolderroot  <br/> |Contém a caixa de entrada e outras pastas de usuário.  <br/> |
|Localizador (pastas de pesquisa)  <br/> |WellKnownFolderName.SearchFolders  <br/> |DistinguishedFolderId.searchfolders.  <br/> |Contém as pastas de pesquisa que são visíveis no Outlook.  <br/> |
   
Para obter uma lista completa dos valores de propriedade da API gerenciada de EWS [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.wellknownfoldername%28v=exchg.80%29.aspx) , consulte a enumeração [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=EXCHG.80%29.aspx) . Para obter uma lista completa dos valores do EWS **DistinguishedFolderId** , consulte [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx).
  
### <a name="folder-properties"></a>Propriedades da pasta

Na API gerenciada do EWS, as [Propriedades da pasta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder_properties%28v=exchg.80%29.aspx) são todos derivados da classe de [pasta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=EXCHG.80%29.aspx) base. E no EWS, todas as pastas usam os elementos de pasta que estão disponíveis no tipo de [pasta](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) . A maioria dos elementos e propriedades relacionadas à pasta são simples (ID da pasta pai, nome para exibição e assim por diante), mas algumas exigem um pouco mais de explicação. 
  
As seguintes condições se aplicam à propriedade EWS Managed API [Folder.FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=EXCHG.80%29.aspx) ou o elemento do EWS [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) : 
  
- Se definido, o valor da propriedade ou elemento deve concordar com o tipo da pasta ou uma classe derivada. Por exemplo, a propriedade **FolderClass** ou elemento não pode indicar que a pasta é uma pasta de contatos ao mesmo tempo a classe ou o tipo da pasta indica que a pasta é uma pasta de calendário. 
    
- Você pode qualquer [criar pastas](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) de um tipo específico sem a definição da propriedade **FolderClass** ou elemento ou você pode criar uma pasta com o tipo de pasta genérico e especifique a propriedade **FolderClass** ou elemento. As duas opções criam o mesmo resultado. 
    
- Depois de definir o valor de **FolderClass** criando um tipo específico de pasta ou definindo a propriedade **FolderClass** ou elemento em si, você não pode alterá-lo. Por exemplo, você não pode alterar uma falha de página inválida. Pasta de anotação para uma falha de página inválida. Pasta de contato. No entanto, você pode, altere-o para uma falha de página inválida. Pasta Note.Contoso. 
    
- Qualquer valor de **FolderClass** que não usa um dos prefixos predefinidos é tratado como uma falha de página inválida. Pasta de nota. Por exemplo, um valor de **FolderClass** de IAmAFolderClass é tratado como uma falha de página inválida. Pasta de nota. 
    
O valor de classe da pasta é extensível. Isso significa que os valores de **FolderClass** padrão listados na tabela 1 são tratados como prefixos e você pode adicionar valores personalizados. Por exemplo, você pode criar uma pasta com um valor de **FolderClass** de falha de página inválida. Contact.Contoso e ele será tratada como uma pasta de contatos. 
  
Você pode determinar quais permissões que o cliente possui nas pastas, como excluir, ler e modificar, usando a propriedade EWS Managed API [Folder.EffectiveRights](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.effectiverights%28v=EXCHG.80%29.aspx) ou o elemento do EWS [EffectiveRights](http://msdn.microsoft.com/library/bf5278eb-3a1a-4d27-9d16-b8be043bb023%28Office.15%29.aspx) . 
  
### <a name="public-folders"></a>Pastas públicas

Pastas públicas são projetadas para acesso compartilhado e oferecem uma maneira fácil e eficaz de coletar, organizar e compartilhar informações com outras pessoas em seu grupo de trabalho ou organização. Você também pode usar pastas públicas para arquivar o conteúdo de grupo de distribuição. Para obter informações detalhadas sobre pastas públicas, consulte a [pasta pública acessar com EWS no Exchange](public-folder-access-with-ews-in-exchange.md).

<a name="bk_hiddenfolders"> </a>

### <a name="hidden-folders"></a>Pastas ocultas

Todas as pastas que Exchange cria na raiz da caixa de correio estão ocultos, e você pode usar a API gerenciada de EWS ou o EWS para ocultar adicionais pastas sob a parte superior do armazenamento de informações. Para obter mais informações sobre pastas ocultas, consulte [trabalhar com pastas ocultas usando o EWS no Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md). 

<a name="bk_hiddenfolders"> </a>

### <a name="search-folders"></a>Pastas de pesquisa

Pastas de pesquisa são assim como as pastas regulares, exceto que eles têm uma propriedade ou um elemento que define o filtro de pesquisa. Você pode criar pastas de pesquisa em qualquer pasta em uma caixa de correio do Exchange e criá-los da mesma maneira que você criar qualquer outra pasta. No entanto, para uma pasta de pesquisa seja exibido no Outlook, Outlook Web App ou Outlook Live, [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) objetos criados usando a API gerenciada de EWS devem estar localizados na pasta [WellKnownFolderName.SearchFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) tipos de que você criar usando o EWS devem estar localizados na pasta [DistinguishedFolderId.SearchFolders](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) . Se a pasta de pesquisa é criada em um local diferente, ela ainda está disponível e possível exibi-la em aplicativos cliente personalizado. 

<a name="bk_item"> </a>

## <a name="items"></a>Items

EWS no Exchange usa **itens** para representar mensagens de email individuais, compromissos, reuniões, contatos, listas de distribuição, tarefas, publicações e outros itens, em uma caixa de correio. Os itens são que um digitado fortemente, que significa que têm uma classe associada específica ou esquema ou itens não fortemente tipadas, também conhecido como genéricos. Itens genéricos são objetos de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) em tipos EWS Managed API e o [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) no EWS. Itens comuns, como mensagens de email, contatos, listas de distribuição, postagens, tarefas são fortemente tipadas e você pode definir as propriedades específicas de esquematizado ou elementos neles. 
  
**Tabela 3. Itens fortemente tipadas**

|**Tipo de item de API gerenciada de EWS**|**Elemento de item EWS**|
|:-----|:-----|
|[Compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Contato](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Contato](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |[DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) <br/> |
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |[PostItem](http://msdn.microsoft.com/library/7727ed84-9591-4a1c-bb04-12129926499b%28Office.15%29.aspx) <br/> |
|[Task](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
API gerenciada de EWS fortemente tipadas itens derivam da classe base do [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=EXCHG.80%29.aspx) . No entanto, você normalmente trabalha com um dos tipos derivados listados na tabela 3 e não com a classe de **Item** diretamente. Quando você trabalha com a classe [ItemCollection](http://msdn.microsoft.com/en-us/library/dd634001%28v=EXCHG.80%29.aspx) , no entanto, você pode trabalhar diretamente com instâncias da classe **Item** . Nesse caso, você deve implementar lógica que determina o tipo de item no repositório que representa a instância da classe **Item** . Para trabalhar com esse item, você deve vincular ao item usando uma instância da classe que representa o item. 
  
### <a name="items-in-folders"></a>Itens em pastas

Algumas pastas têm restrições sobre os tipos de itens que podem conter. Estas são as restrições que o banco de dados de caixa de correio do Exchange se aplica às pastas, não limitações de modo de exibição do cliente. 
  
**Tabela 4. Restrições de item para pastas**

|**Classe de pasta API gerenciada de EWS**|**Tipo de pasta de EWS**|**Restriction**|
|:-----|:-----|:-----|
|[Classe de pasta base](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |[Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de API gerenciada de EWS [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) e objetos [PostItem](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) , ou tipos de EWS [mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) ou **PostItem** tipos, nas pastas genéricas. Você pode mover outros tipos de itens em pastas genéricas, mas o cliente não poderá exibi-las.  <br/> |
|[CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |[CalendarFolder](http://msdn.microsoft.com/library/48687a78-e757-4c04-9641-bf4302c6b565%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de API gerenciada de EWS [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) e tipos EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) na pasta de calendário. Você pode mover outros tipos de item para a pasta Calendário, mas o cliente não poderá exibi-las.  <br/> |
|[ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |[ContactsFolder](http://msdn.microsoft.com/library/6c299de8-2087-4aeb-8e66-2bc7586509a6%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de API gerenciada de EWS [contato](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) e [ContactGroup](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) , ou tipos EWS [contato](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) ou [DistributionList](http://msdn.microsoft.com/library/f65aea01-e870-44a2-8571-fa6c001341cc%28Office.15%29.aspx) na pasta Contatos. Você pode mover outros tipos de item para a pasta Contatos, mas o cliente não poderá exibi-las  <br/> |
|[SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) <br/> |Sem restrições. Itens realmente não estão localizados na pasta de pesquisa; eles estão localizados em outro lugar na caixa de correio.  <br/> |
|[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |[TasksFolder](http://msdn.microsoft.com/library/5a9a4612-8064-4986-b467-c44f268c64df%28Office.15%29.aspx) <br/> |Você só pode criar novos objetos de API gerenciada de EWS [tarefa](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) ou tipos EWS [tarefa](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) na pasta tarefas. Você pode mover outros tipos de item para a pasta tarefas, mas o cliente não poderá exibi-las  <br/> |

<a name="bk_upgrading"> </a>

## <a name="upgrading-from-earlier-product-versions"></a>Atualizando versões anteriores do produto

Pastas na maioria das vezes permanecem inalteradas em versões do produto anterior e atual. No entanto, observe que as versões anteriores do Exchange usam pastas gerenciadas para executar o gerenciamento de registros de mensagens (MRM). O Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013 use políticas de retenção para MRM. Você pode [atualização gerenciados pastas usar políticas de retenção](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.150%29.aspx). 
  
Itens não foram alteradas em versões do produto anterior e atual.

<a name="bk_inthissection"> </a>

## <a name="in-this-section"></a>Nesta seção

- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com pastas ocultas usando o EWS no Exchange](how-to-work-with-hidden-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Exportar e importar itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)   
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)   
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

