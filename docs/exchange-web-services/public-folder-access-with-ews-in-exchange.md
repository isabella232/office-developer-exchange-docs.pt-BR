---
title: Acessar pastas públicas com EWS no Exchange
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Saiba mais sobre como usar o EWS e a API gerenciada de EWS para acessar pastas públicas e rotear as solicitações de pasta pública no Exchange.
ms.openlocfilehash: cfa089ba617dc760ed12883590e141debb5ecd9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750952"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Acessar pastas públicas com EWS no Exchange

Saiba mais sobre como usar o EWS e a API gerenciada de EWS para acessar pastas públicas e rotear as solicitações de pasta pública no Exchange.
  
Pastas públicas fornecem um repositório compartilhado de itens que os usuários em sua organização podem acessar. O Office 365, Exchange Online e a versões locais do Exchange, começando com o Exchange 2013 introduzem uma nova arquitetura de pastas públicas. Pastas públicas no Exchange usam um design de caixa de correio especializados (em vez de um banco de dados de pasta pública) para armazenar o conteúdo de pasta pública e a hierarquia de pastas públicas. Permissões de pastas públicas são gerenciadas por meio de função com base em acesso de controle (RBAC).
  
Tecnologias de acesso de cliente, como serviços Web do Exchange (EWS) e a API gerenciada de EWS, fornecem acesso programático aos itens de conteúdo em um banco de dados de pasta pública e a hierarquia de pastas públicas. Este artigo fornece informações sobre como você pode usar o EWS e a API gerenciada de EWS para acessar pastas públicas e as pastas públicas e dados de pasta pública. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Operações do EWS e métodos de API gerenciada de EWS para acesso de pasta pública
<a name="bk_functionality"> </a>

A maioria das operações EWS core oferecer suporte ao acesso de pasta pública. Você pode usar as operações de pasta e item e os métodos de API gerenciada de EWS listados na tabela a seguir para trabalhar com pastas públicas.
  
Para obter informações sobre métodos de API gerenciada de EWS, consulte [namespaces de API gerenciada de EWS](http://msdn.microsoft.com/en-us/library/jj220535%28v=exchg.80%29.aspx).
  
|**Operação do EWS**|**Método API gerenciada de EWS**|
|:-----|:-----|
|[Operação CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder.Save()** <br/> |
|[Operação UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder.Update()** <br/> |
|[Operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder.Delete()** <br/> |
|[Operação MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <sup>1</sup> <br/> |**Folder.Move()** <br/> |
|[Operação CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <sup>2</sup> <br/> |**Folder.Copy()** <br/> |
|[Operação GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder.Bind()** <br/> |
|[Operação EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <sup>3</sup> <br/> |**Folder.Empty()** <br/> |
|[Operação FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService.FindFolders()** <br/> **Folder.FindFolders()** <br/> |
|[Operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item.Save()** <br/> |
|[Operação MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item.Move()** <br/> |
|[Operação CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item.Copy()** <br/> |
|[Operação UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item.Update()** <br/> |
|[Operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item.Delete()** <br/> |
|[Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <sup>4</sup> <br/> |**ExchangeService.FindItems()** <br/> **Folder.FindItems()** <br/> |
|[Operação GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item.Bind()** <br/> |
|[Operação ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) <sup>5</sup> <br/> |**ExchangeService.ConvertId()** <br/> **ExchangeService.ConvertIds()** <br/> |
   
<sup>1</sup> a movimentação de pastas entre uma pasta pública e privada pasta não está disponível nas versões do Exchange, começando com o Exchange 2013. 
  
<sup>2</sup> essa operação só é aplicável a pastas públicas no Exchange Server 2007 e o Exchange Server 2010. 
  
<sup>3</sup> essa operação só é aplicável a pastas públicas no Exchange 2010. 
  
<sup>4</sup> a pesquisa de texto completo indexado dentro de uma única pasta pública por meio da opção de pesquisa QueryString é suportada nas versões do Exchange, começando com o Exchange 2013. 
  
<sup>5</sup> ConvertId a operação não converter corretamente os identificadores de pasta pública do identificador EWS para o identificador do repositório. Você pode atualizar manualmente o identificador retornado como uma [solução alternativa](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).
  
As operações a seguir não são suportadas ou são parcialmente suportadas, para pastas públicas em versões do Exchange, começando com o Exchange 2013:
  
- **CopyFolder** (não são suportados). Você pode usar **CreateFolder** com a operação **CopyItems** para implementar a funcionalidade de operação **CopyFolder** . 
    
- **EmptyFolder** (não são suportados). Você pode usar **FindItem** com a operação **DeleteItem** para implementar a funcionalidade de operação **EmptyFolder** . 
    
- **MoveFolder** (parcialmente suportado). Você não pode mover pastas entre pastas públicas e privadas. Você pode mover pastas entre pastas públicas e privadas no Exchange 2007 e Exchange 2010. Você pode mover pastas dentro de uma pasta pública em todas as versões do Exchange. 
    
EWS e a API gerenciada de EWS não suportam a funcionalidade a seguir para pastas públicas:
  
- Usando **SyncFolderHierarchy**. Use as operações **FindFolder**, **GetFolder** e **SyncFolderItems** para sincronizar itens e pastas em uma caixa de correio de pasta pública. 
    
- Pesquisas de profunda-passagem de uma hierarquia de pasta pública. Chamadas de operação uso recursivas **FindFolder** para percorrer a hierarquia de pasta pública. 
    
- Usando a operação **CreateFolderPath** para criar uma hierarquia de pastas para pastas públicas. Você precisará usar a operação de **CreateFolder** para cada nível de pasta em uma hierarquia de pasta distintos quando você uma caixa de correio de pasta pública de destino. 
    
- Usando a operação **CreateItem** para salvar cópias das mensagens de email enviado. Em vez disso, use a operação **MoveItem** para mover uma cópia da mensagem para uma pasta pública. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Cenários para usar o EWS e a API gerenciada de EWS para trabalhar com pastas públicas
<a name="bk_scenarios"> </a>

Pastas públicas habilitar muitos cenários importantes para os usuários de caixa de correio do Exchange. Você pode capacitar os usuários usando o EWS e a API gerenciada de EWS para implementar soluções personalizadas para acessar e usar pastas públicas e seus conteúdos. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Programaticamente acesso emails que foram enviados para listas de distribuição

Usuários de caixa de correio do Exchange podem usar pastas públicas para armazenar mensagens de email enviadas para listas de distribuição. Essa é uma maneira conveniente para salvar o histórico da lista de distribuição. Você pode usar a [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) no EWS ou os métodos **ExchangeService.FindItems()** e **Folder.FindItems()** na API gerenciada do EWS para acessar mensagens de email de lista de distribuição armazenado. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Compartilhar mensagens de email importantes e outros itens de caixa de correio

Usuários de caixa de correio podem usar pastas públicas como um repositório compartilhado para itens de caixa de correio. Diferentes usuários em uma organização podem compartilhar mensagens de email importantes ou contatos usando pastas públicas. EWS pode fornecer o acesso aos seguintes itens de caixa de correio compartilhada. Você pode usar a [operação MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) no EWS ou o método **Item.Move()** na API gerenciada do EWS para mover mensagens de email, contatos e outros itens de caixa de correio e sair de uma pasta pública. 
  
### <a name="public-discussions-with-post-items"></a>Discussões públicas com itens de postagem

Pastas públicas são um contêiner conveniente para itens de postagem. Itens de postagem fornecem uma maneira de usar conversas encadeadas sem precisar enviar mensagens de email entre usuários. Os usuários podem usar pastas públicas e postar itens para hospedar e manter encadeadas conversas entre usuários de caixa de correio diferentes em uma organização. Dessa forma, os usuários de caixa de correio podem acessar o histórico compartilhado de uma conversa que usa lança itens, mesmo que eles não faziam parte da conversa. Você pode usar a [operação CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) no EWS ou o método **Item.Save()** na API gerenciada do EWS ao criar e responder para postar itens armazenados em uma pasta pública. 
  
## <a name="routing-public-folder-requests"></a>Roteamento de solicitações de pasta pública
<a name="bk_routing"> </a>

Conteúdo de pastas públicas pode ser armazenado em vários servidores de caixa de correio. A hierarquia de pasta pública pode ser armazenada em uma caixa de correio, enquanto o conteúdo da pasta pública está armazenado em outro. E cada um desses servidores pode ser diferente do que o servidor de caixa de correio para o usuário que está solicitando as informações. Nesses casos, é importante incluir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox adicionais em suas solicitações de pasta pública para receber informações precisas sobre pastas públicas.
  
O valor para o X-AnchorMailbox e X-PublicFolderMailbox diferem, dependendo se você estiver realizando uma solicitação relacionada a hierarquia da pasta ou o conteúdo da pasta. A tabela a seguir identifica o procedimento a seguir para cada método de API gerenciada de EWS ou a operação do EWS.
  
**Métodos de API gerenciada de EWS e operações de EWS para rotear solicitações de pasta pública**

|**Ao chamar esses métodos**|**Ao chamar essas operações**|**Use este procedimento**|
|:-----|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Rotear solicitações de hierarquia de pasta pública  <br/> |
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Roteamento de solicitações de conteúdo de pasta pública  <br/> |
   
## <a name="version-differences"></a>Diferenças de versão
<a name="VersionDifferences"> </a>

No Exchange 2007 e Exchange 2010, a operação de **ConvertId** funciona conforme o esperado, ao converter o identificador do EWS identificadores de pasta pública para o identificador do repositório. 
  
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Limites de pastas públicas](http://technet.microsoft.com/en-us/library/dn594582%28v=exchg.150%29.aspx)
    
- [Perguntas Frequentes: Pastas públicas](http://technet.microsoft.com/en-us/library/jj552408.aspx)
    
- [Procedimentos de pasta pública](http://technet.microsoft.com/en-us/library/jj657481.aspx)
    

