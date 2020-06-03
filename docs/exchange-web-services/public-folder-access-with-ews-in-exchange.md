---
title: Acesso a pastas públicas com o EWS no Exchange
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Saiba como usar o EWS e a API gerenciada do EWS para acessar pastas públicas e encaminhar solicitações de pasta pública no Exchange.
localization_priority: Priority
ms.openlocfilehash: e921a77b250e11e974b0c47b1d28a8e020837d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460208"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Acesso a pastas públicas com o EWS no Exchange

Saiba como usar o EWS e a API gerenciada do EWS para acessar pastas públicas e encaminhar solicitações de pasta pública no Exchange.
  
As pastas públicas fornecem um repositório compartilhado de itens que os usuários em sua organização podem acessar. O Office 365, o Exchange Online e as versões locais do Exchange, começando com o Exchange 2013, introduzem uma nova arquitetura para pastas públicas. As pastas públicas do Exchange usam um design de caixa de correio especializado (em vez de um banco de dados de pasta pública) para armazenar a hierarquia de pastas públicas e o conteúdo da pasta pública. As permissões de pasta pública são gerenciadas por meio do controle de acesso baseado em função (RBAC).
  
As tecnologias de acesso para cliente, como os serviços Web do Exchange (EWS) e a API gerenciada do EWS, oferecem acesso programático à hierarquia de pastas públicas e a itens de conteúdo em um banco de dados de pasta pública. Este artigo fornece informações sobre como você pode usar o EWS e a API gerenciada do EWS para acessar pastas públicas e pastas públicas e dados de pasta pública. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Operações do EWS e métodos da API gerenciada do EWS para acesso à pasta pública
<a name="bk_functionality"> </a>

A maioria das operações do EWS principal dão suporte ao acesso à pasta pública. Você pode usar as operações de item e de pasta e os métodos da API gerenciada do EWS listados na tabela a seguir para trabalhar com pastas públicas.
  
Para obter informações sobre os métodos da API gerenciada do EWS, consulte [EWS Managed API namespaces](https://msdn.microsoft.com/library/jj220535%28v=exchg.80%29.aspx).
  
|**Operação do EWS**|**Método de API gerenciada do EWS**|
|:-----|:-----|
|[Operação CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder. Save ()** <br/> |
|[Operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder. Update ()** <br/> |
|[Operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder. Delete ()** <br/> |
|[Operação](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup> do MoveFolder <br/> |**Folder. Move ()** <br/> |
|[Operação](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup> do CopyFolder <br/> |**Folder. Copy ()** <br/> |
|[Operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder. Bind ()** <br/> |
|[Operação de EmptyFolder](https://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup> <br/> |**Folder. Empty ()** <br/> |
|[Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService. FindFolders ()** <br/> **Folder. FindFolders ()** <br/> |
|[Operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item. Save ()** <br/> |
|[Operação MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item. Move ()** <br/> |
|[Operação CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item. Copy ()** <br/> |
|[Operação UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item. Update ()** <br/> |
|[Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item. Delete ()** <br/> |
|[Operação de FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup> <br/> |**ExchangeService. FindItems ()** <br/> **Folder. FindItems ()** <br/> |
|[Operação GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item. Bind ()** <br/> |
|[Operação convertid](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup> <br/> |**ExchangeService. convertid ()** <br/> **ExchangeService. ConvertIds ()** <br/> |
   
<sup>1</sup> a movimentação de pastas entre uma pasta pública e uma pasta privada não está disponível nas versões do Exchange a partir do Exchange 2013. 
  
<sup>2</sup> esta operação só é aplicável a pastas públicas no exchange Server 2007 e no exchange Server 2010. 
  
<sup>3</sup> essa operação só é aplicável a pastas públicas no Exchange 2010. 
  
<sup>4</sup> a pesquisa indexada de texto completo em uma única pasta pública por meio da opção de pesquisa de QueryString é suportada em versões do Exchange a partir do Exchange 2013. 
  
<sup>5</sup> a operação convertid não converte corretamente identificadores de pasta pública do identificador EWS no identificador de repositório. Você pode atualizar manualmente o identificador que é retornado como uma [solução alternativa](https://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).
  
As operações a seguir não são suportadas ou são parcialmente suportadas para pastas públicas em versões do Exchange a partir do Exchange 2013:
  
- **CopyFolder** (sem suporte). Você pode usar **CreateFolder** com a operação **CopyItems** para implementar a funcionalidade de operação **CopyFolder** . 
    
- **EmptyFolder** (sem suporte). Você pode usar o **FindItem** com a operação **DeleteItem** para implementar a funcionalidade de operação do **EmptyFolder** . 
    
- **MoveFolder** (parcialmente suportado). Não é possível mover pastas entre pastas privadas e públicas. Você pode mover pastas entre pastas privadas e públicas no Exchange 2007 e no Exchange 2010. Você pode mover pastas dentro de uma pasta pública em todas as versões do Exchange. 
    
O EWS e a API gerenciada do EWS não oferecem suporte à seguinte funcionalidade para pastas públicas:
  
- Usando o **SyncFolderHierarchy**. Use as operações **FindFolder**, **GetFolder** e **SyncFolderItems** para sincronizar itens e pastas em uma caixa de correio de pasta pública. 
    
- Pesquisas de passagem profunda de uma hierarquia de pastas públicas. Use as chamadas recursivas de operação do **FindFolder** para percorrer a hierarquia de pastas públicas. 
    
- Usando a operação **createfolderpath** para criar uma hierarquia de pastas para pastas públicas. Você precisará usar a operação **CreateFolder** para cada nível de pasta em uma hierarquia de pastas distintas ao direcionar uma caixa de correio de pasta pública. 
    
- Usando a operação **CreateItem** para salvar cópias de mensagens de email enviadas. Em vez disso, use a operação **MoveItem** para mover uma cópia da mensagem para uma pasta pública. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Cenários para usar o EWS e a API gerenciada do EWS para trabalhar com pastas públicas
<a name="bk_scenarios"> </a>

As pastas públicas permitem vários cenários importantes para usuários de caixa de correio do Exchange. Você pode habilitar usuários usando o EWS e a API gerenciada do EWS para implementar soluções personalizadas para acessar e usar pastas públicas e seu conteúdo. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Acessar programaticamente mensagens de email enviadas para listas de distribuição

Os usuários de caixa de correio do Exchange podem usar pastas públicas para armazenar mensagens de email enviadas a listas de distribuição. Essa é uma maneira conveniente de salvar o histórico de lista de distribuição. Você pode usar a [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) no EWS ou nos métodos **ExchangeService. FindItems ()** e **Folder. FindItems ()** na API gerenciada do EWS para acessar mensagens de email de lista de distribuição armazenadas. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Compartilhar mensagens de email importantes e outros itens de caixa de correio

Os usuários de caixa de correio podem usar pastas públicas como um repositório compartilhado para itens de caixa de correio. Diferentes usuários em uma organização podem compartilhar mensagens de email importantes ou contatos usando pastas públicas. O EWS pode fornecer acesso a esses itens de caixa de correio compartilhada. Você pode usar a [operação MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) no EWS ou o método **Item. Move ()** na API gerenciada do EWS para mover mensagens de email, contatos e outros itens de caixa de correio para dentro e para fora de uma pasta pública. 
  
### <a name="public-discussions-with-post-items"></a>Discussões públicas com itens de postagem

As pastas públicas são um contêiner conveniente para postar itens. Os itens post fornecem uma maneira de usar conversas encadeadas sem ter que enviar mensagens de email entre usuários. Os usuários podem usar pastas públicas e postar itens para hospedar e manter conversas encadeadas entre diferentes usuários de caixa de correio em uma organização. Dessa forma, os usuários de caixa de correio podem acessar o histórico compartilhado de uma conversa que usa itens post, mesmo que eles não sejam parte da conversa. Você pode usar a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) no EWS ou o método **Item. Save ()** na API gerenciada do EWS para criar e responder a itens de postagem armazenados em uma pasta pública. 
  
## <a name="routing-public-folder-requests"></a>Roteamento de solicitações de pasta pública
<a name="bk_routing"> </a>

O conteúdo da pasta pública pode ser armazenado em vários servidores de caixa de correio. A hierarquia de pastas públicas pode ser armazenada em uma caixa de correio, enquanto o conteúdo da pasta pública é armazenado em outra. E cada um desses servidores pode ser diferente do servidor de caixa de correio para o usuário que está solicitando as informações. Nessas situações, é importante incluir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox adicionais em suas solicitações de pasta pública para receber informações precisas sobre pastas públicas.
  
O valor do X-AnchorMailbox e do X-PublicFolderMailbox pode diferir, dependendo se você está executando uma solicitação relacionada à hierarquia de pastas ou ao conteúdo da pasta. A tabela a seguir identifica o procedimento a seguir para cada método da API gerenciada do EWS ou operação do EWS.
  
**Métodos da API gerenciada do EWS e operações do EWS para roteamento de solicitações de pasta pública**

|**Ao chamar esses métodos**|**Ao chamar essas operações**|**Use este procedimento**|
|:-----|:-----|:-----|
|[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Pasta. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Pasta. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder. move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Roteamento de solicitações de hierarquia de pasta pública  <br/> |
|[Item. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item. Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item. move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Roteamento de solicitações de conteúdo de pasta pública  <br/> |
   
## <a name="version-differences"></a>Diferenças de versão
<a name="VersionDifferences"> </a>

No Exchange 2007 e no Exchange 2010, a operação **convertid** funciona como esperado ao converter identificadores de pasta pública do identificador do EWS para o identificador de repositório. 
  
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Limites de pasta pública](https://technet.microsoft.com/library/dn594582%28v=exchg.150%29.aspx)
    
- [Perguntas frequentes: pastas públicas](https://technet.microsoft.com/library/jj552408.aspx)
    
- [Procedimentos de pasta pública](https://technet.microsoft.com/library/jj657481.aspx)
    

