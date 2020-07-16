---
title: Limitação do EWS no Exchange
manager: sethgros
ms.date: 05/10/2019
ms.audience: Developer
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Saiba mais sobre as políticas de limitação que afetam o EWS quando você está usando o Exchange.
localization_priority: Priority
ms.openlocfilehash: 0c6ac49629ad4cdb4419cc8638d8e60ecb6509d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455398"
---
# <a name="ews-throttling-in-exchange"></a>Limitação do EWS no Exchange

Saiba mais sobre as políticas de limitação que afetam o EWS quando você está usando o Exchange.

**Fornecido por:** Glen escalas; Michael principal, Microsoft Corporation

O artigo fornece informações sobre a limitação de EWS no Exchange Online, o Exchange Online como parte do Office 365 e versões locais do Exchange a partir do Exchange 2010. A limitação no Exchange ajuda a garantir a confiabilidade e o tempo de atividade do servidor, limitando a quantidade de recursos do servidor que um único usuário ou aplicativo pode consumir. A limitação é uma resposta reativa para o uso em excesso dos recursos do sistema que podem afetar a confiabilidade e a funcionalidade do serviço. O Exchange monitora constantemente os recursos de infraestrutura crítica, como os bancos de dados de caixa de correio. Quando são detectados fatores de alta carga que diminuem o desempenho desses recursos, as conexões do EWS são limitadas de maneira proporcional com base no valor que cada chamador contribuiu para esta condição de alta carga. O resultado é que um usuário pode estar dentro de seu limite de limitação e ainda ter lentidão até que a integridade do recurso volte aos níveis operacionais.

Cada protocolo de acesso para cliente no Exchange, incluindo o EWS, tem uma política de limitação. Ao projetar aplicativos que usam o EWS, é importante considerar políticas de limitação para ajudar a garantir a confiabilidade do aplicativo e a integridade do seu servidor Exchange. Este artigo identifica as diferentes políticas de limitação e limites de serviço do EWS, se você está direcionando para o Exchange Online ou versões do Exchange no local, a partir do Exchange Server 2010. Como aplicável, este artigo também identifica as diferenças em políticas de limitação em diferentes versões do Exchange.

> [!IMPORTANT]
> A política de limitação padrão, o acesso à política de limitação e a configuração de política de limitação difere entre o Exchange Online e o Exchange local. Os valores de configuração de limitação específicos só são precisos para uma versão específica do Exchange. Como os valores de configuração variam entre as versões, e como os administradores do Exchange podem alterar as políticas de limitação padrão para implantações locais, este artigo não fornece os valores de configuração padrão. É mais importante ter em mente as considerações para projetar um aplicativo que funcione dentro de limites de limitação e reage de forma adequada aos cenários de limitação.

Se você é um desenvolvedor de aplicativos, você precisa limitar o fator para o design do aplicativo. Versões diferentes do Exchange têm valores padrão diferentes para os parâmetros de limitação do EWS. Os aplicativos de cliente e de serviço projetados para acessar versões diferentes do Exchange precisarão considerar essas configurações, se são valores padrão, valores personalizados definidos por um administrador do Exchange ou, como para o Exchange Online, definidos por padrão e não detectáveis. Como os valores do parâmetro throttling não podem ser descobertos programaticamente, suas especificações de design de cliente devem incluir um plano para que o aplicativo se adapte a diferentes limites de limitação potenciais. Quando você projeta aplicativos de vários threads que acessarão um grande número de caixas de correio ou quando muitos clientes estiverem acessando a mesma caixa de correio, considere os limites de simultaneidade que a política padrão aplica ao Exchange.

## <a name="throttling-policies-that-affect-ews"></a>Limitação de políticas que afetam o EWS

As políticas de limitação no Exchange afetam não apenas o EWS, mas também todas as conexões de cliente com o servidor Exchange, incluindo os protocolos usados pelo Office Outlook, Outlook Web App e Exchange ActiveSync.

A política de limitação do **CPUStartPercent** pode afetar o desempenho do EWS quando você estiver executando o Exchange 2010. Quando a utilização média da CPU dos processos do Exchange em execução no servidor de acesso para cliente, incluindo, mas não limitado a, o processo EWS, exceder o valor especificado por essa política, as solicitações de entrada serão atrasadas para reduzir a utilização da CPU. Você não pode alterar o valor dessa política, mas conhecer isso pode ajudá-lo a solucionar problemas de desempenho. A lógica de amostragem que o servidor de acesso para cliente executa para esse valor é uma média em uma janela de 10 segundos de rolagem. Isso permite que o processo responda apropriadamente aos picos rápidos de utilização da CPU. Quando esse limite for excedido, as conexões de entrada para o EWS serão atrasadas. Esse atraso é limitado em 500 milissegundos (MS) em um uso de CPU 100 teórico por solicitação do EWS. Se uma solicitação de EWS de lote para obter 100 itens for passada, o servidor verificará o uso da CPU 100 vezes (uma vez por item) para obter um atraso máximo de 50 segundos. O tempo de atraso é linearmente proporcional ao uso da CPU. Em **CPUStartPercent**, o atraso é 0 (um segmento de rendimento) e aumenta linearmente até 500 mseg em 100% uso da CPU. Como as políticas de limitação se aplicam a todos os usuários do Exchange, é improvável que o uso da CPU exceda o limite **CPUStartPercent** em um servidor de acesso para cliente do Exchange, pois os usuários ou aplicativos individuais não podem obter utilização de CPU suficiente para afetar a operação do servidor.

A tabela a seguir lista os parâmetros de política de limitação que afetam os aplicativos que usam o EWS.

**Tabela 1: limitação dos parâmetros da política que afetam o EWS**

|**Nome do parâmetro de política de limitação**|**Aplica-se a**|**Descrição**|
|:-----|:-----|:-----|
|**DiscoveryMaxConcurrency** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de conexões simultâneas de pesquisa de descoberta que um usuário pode ter ao mesmo tempo.  <br/> |
|**DiscoveryMaxKeywords** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de palavras-chave que um usuário pode incluir em uma pesquisa de descoberta.  <br/> |
|**DiscoveryMaxKeywordsPerPage** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de palavras-chave para as quais as estatísticas serão mostradas.  <br/> |
|**DiscoveryMaxMailboxes** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de caixas de correio de origem que um usuário pode incluir em uma pesquisa de descoberta.  <br/> |
|**DiscoveryMaxMailboxesResultsOnly** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de caixas de correio que você pode pesquisar em uma pesquisa de descoberta eletrônica in-loco sem poder exibir as estatísticas.  <br/> |
|**DiscoveryPreviewSearchResultsPageSize** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de mensagens retornadas em uma resposta de visualização da pesquisa de descoberta eletrônica.  <br/> |
|**EwsCutoffBalance** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define os limites de consumo de recursos para o usuário EWS antes que o usuário seja bloqueado completamente para executar operações em um componente específico.  <br/> |
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define a quantidade de tempo que um usuário do EWS pode consumir um valor elevado de recursos antes de ser limitado. Isso é medido em milissegundos. Esse valor é definido separadamente para cada componente.  <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define a taxa na qual o orçamento de um usuário do EWS é recarregado (o orçamento aumenta por) durante o tempo do orçamento.  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número máximo de assinaturas ativas de envio, recepção e transmissão de fluxo contínuo que um usuário pode ter em um servidor de acesso para cliente específico ao mesmo tempo. Isso é orçado de modo diferente para diferentes versões do Exchange.  <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |Define a quantidade de tempo, em segundos, que pesquisas rápidas feitas usando a pesquisa do Exchange no EWS continuam antes de expirarem. Pesquisas rápidas são pesquisas feitas usando uma cadeia de caracteres de consulta de sintaxe de consulta avançada (AQS) em uma [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).  <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número máximo de itens de uma [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) ou [FindFolder operação](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) que pode existir na memória do servidor de acesso para cliente de uma vez para um usuário. O valor padrão para essa propriedade é 1000. O [valor de fallback](https://technet.microsoft.com/library/dd297964%28v=exchg.141%29.aspx#fallback)para esse valor é 1000.  <br/> No Exchange Online e nas versões locais do Exchange a partir do Exchange 2013, esta política de limitação não pode ser consultada ou configurada por um cmdlet. No Exchange Online e nas versões locais do Exchange a partir do Exchange 2013, a pesquisa do EWSFindCountLimit para [AQS](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) e qualquer pesquisa do Exchange com uma restrição é de 250 resultados. Uma pesquisa do Exchange sem uma restrição retornará até 1000 resultados.  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante a qual um usuário específico pode executar solicitações do Active Directory.  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante a qual um usuário específico pode executar o código do servidor de acesso para cliente.  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante a qual um usuário específico pode executar solicitações RPC de caixa de correio  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número de conexões simultâneas abertas que um usuário específico pode ter em relação a um servidor do Exchange que usa o EWS de uma só vez. O valor padrão para o Exchange 2010 é 10. O valor padrão para o Exchange 2013 e o Exchange Online é 27.  <br/> Esta política se aplica a todas as operações, exceto para notificações de streaming. Notificações de streaming use o **HangingConnectionLimit** para indicar o número de conexões de eventos de streaming abertas que estão disponíveis. Para obter mais informações, consulte [que valores de limitação Eu preciso considerar?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número de mensagens por minuto que podem ser enviadas.  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o limite para o número de destinatários que um usuário pode endereçar em um período de 24 horas.  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o limite para o número de destinatários para ações de encaminhamento/redirecionamento de caixa de entrada em um período de 24 horas.  <br/> |
|**ConcurrentSyncCalls** <br/> |Exchange 2019  <br/> Exchange 2016  <br/> Exchange Online  <br/> |Define o limite para o número de chamadas de sincronização simultâneas (SyncFolderHierarchy, SyncFolderItems) para um usuário. <br/> |

> [!CAUTION]
> Não defina as políticas de limitação como **NULL**. Isso definirá a política para um valor igual a ilimitado, o que indica que uma política de limitação não está definida.

## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Exibindo as políticas que se aplicam às caixas de correio do Exchange

O Exchange local fornece cmdlets do Shell de gerenciamento do Exchange que você pode usar para definir e obter a política de limitação. O Exchange Online não fornece acesso aos cmdlets da política de limitação.

Você pode usar os cmdlets a seguir para exibir as políticas de limitação para uma implantação local do Exchange Server:

- **Get-ThrottlingPolicy** — Obtém as configurações de limitação de cliente para uma ou mais políticas de limitação. Para obter mais informações, consulte [Get-ThrottlingPolicy](https://technet.microsoft.com/library/dd351264.aspx) no TechNet.

- **Get-ThrottlingPolicyAssociation** — permite que você visualize a relação entre um objeto e suas políticas de limitação associadas. O objeto pode ser um usuário com uma caixa de correio, um usuário sem uma caixa de correio ou um contato. Para obter mais informações, consulte [Get-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459241.aspx) no TechNet.

Use o seguinte comando para mostrar a política de limitação padrão para o Exchange 2010.

**Get-ThrottlingPolicy | Em que-Object {$ _. IsDefault-EQ "true"} | Format-List**

Use o seguinte comando para mostrar a política de limitação global (que equivale à política de limitação padrão no Exchange 2010) no Exchange 2013.

**Get-ThrottlingPolicy | Em que-Object {$ _. ThrottlingPolicyScope-EQ "global"} | Format-List**

Use o seguinte comando para mostrar a política de limitação associada a um usuário no Exchange 2010 ou no Exchange 2013. Substitua o nome de usuário john@contoso.com pelo nome de usuário do usuário de destino para o qual você deseja obter informações de política de limitação.

**Get-ThrottlingPolicyAssociation john@contoso.com | Format-List**

A execução desse comando no Shell de gerenciamento do Exchange resulta em uma saída semelhante à seguinte.

```powershell
PS C:\>Get-ThrottlingPolicyAssociation john@contoso.com
RunspaceId               : 72153d6-9dce-2fae-8dbd-5ca5f760g2df
ObjectId                 : john
ThrottlingPolicyId       :
Name                     : john
Identity                 : FHXB-28178dom.contoso.com/Users/john
IsValid                  : True
NeedsToSuppressPii       : False
ExchangeVersion          : 0.10 (15.0.0.0)
DistinguishedName        : CN=john,CN=Users,DC=FHXB-28178dom,DC=contoso,DC=com
Guid                     : 2c10dab6-de28-1937-ad8g-535832613a08
```

> [!NOTE]
> Quando a propriedade **ThrottlingPolicyId** está em branco, a política padrão é aplicada à caixa de correio.

Você pode definir a política de limitação em um servidor do Exchange usando os cmdlets [Set-ThrottlingPolicy](https://technet.microsoft.com/library/dd298094.aspx) e [Set-ThrottlingPolicyAssociation](https://technet.microsoft.com/library/ff459231.aspx) . Você pode criar e remover políticas de limitação não padrão usando os cmdlets [New-ThrottlingPolicy](https://technet.microsoft.com/library/dd351045.aspx) e [Remove-ThrottlingPolicy](https://technet.microsoft.com/library/dd351178.aspx) .

> [!TIP]
> Recomendamos que você projete seus aplicativos para aderir à política de limitação padrão. Só faça alterações nas políticas de limitação padrão se o design do aplicativo cliente não puder acomodar a política padrão. Lembre-se de que as políticas de limitação menos restritivas podem afetar negativamente a confiabilidade do serviço.

## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>Considerações de limitação para aplicativos que usam a representação do EWS

[Representação](impersonation-and-ews-in-exchange.md) é um método de autorização que permite que uma única conta acesse muitas contas. Quando uma conta de serviço representa usuários, ela atua como os usuários e, portanto, supõe os direitos atribuídos a esses usuários. Os arquivos de log registram o acesso como o usuário representado. Os administradores usam o controle de acesso baseado em função (RBAC) para configurar a representação por meio do Shell de gerenciamento do Exchange.

Quando a representação é usada, os orçamentos de todos os limites de limitação se aplicam de forma diferente, dependendo da versão do Exchange. O orçamento é calculado em relação à conta representada ou à conta de serviço. Se seu aplicativo é multi-threaded e faz solicitações simultâneas em várias caixas de correio, você deve considerar como o limite de limitação afetará o desempenho do aplicativo. Em geral, esteja ciente dos seguintes limites de contas de serviço quando você cria um aplicativo baseado em serviço que usa representação para acessar todas as caixas de correio:

- Quando você usa a representação, a conta de serviço tem um orçamento separado para os seguintes parâmetros de política:

  - **EWSMaxConcurrency**

  - **EWSPercentTimeInAD**

  - **EWSPercentTimeInCAS**

  - **EWSPercentTimeInMailboxRPC**

  - **EWSMaxSubscriptions**

  - **EWSFastSearchTimeoutInSeconds**

  - **EWSFindCountLimit**

- O orçamento **EWSMaxConcurrency** é compartilhado para a conta de serviço e a conta que está sendo representada para todas as conexões com as versões do Exchange anteriores ao Exchange 2010 Service Pack 2 (SP2) Update Rollup 4 (RU4). Começando com o Exchange 2010 SP2 RU4 e incluindo o Exchange Online, o acesso à conta de serviço usa um orçamento separado do orçamento **EWSMaxConcurrency** do usuário. Para obter mais informações sobre a atualização da política de limitação de conexão simultânea do Exchange para o EWS, consulte [Descrição do pacote cumulativo de atualizações 4 para o Exchange Server 2010 Service Pack 2](https://support.microsoft.com/kb/2706690).

    As notificações de streaming do EWS nas versões do Exchange a partir do Exchange 2010 e, incluindo o Exchange Online, têm um orçamento **EWSMaxConcurrency** clonado adicional de todas as outras conexões de cliente do EWS. As conexões de notificação de streaming são contadas em um orçamento separado em relação a todas as outras operações do EWS. O orçamento máximo de simultaneidade da notificação de streaming é de fato dois orçamentos diferentes: um orçamento é para todas as contas de serviço e um orçamento é para a conta que está sendo representada. As notificações de fluxo contínuo no Exchange Online e nas versões do Exchange a partir do Exchange 2013 usam o [HangingConnectionLimit](#throttling-considerations-for-ews-notification-applications) para limitar o número de conexões.

    Por exemplo, vamos supor que **EWSMaxConcurrency** seja igual a cinco. Um usuário pode ter cinco conexões de notificação pull abertas, enquanto uma conta de serviço pode ter cinco conexões simultâneas de notificação de recebimento em relação à caixa de correio do usuário ao mesmo tempo que o usuário.

- A tabela a seguir identifica como os orçamentos de limitação do **EWSMaxSubscriptions** são calculados entre a conta de serviço e a conta para representar.

   **Tabela 2: contabilidade de orçamento EWSMaxSubscriptions**

   |**Versão do Exchange**|**Contabilidade de orçamento de limitação EWSMaxSubscriptions**|
   |:-----|:-----|
   |Exchange Online  <br/> |Cobrado da caixa de correio de destino.  <br/> |
   |Exchange 2013  <br/> |Cobrado da caixa de correio de destino.  <br/> |
   |Exchange 2010 SP3  <br/> |Cobrado da caixa de correio de destino.  <br/> |
   |Exchange 2010 SP3  <br/> |Cobrado da conta de chamada. A partir do Exchange 2010 SP2 RU4, o orçamento é cobrado em relação à caixa de correio de destino.  <br/> |
   |Exchange 2010 SP1  <br/> |Cobrado da conta de chamada.  <br/> |
   |Exchange 2010  <br/> |Cobrado da conta de chamada.  <br/> |

- Como o orçamento de limitação **EWSMaxSubscriptions** é cobrado em relação à conta que está sendo representada, não há limite no número de caixas de correio em que uma conta de serviço pode assinar e receber notificações de streaming, desde que a representação esteja sendo usada. Para que a conta seja representada, não é possível ter mais de _n_ solicitações simultâneas por caixa de correio de destino, onde _n_ é o valor de **EWSMaxSubscriptions** . Se você não estivesse usando representação, a mesma conta de serviço não pôde ter mais de _n_ total de solicitações simultâneas. Portanto, a vantagem é que, usando a representação em uma conta de serviço, você aumenta exponencialmente o número de caixas de correio que você pode atender. Para obter mais informações, consulte [manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md).

- Os parâmetros de política **EWSPercentTimeInMailboxRPC**, **EWSPercentTimeInCAS**e **EWSPercentTimeInAD** se referem a ações executadas por um único thread. Quando um aplicativo executa várias operações simultâneas, você deve considerar o efeito cumulativo dessas operações no orçamento de recursos do usuário.

## <a name="throttling-implications-for-ews-batch-requests"></a>Limitações de limitação para solicitações de lote do EWS

O EWS permite que você execute várias solicitações de item em lote em uma única solicitação executada pelo servidor de acesso para cliente. Isso permite maior eficiência e desempenho. Quando um servidor Exchange executa uma solicitação em lote, ele verifica o orçamento do usuário após a execução de cada item dentro do lote. Se o aplicativo estiver acima do orçamento, o processamento do próximo item no lote será adiado até que o orçamento desse usuário seja recarregado. Para garantir que os aplicativos que usam operações em lotes sejam executados com êxito, limite o número de solicitações de item que podem ser incluídas em um único lote e divida grandes lotes em vários lotes menores para aumentar a confiabilidade dos resultados. O efeito que uma operação em lote tem em determinados limites de limitação depende do tipo da solicitação, o tamanho dos itens a serem processados (por exemplo, em operações do **UploadItems** ou do **ExportItems** ) e o conteúdo da caixa de correio. As políticas de limitação afetam as operações em lote fazendo com que a solicitação seja mais longa para ser processada. Portanto, o chamador terá que aguardar mais tempo para a resposta e, como o EWS limita o tempo de execução de uma solicitação em lote a um minuto, a chamada pode expirar.

Para determinar o tamanho do lote ideal para um aplicativo, execute o teste de unidade usando vários conjuntos de entrada para garantir que o aplicativo não encontre nenhum erro em um ambiente de produção.

## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>Limitação de parâmetros de política que afetam as operações de pesquisa do EWS

[As operações de pesquisa no EWS](search-and-ews-in-exchange.md) podem exigir grandes quantidades de tempo e recursos, dependendo de como a pesquisa é executada e quais informações são solicitadas. Para controlar o uso de recursos durante as pesquisas, dois parâmetros de política têm efeito: **EWSFastSearchTimeoutInSeconds** e **EWSFindCountLimit**.

O parâmetro de política **EWSFastSearchTimeoutInSeconds** especifica a quantidade de tempo, em segundos, que pesquisas rápidas do EWS (também conhecidas como pesquisa de indexação de conteúdo) são executadas antes do tempo limite. Uma pesquisa rápida é uma pesquisa feita usando uma cadeia de caracteres de consulta de sintaxe de consulta avançada (AQS) em uma [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).

Você pode pesquisar uma pasta de caixa de correio do Exchange de duas maneiras:

- Usando uma pesquisa do repositório do Exchange, que realiza uma verificação seqüencial de todas as mensagens no escopo de pesquisa de destino.

- Usando o serviço de pesquisa do Exchange (indexação de conteúdo).

Esses dois tipos de pesquisas podem resultar em tempos limite. Quando possível, use o serviço de pesquisa do Exchange, pois essas pesquisas costumam ser direcionadas a índices de caixa de correio e usar consultas do AQS. O exemplo a seguir mostra como realizar uma pesquisa do AQS da caixa de entrada usando o EWS e o serviço de pesquisa do Exchange.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

Se você não pode usar uma pesquisa do AQS, evite usar filtros de pesquisa muito complexos. Além disso, tente evitar a criação de filtros de pesquisa com base em valores calculados se a consulta envolver propriedades estendidas MAPI. A pesquisa do AQS foi introduzida no Exchange 2010.

> [!NOTE]
> Na primeira vez que você executa uma consulta complexa de pesquisa do repositório do Exchange, ela é executada muito lentamente e pode expirar. Depois, a consulta responderá mais rapidamente. Para obter mais informações sobre os processos de back-end do Exchange Server que ocorrem durante consultas de pesquisa do Exchange Store, consulte [Understanding the performance Impact of High item views and Restricted views](https://technet.microsoft.com/library/cc535025%28EXCHG.80%29.aspx) in technet. O uso de um **SearchFilter** cria uma restrição dinâmica que ajuda consultas similares no futuro, mas como essas restrições são dinâmicas por natureza, elas não são permanentes ou confiáveis e são excluídas após um máximo de três dias.

O parâmetro de política **EWSFindCountLimit** especifica o número máximo de itens dos resultados de uma operação **FindItem** ou **FindFolder** que pode existir na memória em um servidor de acesso para cliente ao mesmo tempo para um usuário. Todos os itens ou pastas que o EWS processa em uma solicitação **FindItem** ou **FindFolder** são contados em relação ao orçamento especificado no elemento **EWSFindCountLimit** . Quando a resposta é enviada de volta para o solicitante, o encargo da contagem localizar para a chamada atual é liberado. A resposta que o servidor retorna a um solicitante quando o orçamento é excedido é baseada no valor do elemento **RequestServerVersion** e se o solicitante especificou a paginação. Quando o valor do elemento **RequestServerVersion** indica o Exchange 2010 ou uma versão anterior do Exchange, o servidor envia uma resposta de falha com o código de erro **ErrorServerBusy**. Se o valor do elemento **RequestServerVersion** indicar uma versão do Exchange a partir do Exchange 2010 SP1 ou Exchange Online e o cliente estiver usando a paginação, o EWS poderá retornar um conjunto de resultados parcial em vez de um erro. O aplicativo deve esperar que o EWS pode não retornar todos os itens. Se o valor do elemento **IncludesLastItemInRange** for false, o aplicativo deve fazer outra solicitação **FindItem** ou **FindFolder** com o novo deslocamento e continuar até que o elemento **IncludesLastItemInRange** retorna true.

Quando você usa uma operação **FindItem** ou **FindFolder** , é importante usar paginação. A API gerenciada do EWS impõe o uso da paginação, mas, se você estiver usando outros métodos, como objetos proxy do EWS ou SOAP bruto, será necessário definir a paginação explicitamente. O exemplo a seguir mostra como usar paginação na API gerenciada do EWS.

```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> A política padrão no Exchange limita o tamanho da página a 1000 itens. Configurar o tamanho da página para um valor maior do que esse número não tem efeito prático.

Os aplicativos também devem considerar o fato de que o valor do parâmetro throttling _EWSFindCountLimit_ pode resultar em um conjunto de resultados parcial sendo retornado para aplicativos que fazem solicitações simultâneas. O exemplo a seguir mostra como usar a propriedade **MoreAvailable** na API gerenciada do EWS para garantir que todos os resultados sejam incluídos em uma consulta.

```cs
ItemView iv = new ItemView(1000);
service.TraceEnabled = false;
FindItemsResults<Item> fiResults = null;
Do
{
    fiResults = service.FindItems(WellKnownFolderName.Inbox, iv);
    PropertySet itItemPropSet = new PropertySet(BasePropertySet.IdOnly) { EmailMessageSchema.Body };
    //Process Items in Result Set
    iv.Offset += fiResults.Items.Count;
}
while (fiResults.MoreAvailable == true);
```

## <a name="throttling-policies-and-concurrency"></a>Políticas de limitação e simultaneidade

A simultaneidade se refere ao número de conexões de um usuário específico. Uma conexão é mantida do momento em que uma solicitação é recebida até que uma resposta seja enviada ao solicitante. Se os usuários tentarem fazer mais solicitações concorrentes que o permitido por suas diretivas, o nova tentativa de conexão falhará. Entretanto, as condições existentes continuam válidas. As políticas de limitação podem afetar a simultaneidade de várias maneiras diferentes.

O parâmetro de política de limitação do **EWSMaxConcurrency** define o número de conexões simultâneas que um usuário específico pode ter em relação a um servidor do Exchange de uma só vez. Para determinar o número máximo de conexões simultâneas a serem permitidas, considere as conexões que os clientes do Outlook usarão. Outlook 2007 e Outlook 2010 use EWS para acessar a disponibilidade e informações de ausência temporária (OOF). O Mac Outlook 2011 usa EWS para todas as funcionalidades de acesso para cliente. Dependendo do número de clientes do Outlook que estão se conectando ativamente à caixa de correio de um usuário, o número de conexões simultâneas disponíveis para um usuário pode ser limitado. Além disso, se o aplicativo tiver que se conectar a várias caixas de correio simultaneamente ao usar um único contexto de segurança, é importante levar o valor da política **EWSMaxConcurrency** para a conta. Para obter mais informações sobre como usar um único contexto de segurança com conexões simultâneas, consulte [throttling considerações para aplicativos que usam a representação EWS](#throttling-considerations-for-applications-that-use-ews-impersonation) anteriormente neste artigo.

Os aplicativos que se conectam simultaneamente a várias caixas de correio devem ser capazes de controlar o uso de recursos no lado do cliente. Como as operações do EWS são baseadas em solicitação/resposta, você pode garantir que seus aplicativos funcionem bem no limite do **EWSMaxConcurrency** rastreando o número de conexões que ocorrem entre o início de uma solicitação e quando a resposta é recebida e garante que não haja mais de dez solicitações abertas ao mesmo tempo.

O parâmetro de política **EWSFindCountLimit** especifica o tamanho máximo do resultado que uma operação **FindItem** ou **FindFolder** pode usar em um servidor de acesso para cliente ao mesmo tempo para um usuário. Se um aplicativo (ou potencialmente vários aplicativos) fizer duas solicitações simultâneas do EWS **FindItem** que retornem 100 itens cada para um usuário específico, o encargo **EWSFindCountLimit** em relação ao orçamento do usuário específico será 200. Quando a primeira solicitação retorna, o orçamento cai para 100 e, quando a segunda solicitação retorna, o orçamento cai para zero. Se o mesmo aplicativo for fazer duas solicitações simultâneas para 1000 itens, o valor de orçamento será 2000 itens, o que excede o valor **EWSFindCountLimit** . Se o orçamento do usuário para itens cair abaixo de zero, a próxima solicitação resultará em um erro até que o orçamento do usuário seja recarregado para um ou mais.

## <a name="throttling-considerations-for-ews-notification-applications"></a>Considerações de limitação para aplicativos de notificação do EWS

Se você estiver criando aplicativos de notificação do EWS que fazem uso de notificações de envio, recepção ou streaming, considere as implicações das políticas de limitação do **EWSMaxSubscriptions** e do **EWSMaxConcurrency** e o **HangingConnectionLimit**.

O parâmetro de política **EWSMaxSubscriptions** especifica o número máximo de assinaturas ativas de envio, recepção e streaming que um usuário pode ter em um servidor de acesso para cliente específico ao mesmo tempo. Versões diferentes do Exchange têm valores padrão diferentes para esse parâmetro. Um usuário pode inscrever-se em todas as pastas em uma caixa de correio usando a propriedade **SubscribeToAllFolders** , que usa uma única assinatura no orçamento **EWSMaxSubscriptions** . Os usuários podem se inscrever em pastas individuais, com cada assinatura de pasta contando com o orçamento **EWSMaxSubscriptions** , até o limite definido pelo valor do parâmetro **EWSMaxSubscriptions** (por exemplo, os usuários podem assinar 20 pastas de calendário em caixas de correio diferentes se **EWSMaxSubscriptions** estiver definido como 20).

Para obter informações sobre representação e o parâmetro **EWSMaxSubscriptions** , consulte [throttling considerações para aplicativos que usam a representação EWS](#throttling-considerations-for-applications-that-use-ews-impersonation) anteriormente neste artigo.

O parâmetro de política **EWSMaxConcurrency** também pode ser um problema para notificações do EWS; por exemplo:

- Quando o EWS incrementa a contagem de conexão do proprietário da assinatura enquanto a notificação é gerada por uma assinatura push.

- Quando um aplicativo é projetado para ouvir as caixas de correio de vários usuários, e os usuários recebem notificações simultâneas para uma instância de uma mensagem enviada a uma lista de distribuição.

Se o aplicativo de notificação for multi-threaded e fizer solicitações de conexão simultâneas para obter mais informações sobre uma mensagem específica que foi recebida por uma conta de usuário, o limite de políticas do **EWSMaxConcurrency** pode ser excedido. Para fazer isso, considere monitorar as conexões simultâneas em seu aplicativo, incluindo aquelas que podem ser usadas pelo servidor e implementar o enfileiramento de solicitações no cliente.

O **HangingConnectionLimit** só é aplicável a notificações por streaming. Esse limite é definido no arquivo Web. config, o que significa que um administrador do Exchange pode definir esse valor em um servidor local do Exchange, mas as caixas de correio do Exchange Online devem usar o valor padrão para esse limite, que é 3 para o Exchange Online e o Exchange 2013. Para saber mais, confira [que valores de limitação Eu preciso levar em consideração?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).

## <a name="throttling-policy-and-application-performance"></a>Limitação da política e do desempenho do aplicativo

Os três parâmetros a seguir da política de limitação **PercentTimeIn** afetam a quantidade de tempo que um aplicativo EWS pode consumir em um servidor de acesso para cliente:

- **EWSPercentTimeInAD**

- **EWSPercentTimeInCAS**

- **EWSPercentTimeInMailboxRPC**

Os valores especificados nos parâmetros da política **PercentTimeIn** indicam a quantidade de tempo que um thread que está fazendo uma solicitação está alocada. Por exemplo, supondo que um valor de **EWSPercentTimeInCAS** de 90, se um processo fizer duas solicitações simultâneas que gastem 54 segundos cada código em execução no servidor de acesso para cliente, o processo usará 108 segundos em uma segunda janela 60. Isso representa um valor de parâmetro **EWSPercentTimeInCAS** de 180%.

> [!NOTE]
> O valor do parâmetro **EWSPercentTimeInCAS** é um superconjunto sobreposto dos valores de parâmetro **EWSPercentTimeInAD** e **EWSPercentTimeInMailboxRPC** . Isso significa que as despesas no tempo de processamento do servidor de acesso para cliente sempre serão maiores que as despesas em **EWSPercentTimeInAD** e **EWSPercentTimeInMailboxRPC**. Isso ocorre porque para o componente do Exchange fazer uma chamada RPC ou Active Directory, ele deve já estar executando o código do servidor de acesso para cliente. Além disso, as despesas em tempo de processamento para o **EWSPercentTimeInCAS** não são interrompidas enquanto as chamadas LDAP ou RPC estão sendo feitas. Embora a solicitação possa estar esperando por uma resposta dos serviços de domínio do Active Directory (AD DS) ou do repositório do Exchange, o processo ainda está consumindo um thread no servidor e, portanto, o thread deve continuar a ser cobrado por esse uso.

A quantidade de tempo de CPU que um aplicativo pode levar em um período de 60 segundos pode exceder esses limites de limitação; Portanto, é importante considerar o volume e o tipo de solicitações que estão sendo feitas. Por exemplo, um grande lote de operações **ResolveNames** que são feitas simultaneamente pode exceder o valor do parâmetro de política **EWSPercentTimeInAD** . Os valores de política que estão contidos na política de limitação padrão foram projetados para permitir que a maioria dos aplicativos do EWS funcione sem problemas; no entanto, quando aplicativos multivolume de vários threads colocam um grande volume de solicitações em um determinado servidor de acesso para cliente, isso pode criar problemas. Para evitar isso, considere limitar o tamanho dos lotes que serão executados no servidor.

## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>Limitação de políticas e aplicativos que enviam um grande volume de email

As políticas de limitação padrão incluem três parâmetros de política de limite de taxa que podem afetar os aplicativos que usam o EWS para enviar um grande volume de mensagens ou enviar mensagens em lotes grandes em um curto período de tempo.

> [!NOTE]
> Em geral, recomendamos que você não use EWS para enviar email em massa. Use um host SMTP que é especializado em serviços de email em massa para enviar mensagens de email em massa muito frequentes.

O parâmetro de política **MessageRateLimit** especifica o número de mensagens por minuto que podem ser enviadas por qualquer cliente do Exchange, incluindo o EWS. Por padrão, essa política é definida como 30 mensagens por minuto. Para usuários comuns, isso geralmente é suficiente. No entanto, aplicativos que enviam grandes lotes de mensagens de email, por exemplo, como parte de um programa de faturamento, podem ter problemas. Quando esse limite de política é excedido, a entrega de mensagens para a caixa de correio é atrasada. Especificamente, as mensagens aparecerão na pasta de saída ou rascunhos por períodos de tempo maiores, quando um usuário ou aplicativo enviar um número maior de mensagens do que o valor especificado pelo parâmetro **MessageRateLimit** . Considere isso quando você estiver desenvolvendo um sistema de controle de entrega, especialmente se o aplicativo usar uma caixa de correio que os usuários se conectam via Outlook. Quando itens adiados são armazenados na pasta de saída ou rascunhos, os usuários podem interpretar isso como um erro.

O parâmetro de política **RecipientRateLimit** especifica o limite no número de destinatários que um usuário pode endereçar em um período de 24 horas. Por exemplo, se esse valor for definido como 500, significa que uma única conta de caixa de correio do Exchange pode enviar mensagens para até 500 destinatários por dia. Esse limite se aplica às mensagens para destinatários dentro e fora da organização. Esse limite padrão pode causar problemas para alguns aplicativos de linha de negócios que fazem execuções de faturas de fim de mês e precisam enviar mensagens para mais do que esse número de destinatários. Você pode usar os serviços externos que permitem o processamento em lotes de mensagens ou soluções de retransmissão de saída locais separadas para contornar essa limitação.

O parâmetro de política **ForwardeeLimit** especifica o número máximo de destinatários para os quais as mensagens podem ser encaminhadas ou redirecionadas por meio de regras de caixa de entrada. Esse parâmetro não limita o número de mensagens que podem ser encaminhadas ou redirecionadas para os destinatários.

## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>Erros gerados quando os limites de limitação são excedidos

Quando as políticas de limitação são excedidos, o EWS gera um dos erros listados na tabela a seguir.

**Tabela 3: erros de limite de limitação**

|**Error**|**Parâmetro de política de limitação**|**Descrição**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |Indica que há mais solicitações simultâneas no servidor do que as permitidas pela política de um usuário.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |Indica que a contagem máxima de assinaturas da política de limitação do usuário foi excedida.  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |Indica que uma chamada de operação de pesquisa excedeu o número total de itens que podem ser retornados.  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC**         **EWSPercentTimeInCAS**         **EWSPercentTimeInAD** <br/> |Ocorre quando o servidor está ocupado. O valor BackOffMilliseconds retornado com erros ErrorServerBusy indica ao cliente o período de tempo que deve aguardar até que ele deva reenviar a solicitação que causou a resposta que retornou esse código de erro.  <br/> |

A tabela a seguir lista os códigos de status HTTP retornados por erros de limitação.

**Tabela 4: códigos de status HTTP retornados por erros de limitação**

|**Código de status de HTTP**|**Descrição**|
|:-----|:-----|
|HTTP 503  <br/> |Indica que as solicitações EWS estão sendo enfileiradas com o IIS. O cliente deve atrasar o envio de solicitações adicionais até um momento posterior.  <br/> |
|HTTP 500  <br/> |Indica um erro interno do servidor com o código de erro ErrorServerBusy. Isso indica que o cliente deve atrasar o envio de solicitações adicionais até um momento posterior. A resposta pode conter uma dica de retorno chamada BackOffMilliseconds. Se presente, o valor de BackOffMilliseconds deve ser usado como a duração até que o cliente reenvie uma solicitação.  <br/> |
|HTTP 200  <br/> |Contém uma resposta de erro baseada em esquema do EWS com um código de erro do ErrorInternalServerError. Um código de erro ErrorServerBusy interno pode estar presente. Isso indica que o cliente deve atrasar o envio de solicitações adicionais até um momento posterior.  <br/> |

## <a name="see-also"></a>Confira também

- [Gerenciamento de carga de trabalho do Exchange](https://technet.microsoft.com/library/jj150503.aspx)
- [Cmdlet New-ThrottlingPolicy](https://technet.microsoft.com/library/dd351045.aspx)
- [Noções básicas sobre políticas de limitação de cliente](https://technet.microsoft.com/library/dd297964.aspx)
- [Classe ThrottlingPolicy](https://msdn.microsoft.com/library/ff342496%28v=EXCHG.140%29.aspx)
- [Políticas de limitação e o EWSFindCountLimit](https://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [Instantâneos de orçamento nos logs do IIS](https://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)

- [Efeitos da limitação em sua implantação no Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Limitação de associações de política no Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [Políticas de limitação e CPUStartPercent](https://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
