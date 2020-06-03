---
title: Excluir itens usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Descubra como você pode usar a API gerenciada do EWS ou o EWS no Exchange para excluir itens movendo-os para a pasta itens excluídos ou para o dumpster.
localization_priority: Priority
ms.openlocfilehash: 83317ccd0fa1db64e14df68652489009fea4ea07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456115"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Excluir itens usando o EWS no Exchange

Descubra como você pode usar a API gerenciada do EWS ou o EWS no Exchange para excluir itens movendo-os para a pasta itens excluídos ou para o dumpster.
  
Você já se perguntou qual é a diferença entre mover itens para a pasta itens excluídos e movê-los para o dumpster? Você pode estar curioso sobre as diferentes opções para manipular itens excluídos e como implementar essas opções em seu aplicativo. Os serviços Web do Exchange (EWS) incluem três opções para lidar com itens excluídos. Neste artigo, esperorá qualquer confusão que você possa ter sobre as diferenças entre eles.
  
## <a name="deleting-items---what-are-my-options"></a>Excluindo itens-quais são as minhas opções?
<a name="bk_DeletingItemsOptions"> </a>

Para que você possa entender o panorama geral da exclusão de itens, é importante reconhecer a diferença entre o seguinte:
  
- A pasta itens excluídos-quando você exclui itens em uma caixa de correio, é aí que eles vão.
    
- O dumpster (aka a pasta itens recuperáveis)-quando você remove itens de uma caixa de correio, é aí que eles vão.
    
As figuras 1 e 2 mostram a aparência do processo de exclusão para itens e pastas em uma caixa de correio. 

**Figura 1. Processo para excluir itens de uma caixa de correio**

![Uma ilustração que mostra para onde os itens vão quando são excluídos. Itens excluídos são movidos para a pasta itens excluídos e, em seguida, são movidos para a pasta itens recuperáveis por política de retenção, onde eles expiram e são permantently excluídos.](media/Ex_DeleteItems_Source.png)

<br/>

**Figura 2. Processo para excluir pastas de uma caixa de correio**

![Uma ilustração que mostra como pastas excluídas são movidas para a pasta Itens Excluídos e, em seguida, podem ser permanentemente excluídas da caixa de correio.](media/Ex_.png)
   
Você pode excluir itens e pastas de três maneiras diferentes, dependendo de como "permanente" você deseja que a exclusão seja.
  
**Tabela 1: opções para excluir itens usando o EWS**

|**Opção**|**O que acontece**|
|:-----|:-----|
|Mover para a pasta Itens Excluídos  <br/> |Esta é a maneira menos permanente de excluir itens.<br/><br/>Isso é como colocar uma folha de papel na lixeira de sua mesa. Você pode facilmente confazê-la se precisar dela novamente.<br/><br/>Você pode usar qualquer [operação de exclusão](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) que implemente a opção mover para a pasta itens excluídos para executar essa ação.<br/><br/>Você também pode usar a [operação MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item. Move ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) ou a [operação MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder. Move ()](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) para mover um item ou pasta para a pasta itens excluídos.  <br/> |
|Exclusão reversível  <br/> |O item é movido para a pasta exclusões no dumpster.<br/><br/>Isso é como esvaziar sua lixeira no contêiner do Curbside. Você ainda pode acessar o item, se precisar, é apenas um pouco mais difícil.  <br/><br/>Para saber mais sobre o dumpster (também chamado de itens recuperáveis) e cenários como eDiscovery ou isenções de litígio, confira [pasta itens recuperáveis](https://technet.microsoft.com/library/ee364755%28v=exchg.150%29.aspx) no TechNet.<br/><br/>As exclusões suaves não são recomendadas para aplicativos direcionados para o Exchange 2007. No Exchange 2007, as exclusões suaves são tratadas Configurando um bit no item para indicar que ele será movido para o dumpster em um horário não especificado.<br/><br/>Exclusões de exclusão reversível ou pesquisas de itens que foram excluídos de forma reversível por meio da [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), não são compatíveis com o Exchange Online, o Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2010.  <br/><br/>**Observação**: pastas não podem ser excluídas de forma reversível.           |
|Exclusão irreversível  <br/> |O item ou pasta é excluído permanentemente.<br/><br/>Os itens excluídos por hardware são colocados na pasta limpezas do dumpster. Isso é como quando o caminhão de reciclagem esvazia o contêiner de reciclagem do Curbside. Os itens não podem ser acessados de um cliente de email como o Outlook ou o Outlook Web App e, a menos que haja uma retenção definida na caixa de correio, os itens serão excluídos permanentemente após um determinado período de tempo.<br/><br/>Você pode ler mais sobre a retenção de itens no artigo [configurar cotas de itens recuperáveis e retenção de item excluído](https://technet.microsoft.com/library/ee364752%28v=exchg.150%29.aspx).<br/><br/>**Observação**: as pastas não são colocadas na pasta limpezas quando são excluídas. As pastas excluídas por hardware são removidas da caixa de correio.  |
   
A movimentação para a pasta itens excluídos e as opções de exclusão de hardware são transacionais, o que significa que, quando a chamada do serviço Web é concluída, o item foi movido para a pasta itens excluídos ou o dumpster.
  
Para ajudá-lo a entender melhor o ecossistema de pastas usadas para armazenar itens excluídos, a figura a seguir mostra a hierarquia de pastas que podem conter itens excluídos. Os nomes de pasta são como aparecem no tipo de esquema **DistinguishedFolderIdNameType** ou a enumeração **WellKnownFolderName** na API gerenciada do EWS. 
  
**Figura 3. Hierarquia de pastas que contêm itens excluídos**

![Uma figura que mostra a hierarquia de pastas que podem conter itens excluídos em uma caixa de correio primária e de arquivamento. Cada pasta na imagem é representada por seu nome de pasta distinto.](media/Ex_FolderHierarchyDeletedItems.png)
  
**Tabela 2: pastas que contêm itens excluídos**

|**Nome da pasta**|**Introduzido no**|**Descrição**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |A pasta itens excluídos padrão. Os itens permanecem nessa pasta até que sejam Soft-ou discos excluídos ou até que um período de retenção tenha sido excedido. Em seguida, eles são movidos para uma pasta no dumpster. As pastas excluídas são colocadas na pasta itens excluídos e, quando são removidas ou impróprias, elas são excluídas permanentemente da caixa de correio e não são recuperáveis.  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |A raiz do dumpster ou da pasta itens recuperáveis. O acesso ao dumpster foi implementado no EWS no Exchange 2010. O nome para exibição dessa pasta é "itens recuperáveis".  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |A pasta de dumpster principal de uma caixa de correio. Itens excluídos por software e itens movidos da pasta itens excluídos por uma política de retenção são colocados nessa pasta. O nome de exibição dessa pasta é "exclusões".  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |Onde as versões mais antigas de um item são armazenadas. Versões antigas de um item são criadas quando um item é atualizado. Versões de item de rascunho não são salvas nesta pasta. O nome de exibição dessa pasta é "Versions".  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |Em que os itens removidos da pasta exclusões são armazenados. Todos os itens excluídos do repositório são movidos para esta pasta. O nome de exibição para esta pasta é "limpezas".  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |A pasta itens excluídos padrão para uma caixa de correio de arquivo morto.  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |A pasta de dumpster raiz para uma caixa de correio de arquivo morto. Os itens arquivados excluídos de forma reversível são movidos para uma subpasta nessa pasta.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |A pasta de dumpster principal para uma caixa de correio de arquivo morto. Os itens arquivados movidos para o dumpster são colocados aqui.  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |Onde as versões mais antigas dos itens arquivados são armazenadas.  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |Em que os itens que são excluídos da pasta de exclusões de arquivo morto no dumpster estão armazenados. Todos os itens arquivados excluídos do repositório são movidos para esta pasta.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Como faço para excluir itens?
<a name="bk_howdoIdeleteitems"> </a>

Use uma das opções a seguir para indicar se mover um item para a pasta itens excluídos ou executar uma exclusão reversível ou uma exclusão difícil:
  
- O tipo simples **alientype** , se você usar EWS para acessar o Exchange. 
    
- A [Enumeração deleteMode](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), se você usar a API gerenciada do EWS.
    
Você pode usar um número de operações EWS diferentes ou métodos de API gerenciada do EWS para excluir itens e pastas de uma caixa de correio.
  
**Tabela 3: operações do EWS e métodos da API gerenciada do EWS para exclusão de itens**

|**Operação do EWS**|**Método de API gerenciada do EWS**|**Introduzido no**|**Função**|
|:-----|:-----|:-----|:-----|
|[Operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Método Folder. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Exclui pastas de uma caixa de correio. Com o EWS, você pode excluir pastas em lote. Com a API gerenciada do EWS, você só pode excluir uma única pasta por chamada.  <br/> |
|[Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Método item. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Método ExchangeService. DeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Exclui itens de uma caixa de correio.  <br/> |
|[Operação EmptyFolder](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Método Folder. Empty](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Exclui todos os itens em uma pasta e, opcionalmente, exclui todas as subpastas em uma pasta.  <br/> |
|[Operação ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Método CONVERSATION. EnableAlwaysDeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Método CONVERSATION. DeleteItems](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Define uma ação de processamento de exclusão em mensagens de email em uma conversa para que elas sejam excluídas.  <br/> |
|[Operação DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Método userconfiguration. Delete](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Exclui um item associado à pasta e o move para o dumpster.  <br/> |
|[Operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Método de compromisso. Accept](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Método de compromisso. AcceptTentatively](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Método de compromisso. CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Compromisso. recusar](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest. Accept](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest. AcceptTentatively](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest. rejeição](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Move indiretamente um item para a pasta itens excluídos sempre que uma resposta a uma solicitação de reunião é enviada ou a resposta é definida no compromisso.<br/><br/>O tipo de exclusão não está definido nessa operação. As mensagens de reunião são movidas para a pasta itens excluídos quando um objeto Response é processado com êxito pelo serviço.  <br/> |
   
Você também pode mover itens para a pasta itens excluídos usando regras de caixa de entrada. Por exemplo, você pode [criar regras](inbox-management-and-ews-in-exchange.md) que têm uma ação de exclusão. 
  
Alguns pontos a serem observados sobre a exclusão de itens:
  
- Excluir uma ocorrência de um item recorrente não dispara uma movimentação para a pasta itens excluídos ou o dumpster. Isso resulta em uma atualização para o item mestre recorrente da série recorrente.
    
- Não é possível excluir pastas padrão da caixa de correio.
    
- Evite excluir reuniões ou mensagens de reunião, como solicitações de reunião e atualizações de reunião. Em vez disso, responda a esses itens usando objetos Response. Dessa forma, os itens de calendário associados são atualizados para refletir as ações do Respondente ou do organizador.
    
- A chave de alteração de um item não é atualizada quando o item é movido para a pasta itens excluídos ou exclusões.
    
- Se você executar uma exclusão de hardware em um item e, em seguida, chamar uma [operação SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) ou um método de API gerenciada do EWS do [SyncFolderHierarchy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) , ou uma [operação SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) ou [SyncFolderItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , uma entrada de alteração de **exclusão** será retornada. Se você mover um item para a pasta itens excluídos, uma entrada de alteração de **atualização** será retornada. Isso ocorre porque o item ou a pasta terá um novo valor da propriedade [ParentFolderId](https://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . [Leia mais sobre sincronização](mailbox-synchronization-and-ews-in-exchange.md) se a sincronização de itens excluídos fizer parte do seu cenário. 
    
## <a name="find-out-more-about-deleting-items"></a>Saiba mais sobre como excluir itens
<a name="findoutmore"> </a>

- [Notificações de recebimento para eventos de caixa de correio relacionados à exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Tratamento de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)    
- [Pasta itens recuperáveis](https://technet.microsoft.com/library/ee364755.aspx)    
- [Recuperação de item único no Exchange Server 2010](https://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: excluir uma série recorrente programaticamente de servidores do Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: excluir tarefas de uma conta em servidores Exchange de forma programática](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013: pastas vazias em servidores Exchange de forma programática](https://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: excluir pastas programaticamente de servidores do Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: excluir vários itens programaticamente de servidores do Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: excluir contatos programaticamente de servidores do Exchange](https://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Gerenciar configurações de aplicativos persistentes usando o EWS no Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

