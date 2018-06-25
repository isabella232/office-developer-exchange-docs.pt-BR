---
title: Excluindo itens usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c81e3160-e12b-47e0-b3d6-4be28537f301
description: Descubra como você pode usar a API gerenciada de EWS ou EWS no Exchange para excluir itens por movê-los para a pasta Itens excluídos ou para o dumpster.
ms.openlocfilehash: a475ebc6677e5f5003cc790a2d4d2b83c513f309
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750672"
---
# <a name="deleting-items-by-using-ews-in-exchange"></a>Excluindo itens usando o EWS no Exchange

Descubra como você pode usar a API gerenciada de EWS ou EWS no Exchange para excluir itens por movê-los para a pasta Itens excluídos ou para o dumpster.
  
Você nunca solicitaram si mesmo o que é a diferença entre mover itens para a pasta Itens excluídos e movê-los para o dumpster? Você pode estar curioso para saber as diferentes opções de itens excluída de manipulação e como implementar essas opções em seu aplicativo. Serviços Web do Exchange (EWS) inclui três opções para itens excluído de tratamento. Este artigo esperamos limpará qualquer confusão, que você pode ter sobre as diferenças entre elas.
  
## <a name="deleting-items---what-are-my-options"></a>Excluindo itens - quais são minhas opções?
<a name="bk_DeletingItemsOptions"> </a>

Antes que você possa compreender o cenário geral para excluir itens, é importante reconhecer a diferença entre o seguinte:
  
- A pasta Itens excluídos - quando você exclui os itens em uma caixa de correio, isso é onde eles ir.
    
- O dumpster (também conhecido como a pasta itens recuperáveis) - quando você remove itens de uma caixa de correio, isso é onde eles ir.
    
Figuras 1 e 2 mostram a aparência do processo de exclusão de itens e pastas em uma caixa de correio. 

**Figura 1. Processo para exclusão de itens de uma caixa de correio**

![Os itens de uma ilustração mostra onde ir quando eles são excluídos. Itens excluídos são movidas para a pasta Itens excluídos e, em seguida, são movidas para a pasta itens recuperáveis por política de retenção, onde eles expiram e são permantently excluído.](media/Ex_DeleteItems_Source.png)

<br/>

**Figura 2. Processo para exclusão de pastas de uma caixa de correio**

![Uma ilustração que mostra como pastas excluídas são movidas para a pasta Itens Excluídos e, em seguida, podem ser permanentemente excluídas da caixa de correio.](media/Ex_.png)
   
Você pode excluir itens e pastas de três maneiras diferentes, dependendo de como "permanente" você gostaria de ser a exclusão.
  
**Tabela 1: Opções de exclusão de itens usando o EWS**

|**Opção**|**O que acontece**|
|:-----|:-----|
|Mover para a pasta Itens excluídos  <br/> |Essa é a maneira permanente mínimos para excluir itens.<br/><br/>Isso é como colocar uma folha de papel na Lixeira por sua mesa de trabalho. Você pode capturá-la facilmente se você precisar novamente.<br/><br/>Você pode usar qualquer [operação de exclusão](deleting-items-by-using-ews-in-exchange.md#bk_howdoIdeleteitems) que implementa a mudança para a opção de pasta de itens excluídos para executar essa ação.<br/><br/>Você também pode usar a [operação MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) ( [Item.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx)) ou a [operação MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) ( [Folder.Move()](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx)) para mover um item ou pasta para a pasta Itens excluídos.  <br/> |
|Exclusão reversível  <br/> |O item é movido para a pasta de exclusões no dumpster.<br/><br/>Isso é como esvaziar a Lixeira em seu contêiner de curbside. Você ainda pode acessar o item se for necessário, é um pouco mais difícil.  <br/><br/>Para obter mais informações sobre o dumpster (também chamado de pasta itens recuperáveis) e cenários como isenções de descoberta eletrônica ou litígios, consulte a [Pasta itens recuperáveis](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx) no TechNet.<br/><br/>Exclusões suaves não são recomendadas para aplicativos destino Exchange 2007. No Exchange 2007, exclusões suaves são tratadas por configuração um pouco no item para indicar que ela será movida para o dumpster momento não especificado.<br/><br/>Exclusão reversível traversais ou pesquisas de itens que tenham sido suaves excluídos por meio da [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx), não são suportadas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2010.  <br/><br/>**Observação**: pastas não podem ser excluídas soft.           |
|Exclusão dura  <br/> |O item ou a pasta é excluída permanentemente.<br/><br/>Itens excluídos de disco rígido são colocados na pasta limpezas do dumpster. Isso é como quando o reciclagem caminhão esvazia seu contêiner de reciclagem curbside. Os itens não podem ser acessados a partir de um cliente de email como o Outlook ou o Outlook Web App e, a menos que haja uma isenção definido na caixa de correio, os itens serão excluídos permanentemente após um período definido de tempo.<br/><br/>Você pode ler mais sobre a retenção de item no artigo [Configurar retenção de Item excluído e cotas de itens recuperáveis](http://technet.microsoft.com/en-us/library/ee364752%28v=exchg.150%29.aspx).<br/><br/>**Observação**: pastas não são colocadas na pasta limpezas quando eles grave são excluídos. Pastas de disco rígido excluído serão removidas da caixa de correio.  |
   
A mudança para a pasta Itens excluídos e as opções de exclusão dura são transacional, o que significa que no momento em que a chamada de serviço da web estiver concluída, o item foi movido para a pasta Itens excluídos ou o dumpster.
  
Para ajudá-lo a compreender melhor o ecossistema das pastas que são usadas para armazenar itens excluídos, a figura a seguir mostra a hierarquia de pastas que pode conter os itens excluídos. Os nomes de pasta são como aparecem no tipo de esquema **DistinguishedFolderIdNameType** ou a enumeração **WellKnownFolderName** na API gerenciada do EWS. 
  
**Figura 3. Hierarquia de pastas que contêm os itens excluídos**

![Uma figura que mostra a hierarquia de pastas que podem conter itens excluídos em uma caixa de correio primária e de arquivamento. Cada pasta na imagem é representada por seu nome de pasta distinto.](media/Ex_FolderHierarchyDeletedItems.png)
  
**Tabela 2: Pastas que contêm os itens excluídos**

|**Nome da pasta**|**Introduzido no**|**Descrição**|
|:-----|:-----|:-----|
|deleteditems  <br/> |Exchange 2007  <br/> |A pasta de itens excluídos do padrão. Os itens permanecem nessa pasta até que estejam ou disco rígido-excluída ou até que um período de retenção foi excedido. Em seguida, eles serão movidos para uma pasta no dumpster. Deleted pastas são colocadas na pasta Itens excluídos, e quando estiverem ou disco rígido-excluída, eles são permanentemente removidos da caixa de correio e não podem ser recuperados.  <br/> |
|recoverableitemsroot  <br/> |Exchange 2010  <br/> |Da raiz do dumpster, ou a pasta itens recuperáveis. Acesso do Dumpster foi implementado no EWS no Exchange 2010. O nome de exibição para essa pasta é "Itens recuperáveis".  <br/> |
|recoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Principal dumpster pasta para uma caixa de correio. Itens excluída e itens movidos da pasta Itens excluídos por uma política de retenção são colocados nessa pasta. O nome de exibição para essa pasta é "Exclusões".  <br/> |
|recoverableitemsversions  <br/> |Exchange 2010  <br/> |Onde as versões mais antigas de um item são armazenadas. Versões antigas de um item são criadas quando um item é atualizado. Versões de itens de rascunho não são salvos nessa pasta. O nome para exibição dessa pasta é "Versões".  <br/> |
|recoverableitemspurges  <br/> |Exchange 2010  <br/> |Onde os itens que são removidos da pasta exclusões são armazenados. Todos os itens de armazenamento de disco rígido excluído são movidos para essa pasta. O nome de exibição para essa pasta é "Limpa".  <br/> |
|archiveddeletedtitems  <br/> |Exchange 2010  <br/> |A pasta Itens excluídos do padrão para uma caixa de correio de arquivo morto.  <br/> |
|archiverecoverablesitemsroot  <br/> |Exchange 2010  <br/> |A raiz do dumpster pasta para uma caixa de correio de arquivo morto. Itens que estão excluída arquivados são movidos para uma subpasta nesta pasta.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Exchange 2010  <br/> |Principal dumpster pasta para uma caixa de correio de arquivo morto. Arquivadas itens movidos para o dumpster são colocados aqui.  <br/> |
|archiverecoverableitemsversions  <br/> |Exchange 2010  <br/> |Onde as versões mais antigas do itens arquivados estão armazenadas.  <br/> |
|archiverecoverableitemspurges  <br/> |Exchange 2010  <br/> |Onde os itens que estão excluídos do arquivo morto exclusões de pasta no dumpster são armazenados. Todos os itens do repositório rígido excluído arquivado são movidos para essa pasta.  <br/> |
   
## <a name="how-do-i-delete-items"></a>Como faço para excluir itens?
<a name="bk_howdoIdeleteitems"> </a>

Utilize um dos procedimentos a seguir para indicar se deseja mover um item para a pasta Itens excluídos ou executar um reversível excluir ou excluir um disco rígido:
  
- O **DisposalType** tipo simples, se você usar o EWS para acessar o Exchange. 
    
- A [enumeração DeleteMode](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx), se você usar a API gerenciada de EWS.
    
Você pode usar um número de diferentes operações de EWS ou os métodos de API gerenciada de EWS para excluir pastas e itens de uma caixa de correio.
  
**Tabela 3: Operações do EWS e métodos de API gerenciada de EWS para excluir itens**

|**Operação do EWS**|**Método API gerenciada de EWS**|**Introduzido no**|**O que ele faz**|
|:-----|:-----|:-----|:-----|
|[Operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |[Método Folder.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Exclui pastas de uma caixa de correio. Com o EWS, você pode lote excluir pastas. Com a API gerenciada de EWS, você só pode excluir uma única pasta por chamada.  <br/> |
|[Operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Método item](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)<br/><br/>[Método ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.exchangeservice.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Exclui os itens de uma caixa de correio.  <br/> |
|[Operação EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <br/> |[Método Folder.Empty](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.folder.empty%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Exclui todos os itens em uma pasta e, opcionalmente, exclui todas as subpastas em uma pasta.  <br/> |
|[Operação ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |[Método Conversation.EnableAlwaysDeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx)<br/><br/>[Método Conversation.DeleteItems](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.conversation.deleteitems%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Define uma exclusão processamento ação em mensagens de email em uma conversa de modo que eles são excluídos.  <br/> |
|[Operação DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[Método UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |Exchange 2010  <br/> |Exclui uma pasta associada item e o move para o dumpster.  <br/> |
|[Operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |[Método Appointment.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accept%28v=exchg.80%29.aspx) <br/><br/>[Método Appointment.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Método Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)<br/><br/>[Appointment.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.decline%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest.Accept](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accept%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest.AcceptTentatively](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.accepttentatively%28v=exchg.80%29.aspx)<br/><br/>[Método MeetingRequest.Decline](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequest.decline%28v=exchg.80%29.aspx) <br/> |Exchange 2007  <br/> |Move um item para a pasta Itens excluídos indiretamente sempre que uma resposta a uma solicitação de reunião é enviada ou a resposta foi definida no compromisso.<br/><br/>O tipo de exclusão não está definida nessa operação. As mensagens de reunião são movidas para a pasta Itens excluídos quando um objeto de resposta com êxito é processado pelo serviço.  <br/> |
   
Você também pode mover itens para a pasta Itens excluídos usando regras de caixa de entrada. Por exemplo, você pode [criar regras](inbox-management-and-ews-in-exchange.md) que tenham uma ação de excluir. 
  
Alguns pontos a serem observados sobre a exclusão de itens:
  
- Excluir uma ocorrência de um item recorrente não aciona uma movimentação para a pasta Itens excluídos ou o dumpster. Isso resulta em uma atualização para o item mestre recorrente da série recorrente.
    
- Você não pode excluir pastas padrão da caixa de correio.
    
- Evite a exclusão de reuniões ou mensagens de reunião, solicitações de reunião e/ou atualizações de reunião. Em vez disso, responda a estes itens usando objetos de resposta. Dessa forma, os itens de calendário associadas são atualizados para refletir do organizador ou do Respondente ações.
    
- Alterar chave de um item não será atualizado quando o item é movido para a pasta Itens excluídos ou exclusões.
    
- Se você executar um disco rígido excluir em um item e chamar uma [operação SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) ou método de API gerenciada de EWS [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) ou um método [SyncFolderItems operação](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) ou [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) , uma alteração de **Excluir** entrada será retornada. Se você mover um item para a pasta Itens excluídos, uma entrada de alteração de **atualização** será retornada. Isso ocorre porque o item ou a pasta terá um novo valor da propriedade [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) . [Leia mais sobre sincronização](mailbox-synchronization-and-ews-in-exchange.md) se sincronizando itens excluídos faz parte do seu cenário. 
    
## <a name="find-out-more-about-deleting-items"></a>Saiba mais sobre a exclusão de itens
<a name="findoutmore"> </a>

- [Receber notificações de eventos de caixa de correio relacionadas a exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Tratando erros relacionados a exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)    
- [Pasta itens recuperáveis](http://technet.microsoft.com/en-us/library/ee364755.aspx)    
- [Recuperação de Item único no Exchange Server 2010](http://blogs.technet.com/b/exchange/archive/2009/09/25/3408389.aspx#_Single_Item_Recovery)    
- [Exchange 2013: Excluir uma série recorrente programaticamente dos servidores do Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-a-e1c7b89d)    
- [Exchange 2013: Excluir tarefas de uma conta em servidores Exchange programaticamente](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-tasks-13824637)    
- [Exchange 2013: Esvaziar pastas em servidores Exchange programaticamente](http://code.msdn.microsoft.com/exchange/Exchange-2013-Empty-6487df37)    
- [Exchange 2013: Exclua pastas programaticamente dos servidores do Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-aa1a5823)    
- [Exchange 2013: Excluir muitos itens programaticamente dos servidores do Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-many-064f8760)    
- [Exchange 2013: Excluir contatos programaticamente dos servidores do Exchange](http://code.msdn.microsoft.com/exchange/Exchange-2013-Delete-3b8b0640)    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)    
- [Gerenciar configurações de aplicativo persistente usando o EWS no Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    

