---
title: Sincronização de caixa de correio e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: decf1eee-9743-44f3-9333-b3a01af3683e
description: Descubra como funciona a sincronização de caixa de correio quando você usa o EWS para acessar o Exchange.
ms.openlocfilehash: 7bca2f7b754dcceee99e4bc24519f6e4f6423ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750871"
---
# <a name="mailbox-synchronization-and-ews-in-exchange"></a>Sincronização de caixa de correio e EWS no Exchange

Descubra como funciona a sincronização de caixa de correio quando você usa o EWS para acessar o Exchange.
  
EWS no Exchange usa dois tipos de sincronização para recuperar o conteúdo de caixa de correio e o altera para conteúdo de caixa de correio:
  
- Sincronização de pastas
    
- Sincronização de item
    
Neste artigo, você aprenderá sobre os tipos de sincronização, como funciona a sincronização, os padrões de design de sincronização e práticas recomendadas de sincronização.
  
## <a name="folder-and-item-synchronization"></a>Sincronização de pasta e item
<a name="bk_typesofsyncs"> </a>

Sincronização de pastas sincroniza uma estrutura de pasta, ou a hierarquia de pastas. Sincronização de item sincroniza os itens dentro de uma pasta. Quando você sincroniza itens, você precisa sincronizar cada pasta na caixa de correio de forma independente. Você pode usar o EWS ou a API gerenciada de EWS em seu aplicativo para implementar a pasta e a sincronização de item.
  
**Tabela 1. Operações do EWS e métodos de API gerenciada de EWS para sincronizar pastas e itens**

|**Operação do EWS**|**Método API gerenciada de EWS**|
|:-----|:-----|
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[Método ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[Método ExchangeService.SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
O escopo da sincronização que ocorre será diferente, dependendo se ela for uma inicial ou uma sincronização em andamento, da seguinte maneira:
  
- Uma sincronização inicial sincroniza todas as pastas ou itens no servidor para o cliente. Depois da sincronização inicial, o cliente tem um estado de sincronização que armazena para sincronizações futuras. O estado de sincronização representa todas as alterações no servidor que o servidor de comunicados para o cliente.
    
- Sincronizações em andamento sincronizar os itens ou pastas que foi adicionadas, excluídas ou alteradas desde a sincronização anterior. O servidor usa o estado de sincronização para calcular as alterações a ser relatado no cliente durante cada um dos loops sincronização em andamento.
    
Cada método de sincronização ou a operação retorna uma lista de alterações, e não a pasta real ou mensagem que foi alterado. Alterações em itens e pastas são relatadas por meio dos seguintes tipos de alteração:
  
- Criar — Indica que um novo item ou pasta deve ser criada no cliente.
    
- Atualização — Indica um item ou pasta deve ser alterada no cliente.
    
- Excluir — Indica de que um item ou pasta deve ser excluída no cliente.
    
- ReadStateChange para EWS ou ReadFlagChange para a API gerenciada de EWS — indica que o estado lido do item foi alterado, a partir não lidas para ler ou leitura para não lidas.
    
No Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2010 SP2, os itens e pastas são retornadas na ordem do mais recente para o mais antigo. Nas versões anteriores do Exchange, os itens e pastas são retornadas do mais antigo para o mais recente.
  
## <a name="how-does-ews-synchronization-work"></a>Como funciona a sincronização do EWS?
<a name="bk_howdoesitwork"> </a>

Resumindo, se você estiver sincronizando uma caixa de correio pela primeira vez, use o processo conforme mostrado na Figura 1. Embora você possa usar outras [padrões de design de sincronização](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns), é recomendável essa abordagem para aplicativos escalonáveis.
  
**Figura 1. Padrão de design de sincronização inicial**

![An illustration that shows the initial synchronization design pattern. The client calls SyncFolderHierarchy and Load or GetItem to get the folders, then calls SyncFolderItems and LoadPropertiesForItems or GetItem to get the items in each folder.](media/Exchange2013_SyncInitial.png)
  
Se você estiver usando um estado de sincronização existente no cliente para sincronizar uma caixa de correio, recomendamos que você implemente o padrão de design, conforme mostrado na Figura 2. 
  
**Figura 2. Padrão de design de sincronização em andamento**

![An illustration that shows the ongoing synchronization design pattern. A client receives a notification and then calls SyncFolderHierarchy or SyncFolderItems, gets the properties, then updates the client, or simply updates the read flag on the client.](media/Exchange2013_Sync_Ongoing.png)
  
## <a name="synchronization-design-patterns"></a>Padrões de design de sincronização
<a name="bk_syncpatterns"> </a>

Você pode usar um dos dois padrões de design de sincronização em seu aplicativo para manter as suas caixas de correio atualizado: sincronização baseada em notificação ou a abordagem somente de sincronização.
  
Sincronização de notificação, conforme ilustrado na [Figura 2](mailbox-synchronization-and-ews-in-exchange.md#bk_howdoesitwork), se baseia em notificações para alertar o cliente para fazer uma chamada para os métodos de API gerenciada de EWS [SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) ou [SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) ou o EWS [SyncFolderHierarchy ](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)ou [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operações. Esse tipo de sincronização geralmente é recomendado para aplicativos escalonáveis, mas talvez não seja a melhor abordagem para todos. Sincronização baseada em notificação tem a vantagem a seguir: 
  
- As notificações são otimizadas para reduzir chamadas para o banco de dados do Exchange de back-end. Assinaturas e filas de evento são gerenciadas por servidor caixa de correio (ou o servidor de acesso para cliente do Exchange 2010 e Exchange 2007); No entanto, o gerenciamento dos eventos e inscrições usa menos recursos que a alternativa, o que é mais frequentes chamadas de sincronização no banco de dados do Exchange. Além disso, o Exchange tem específico [políticas de limitação](ews-throttling-in-exchange.md) para notificações e inscrições proteger o consumo de recursos. 
    
No entanto, também existem algumas desvantagens para usando a sincronização com base em notificação:
  
- As notificações são com ruído porque a maioria dos cenários envolvem várias notificações de tentativa de um usuário. Isso acontece principalmente da pasta Calendário. Por exemplo, quando uma solicitação de reunião único é recebida, várias notificações de item e pasta são criadas, incluindo uma notificação para criar o item e outro para modificar o item. Uma maneira para atenuar esse obstáculo é criar um atraso de alguns segundos na sua chamada de [carga](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceobject.load%28v=exchg.80%29.aspx), [LoadPropertiesForItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.loadpropertiesforitems%28v=exchg.80%29.aspx), [GetItem](http://msdn.microsoft.com/en-us/library/exchange/aa565934%28v=exchg.150%29.aspx.aspx)ou [GetFolder](http://msdn.microsoft.com/en-us/library/exchange/aa580274%28v=exchg.150%29.aspx.aspx) . No caso de uma solicitação de reunião, se você tiver feito chamadas para a operação **GetItem** imediatamente, você pode ter uma chamada para criar o item e outro para modificar o item. Em vez disso, atrasando a chamada, você pode chamar a operação **GetItem** uma vez e fazer as alterações que abrangem a criação e a modificação do item ao mesmo tempo. 
    
- As notificações são enfileiradas no servidor de caixa de correio e assinaturas são salvas no servidor de caixa de correio. Se o servidor de caixa de correio que gerencia a assinatura não estiver disponível, você perde quaisquer novas notificações, sua caixa de correio não sincronizar e você precisará inscrever-se novamente para as notificações.
    
- Você precisará planejar estratégias de redução de risco que as notificações de falham. Dessa forma, a segunda abordagem, o padrão de design somente sincronização, é mais resiliente de sincronização de notificação, pois só requer que o cliente manter o estado de sincronização — não existem problemas com afinidade no servidor de caixa de correio Gerenciando a assinatura.
    
Se implementado conforme recomendado, o padrão de design de assinatura com base em notificação se baseia em: 
  
- Notificações para determinar *quando* os dados alterados. 
    
- A API gerenciada de EWS **SyncFolderHierarchy** ou **SyncFolderItems** métodos, ou o EWS **SyncFolderHierarchy** ou operações **SyncFolderItems** para determinar *quais* alterado, otimização do número de eventos de sincronização retornados. Foi um novo item criado, atualizado ou excluído? Isso é tudo o que você precisa saber a partir desses métodos, não contam-los para a lista de propriedade de alterações. (Não fazer uma chamada de **LoadPropertiesForItems** em todos os itens ou pastas retornadas de **GetItem** ou). 
    
- Usando os métodos de **carga** ou **LoadPropertiesForItems** em operação o EWS **GetItem** ou a API gerenciada de EWS para determinar *como* os dados alterados e para recuperar as propriedades do servidor conforme necessário, organizar solicitações em lote com base a quantidade de dados que serão retornadas. Isso é seguido por uma comparação das propriedades no cliente e aqueles retornados acabou de servidor e, por fim, a criação, exclusão ou modificação do item ou pasta no cliente. 
    
A abordagem somente sincronização depende inteiramente os métodos **SyncFolderItems** e **SyncFolderHierarchy** EWS Managed API, ou o **SyncFolderHierarchy** ou **SyncFolderItems** EWS operações, que você pode chamar ou continuamente, ou como um evento cronometrado. Há prós e contras para essa opção também. A abordagem somente sincronização é mais resiliente, como o estado de sincronização é armazenado no cliente a nível de caixa de correio e uma relação exclusiva entre o estado de sincronização e qualquer servidor caixa de correio que mantém a assinatura de notificação não é necessário. A abordagem de sincronização pode sobreviver um failover de caixa de correio devido à sua independência do servidor de caixa de correio. No entanto, a abordagem de sincronização aumenta a latência para o usuário porque os itens são sincronizados em uma base cronometrada ou intermitente — não em tempo real quando itens chegarem. Essa abordagem também é mais cara, porque você está fazendo chamadas para o banco de dados do Exchange quando é possível que nenhuma alteração tenha ocorrido. 
  
## <a name="synchronization-best-practices"></a>Práticas recomendadas de sincronização
<a name="bk_bestpractices"> </a>

Para aplicativos altamente escalonáveis, recomendamos que você aplique as seguintes práticas recomendadas para sincronizar as caixas de correio em seu aplicativo:
  
- Ao chamar o método API gerenciada de EWS **SyncFolderItems** ou **SyncFolderHierarchy** use o valor de _IdOnly_ para o parâmetro _propertySet_ ou ao usar o EWS **SyncFolderHierarchy** ou **SyncFolderItems** operações usam o valor de **IdOnly** para o valor de [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) para reduzir chamadas para o banco de dados do Exchange. As propriedades mais você solicitar no conjunto de propriedade do **SyncFolderItems** ou **SyncFolderHierarchy** chamada, o back-end mais chamadas são criadas. Uma nova chamada RPC é feita para cada valor da propriedade solicitada, enquanto que apenas uma chamada RPC é feita para recuperar todas as **ItemIds** para uma solicitação - não importa o número de resultados ao relatório. Para uma solicitação de **IdOnly** resulta na chamada de um banco de dados, enquanto uma solicitação de recipiente de propriedade para o assunto e o remetente resulta em três chamadas de banco de dados: um para o **assunto**, um para o **remetente**e outro para o **ItemId**.
    
- Não chame os métodos EWS Managed API de **carga** ou **LoadPropertiesForItems** , ou o EWS **GetItem** ou **GetFolder** operações, em cada item em uma resposta de sincronização. Em vez disso, analisar os resultados; como procurar por alterações que não exigem a todas as propriedades a serem recuperados, leia as alterações de estado. Se uma resposta inclui uma alteração de estado de leitura, apenas atualizar o sinalizador no cliente e terminar; Não há necessidade para obter todas as propriedades do item. E certifique-se de que você não duplique esforço fazendo alterações que originou a partir do mesmo cliente. Por exemplo, se a resposta de sincronização inclui a exclusão de um item e a exclusão ocorreu no cliente local, você não precisa excluir a mensagem novamente ou obter todas as propriedades para esse item. 
    
- Evite obtendo limitadas, fazendo o seguinte:
    
  - Quando você chama o método de API gerenciada de EWS **LoadPropertiesForItems** ou a operação de EWS **GetItem** para obter os itens em um lote, não batch muitos itens em sua solicitação; Caso contrário, talvez você obtenha [limitadas](ews-throttling-in-exchange.md). Recomendamos que você inclua 10 itens por lote.
    
  - Não fizer muitas solicitações em um tempo muito curto. Isso irá também causar limitação e aumentar o tempo de resposta, em vez de diminuir a ele. 
    
  - Se você estiver processamento em lotes itens, todos os itens com os mesmos valores para os atributos **Id** e **ChangeKey** do elemento [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) de lote. 
    
  - Se você obter limitadas, pare enviando solicitações. Solicitações de reenvio será prolongar os esforços de recuperação. Em vez disso, aguarde a tempo de expiração de retirada e tente enviar suas solicitações de sincronização novamente.
    
- Dependendo do tipo de [evento de notificação](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_eventtypes) recebido: 
    
  - Para eventos **NewMail** ou **modificado** , chamar o método API gerenciada de EWS **SyncFolderItems** ou a operação de EWS **SyncFolderItems** porque notificações não fornecem um **ChangeKey**e notificações não chamar estado lido alterações.
    
  - Para eventos **Deleted** , se a assinatura de notificação esteve ativa antes de sincronizar o anterior, exclua o evento localmente. Você não precisará chamar o método API gerenciada de EWS **SyncFolderItems** ou a operação de EWS **SyncFolderItems** imediatamente após a exclusão. 
    
  - Se um evento **modificado** foi causado por uma alteração de estado de leitura, não chamar o método API gerenciada de EWS **LoadPropertiesForItems** ou a operação de EWS **GetItem** , basta alterar o sinalizador no item. 
    
- Quando a sincronização de dados de calendário, faça o seguinte:
    
  - Use uma abordagem semelhante à sincronização baseada na notificação. Porque **SyncFolderItem** não incluir qualquer lógica de calendário, use o método API gerenciada de EWS [FindAppointments](http://msdn.microsoft.com/en-us/library/dd633767%28v=exchg.80%29.aspx) , ou o EWS [FindItem operação](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) com o elemento de [exibição de calendário](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) para exibir compromissos entre duas datas e depois Chame o método API gerenciada de EWS **LoadPropertiesForItems** ou a operação de EWS **GetItem** para recuperar as propriedades do item para o item de calendário. 
    
  - Não pesquise usando o método API gerenciada de EWS **FindAppointments** ou a operação de EWS **FindItem** com um elemento de **exibição de calendário** . 
    
- Quando a sincronização das pastas de pesquisa:
    
  - Use uma abordagem semelhante à sincronização baseada na notificação. 
    
  - Use notificações para determinar quando os dados são alterados.
    
  - Porque você não pode usar **SyncFolderItem** em uma pasta de pesquisa, use um método de API gerenciada de EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) classificado e paginado ou EWS **FindItem** operação com o conjunto de elemento [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx) e [SortOrder](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) , para determinar o que mudou. 
    
  - Use o método de API gerenciada de EWS **LoadPropertiesForItems** ou a operação de EWS **GetItem** para recuperar dados. 
    
## <a name="filtered-synchronization"></a>Sincronização filtrada
<a name="bk_filteredsync"> </a>

O método de API gerenciada de EWS **SyncFolderItems** e a operação de EWS **SyncFolderItems** permitem que você ignorar itens específicos, com base em suas ItemIds, definindo o parâmetro _ignoreItemIds_ no EWS Managed API ou a [Ignorar](http://msdn.microsoft.com/library/7789eec5-ceec-43f2-84d5-d0d15b734076%28Office.15%29.aspx) elemento no EWS. Isso é ideal quando, por exemplo, indivíduos começam responder a todos em uma mensagem de email enviada para todos na empresa. 
  
Você pode imaginar, posso Minhas notificações de filtro (e, portanto, somente acionar sincronização) se alteram propriedades específicas? Embora que parecem razoável, pois as inscrições de notificação baseiam-se ao tipo de alteração (criar, atualizar e excluir), e não a propriedade que está sendo atualizada, não é possível filtrar notificações dessa maneira. Em vez disso, você pode fazer o seguinte:
  
- Use o padrão de design de assinatura com base em notificação.
    
- Chame os métodos de **SyncFolderHierarchy** e a API gerenciada de EWS **SyncFolderItems** repetidamente com o parâmetro _propertySet_ definido como _IdOnly_ para tornar seu estado de sincronização atual. Ou, se usando o EWS, chamar o **SyncFolderHierarchy** e operações **SyncFolderItems** repetidamente com o valor de **BaseShape** definido como **IdOnly**. 
    
- Descartar a resposta (não analisá-lo ou fazer comparações qualquer propriedade).
    
- Use o método API gerenciada de EWS **FindItems** ou a operação de EWS **FindItem** e classificação e página para pré-preencher os itens do escopo filtrada que você se preocupar. 
    
- Use o seu estado de sincronização para continuar a chamar o método API gerenciada de EWS **SyncFolderItems** ou a operação de EWS **SyncFolderItems** , mas apenas monitorar as alterações no conjunto filtrado de item. Se novos itens forem criados, você terá que ver se esses novos itens estão dentro de seu escopo filtrado. 
    
## <a name="in-this-section"></a>Nesta seção
<a name="bk_filteredsync"> </a>

- [Sincronizar pastas usando o EWS no Exchange](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Sincronizar itens usando o EWS no Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [Tratando erros relacionados a sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Método SyncFolderItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx)
    
- [Método SyncFolderHierarchy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx)
    
- [Operação SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)
    
- [Operação SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx)
    

