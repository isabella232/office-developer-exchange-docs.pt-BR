---
title: EWS limitação no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b4fff4c9-c625-4d2a-9d14-bb28a5da5baf
description: Saiba mais sobre as políticas de limitação que afetam o EWS quando você estiver usando o Exchange.
ms.openlocfilehash: e7966f67753b3998235e000a022e41c90fa227b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750713"
---
# <a name="ews-throttling-in-exchange"></a>EWS limitação no Exchange

Saiba mais sobre as políticas de limitação que afetam o EWS quando você estiver usando o Exchange.
  
**Fornecido por:** Dimensiona Glen; Michael Mainer, Microsoft Corporation 
  
O artigo fornece informações sobre limitação no Exchange Online, Exchange Online como parte do Office 365, do EWS e versões do Exchange, começando com o Exchange 2010 no local. Limitação no Exchange ajuda a garantir a confiabilidade de servidor e o tempo de atividade, limitando a quantidade de recursos do servidor que um único usuário ou aplicativo pode consumir. Limitação é uma resposta reativa ao uso excessivo dos recursos do sistema que possam afetar a funcionalidade e confiabilidade de serviço. Exchange constantemente monitora a integridade dos recursos de infraestrutura crítico, como bancos de dados de caixa de correio. Quando os fatores de carga alta são detectados que prejudicar o desempenho desses recursos, as conexões do EWS serão restritas proporcionalmente com base na quantidade que cada chamador tiver contribuíram para essa condição de carga alta. O resultado é que um usuário pode estar dentro do seu limite de limitação e ainda enfrentar gargalos até que seja de integridade do recurso de volta aos níveis de operacionais.
  
Cada protocolo de acesso do cliente no Exchange, incluindo o EWS, tem uma política de limitação. Ao criar aplicativos que usam o EWS, é importante levar em conta as políticas de limitação, para ajudar a garantir a confiabilidade do aplicativo e a integridade do seu servidor Exchange. Este artigo identifica os limites de serviço e de diferentes políticas de limitação para o EWS, se você está direcionando o Exchange Online ou versões do Exchange começando com o Exchange Server 2010 ao local. Conforme aplicável, este artigo também identifica as diferenças nas políticas em versões diferentes do Exchange de limitação.
  
> [!IMPORTANT]
> Padrão de diretiva de limitação, acesso a política de limitação e configuração de diretiva de limitação difere entre o Exchange Online e do Exchange local. Valores de configuração de limitação específicos somente são precisos para uma versão específica do Exchange. Como os valores de configuração variam entre versões, e os administradores do Exchange podem alterar o padrão de limitação de políticas para implantações em instalações, este artigo não fornece o padrão valores de configuração. É mais importante para que você esteja ciente das considerações para projetar um aplicativo que funciona dentro de limites de limitação e reage apropriadamente para cenários de limitação. 
  
Se você for um desenvolvedor de aplicativos, você precisará fator limitação em seu design de aplicativo. Versões diferentes do Exchange têm valores padrão diferente para os parâmetros de limitação EWS. Aplicativos cliente e o serviço projetadas para acessar as versões diferentes do Exchange precisarão de levar em conta para essas configurações, quer estejam valores padrão, os valores personalizados definidos por um administrador do Exchange, ou, como Exchange Online, definidos por padrão e não detectáveis. Porque os valores de parâmetro de limitação não pode ser descoberto programaticamente, suas especificações de design do cliente devem incluir um plano para o aplicativo para se adaptar potencial diferente limites de limitação. Ao criar aplicativos multithread que irão acessar um grande número de caixas de correio ou quando muitos clientes estão acessando a mesma caixa de correio, considere os limites de simultaneidade que a política padrão se aplica ao Exchange. 
  
## <a name="throttling-policies-that-affect-ews"></a>Políticas de limitação que afetam o EWS
<a name="bk_PolicyParameters"> </a>

A limitação de políticas em afetam do Exchange não apenas EWS, mas também todas as conexões de cliente para o servidor do Exchange, incluindo os protocolos usados pelo Office Outlook, Outlook Web App e Exchange ActiveSync. 
  
**CPUStartPercent** política de limitação pode afetar o desempenho de EWS quando você estiver executando o Exchange 2010. Quando a utilização média de CPU do Exchange processa executado no servidor de acesso para cliente — incluindo, mas não limitado, o processo EWS — excede o valor especificado por essa diretiva, as solicitações de entrada serão atrasadas para reduzir a utilização da CPU. Você não pode alterar o valor dessa diretiva, mas saber sobre ele pode ajudá-lo a solucionar problemas de desempenho. A lógica de amostragem, que o servidor de acesso para cliente executa para esse valor é uma média sobre um segundo 10 aplicação da janela. Isso permite que o processo responder apropriadamente a rápida picos de utilização da CPU. Quando esse limite for excedido, conexões de entrada para o EWS atraso. Esse atraso está limitado a 500 milissegundos (MS) em um uso de CPU de 100% teórico por solicitação do EWS. Se uma solicitação EWS em lote para obter 100 itens é passada, o servidor verificará o uso da CPU 100 vezes (uma vez por item) para um atraso máximo de 50 segundos. O tempo de atraso é linearmente proporcional ao uso da CPU. Em **CPUStartPercent**, o atraso é 0 (um rendimento thread) e aumenta linearmente até 500 ms no uso de CPU de 100%. Como políticas de limitação se aplicam a todos os usuários do Exchange, é improvável que o uso da CPU excede o limite de **CPUStartPercent** em um servidor de acesso para cliente do Exchange, porque a usuários individuais ou aplicativos não podem obter o suficiente para afetar de utilização da CPU operação do servidor. 
  
A tabela a seguir lista os parâmetros de política de limitação que afetam os aplicativos que usam o EWS.
  
**Tabela 1: Limitação parâmetros de política que afetam o EWS**

|**Nome do parâmetro de política de limitação**|**Aplica-se a**|**Descrição**|
|:-----|:-----|:-----|
|**DiscoveryMaxConcurrency** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de conexões de pesquisa de descoberta simultâneas que um usuário pode ter ao mesmo tempo.  <br/> |
|**DiscoveryMaxKeywords** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de palavras-chave que um usuário pode incluir em uma pesquisa de descoberta.  <br/> |
|**DiscoveryMaxKeywordsPerPage** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de palavras-chave para as quais exibir estatísticas.  <br/> |
|**DiscoveryMaxMailboxes** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de caixas de correio de origem que um usuário pode incluir em uma pesquisa de descoberta.  <br/> |
|**DiscoveryMaxMailboxesResultsOnly** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número máximo de caixas de correio que você pode pesquisar em uma pesquisa eDiscovery no pesquisa sem poder exibir as estatísticas.  <br/> |
|**DiscoveryPreviewSearchResultsPageSize** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Especifica o número de mensagens retornadas em uma resposta de visualização de pesquisa de descoberta eletrônica.  <br/> |
|**EwsCutoffBalance** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define os limites de consumo de recursos para o usuário do EWS antes que o usuário seja bloqueado totalmente para executar operações em um componente específico.  <br/> |
|**EwsMaxBurst** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define a quantidade de tempo que um usuário do EWS pode consumir uma quantidade elevada de recursos antes que está sendo limitadas. Isso é medido em milissegundos. Esse valor é definido separadamente para cada componente.  <br/> |
|**EwsRechargeRate** <br/> |Exchange 2013  <br/> Exchange Online  <br/> |Define a taxa na qual o orçamento de usuário do EWS é recarregado (orçamento aumenta por) durante o tempo do orçamento.  <br/> |
|**EWSMaxSubscriptions** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número máximo de push ativo, recepção e streaming inscrições de notificação de que um usuário pode ter ao mesmo tempo em um servidor de acesso para cliente específico. Isso é orçado forma diferente para diferentes versões do Exchange.  <br/> |
|**EWSFastSearchTimeoutInSeconds** <br/> |Exchange 2010  <br/> |Define a quantidade de tempo em segundos, que fast pesquisas feitas por meio de pesquisa do Exchange no EWS continuam antes que eles expirarem. Buscas Fast são feitas por meio de uma cadeia de caracteres de consulta de sintaxe de consulta avançada (AQS) em uma [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).  <br/> |
|**EWSFindCountLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número máximo de itens de uma [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) ou [FindFolder operação](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) que podem existir na memória do servidor de acesso para cliente para um usuário de uma só vez. O valor padrão para essa propriedade é 1000. O [valor de fallback](http://technet.microsoft.com/en-us/library/dd297964%28v=exchg.141%29.aspx#fallback)para esse valor é 1.000.  <br/> No Exchange Online e versões de local do Exchange, começando com o Exchange 2013, essa política de limitação não pode ser consultada ou configurada por um cmdlet. Nas versões do Exchange Online e no local do Exchange, começando com o Exchange 2013, o EWSFindCountLimit para [pesquisa AQS](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md) e qualquer Exchange pesquisa com uma restrição é 250 resultados. Uma pesquisa do Exchange sem uma restrição retornará até 1000 resultados.  <br/> |
|**EWSPercentTimeInAD** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante o qual um usuário específico pode executar solicitações do Active Directory.  <br/> |
|**EWSPercentTimeInCAS** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante o qual um usuário específico pode executar o código de servidor de acesso para cliente.  <br/> |
|**EWSPercentTimeInMailboxRPC** <br/> |Exchange 2010  <br/> |Define a porcentagem de tempo por minuto durante o qual um usuário específico pode executar solicitações RPC de caixa de correio  <br/> |
|**EWSMaxConcurrency** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número de conexões abertas simultâneas que um usuário específico pode ter em relação a um servidor do Exchange que está usando o EWS ao mesmo tempo. O valor padrão para o Exchange 2010 é 10. O valor padrão para o Exchange 2013 e Exchange Online é 27.  <br/> Essa política se aplica a todas as operações, exceto as notificações de fluxo contínuo. Notificações de streaming usam o **HangingConnectionLimit** para indicar o número de conexões abertas do streaming evento que estão disponíveis. Para obter mais informações, consulte [quais valores limitação eu preciso levar em consideração?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).  <br/> |
|**MessageRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o número de mensagens por minuto que possa ser enviado.  <br/> |
|**RecipientRateLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o limite ao número de destinatários que um usuário pode endereçar em um período de 24 horas.  <br/> |
|**ForwardeeLimit** <br/> |Exchange 2010  <br/> Exchange 2013  <br/> Exchange Online  <br/> |Define o limite para o número de destinatários para ações de encaminhamento/redirecionamento da caixa de entrada em um período de 24 horas.  <br/> |
   
> [!CAUTION]
> Não definir políticas de limitação para **Nulo**. Isso definirá a política como igual ilimitado, que indica que uma política de limitação não estiver definida. 
  
## <a name="displaying-the-policies-that-apply-to-exchange-mailboxes"></a>Exibindo as políticas que se aplicam às caixas de correio do Exchange
<a name="bk_PolicyCmdlets"> </a>

Exchange local fornece cmdlets do Shell de gerenciamento do Exchange que você pode usar para definir e obter a política de limitação. O Exchange Online não fornece acesso aos cmdlets de política de limitação.
  
Você pode usar os seguintes cmdlets para exibir a limitação de políticas para uma implantação do Exchange Server local:
  
- **Get-ThrottlingPolicy** — obtém o cliente limitação configurações para uma ou mais políticas de limitação. Para obter mais informações, consulte [Get-ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351264.aspx) no TechNet. 
    
- **Get-ThrottlingPolicyAssociation** — permite que você exiba o relacionamento entre um objeto e suas políticas de limitação associadas. O objeto pode ser um usuário com uma caixa de correio, um usuário sem uma caixa de correio ou um contato. Para obter mais informações, consulte [Get-ThrottlingPolicyAssociation](http://technet.microsoft.com/en-us/library/ff459241.aspx) no TechNet. 
    
Use o seguinte comando para mostrar a diretiva padrão de limitação para o Exchange 2010.
  
**Get-ThrottlingPolicy | Where-Object {$_. IsDefault - eq "True"} | format-list**
  
Use o seguinte comando para mostrar a diretiva de limitação global (que corresponde à diretiva padrão de limitação no Exchange 2010) no Exchange 2013.
  
**Get-ThrottlingPolicy | Where-Object {$_. ThrottlingPolicyScope - eq "Global"} | format-list**
  
Use o seguinte comando para mostrar a limitação política associada a um usuário no Exchange 2010 ou Exchange 2013. Substitua o nome de usuário john@contoso.com com o nome de usuário do usuário de destino para o qual você deseja obter informações sobre a diretiva de limitação.
  
**Get-ThrottlingPolicyAssociation john@contoso.com | format-list**
  
Executar este comando no Exchange Management Shell resulta em uma saída semelhante à seguinte.
  
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
> Quando a propriedade **ThrottlingPolicyId** estiver em branco, a política padrão é aplicada à caixa de correio. 
  
Você pode definir a limitação de diretiva em um servidor do Exchange usando os cmdlets [Set-ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd298094.aspx) e [Set-ThrottlingPolicyAssociation](http://technet.microsoft.com/en-us/library/ff459231.aspx) . Você pode criar e remover políticas de limitação usando os cmdlets [New-ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351045.aspx) e [Remove-ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351178.aspx) de não-padrão. 
  
> [!TIP]
> Recomendamos que você crie seus aplicativos para cumpram a diretiva padrão de limitação. Só faça alterações como padrão as políticas de limitação se o projeto do seu aplicativo de cliente não puder acomodar a política padrão. Lembre-se de que as políticas de limitação menos restritivas podem afetar negativamente confiabilidade de serviço. 
  
## <a name="throttling-considerations-for-applications-that-use-ews-impersonation"></a>Considerações de limitação para aplicativos que utilizam a representação do EWS
<a name="bk_ThrottlingConsiderations"> </a>

[Representação](impersonation-and-ews-in-exchange.md) é um método de autorização que permite uma única conta acessar as contas de muitos. Quando uma conta de serviço personifica usuários, ele atua como os usuários e, portanto, pressupõe os direitos que são atribuídos aos usuários. Arquivos de log registram o acesso como usuário representado. Os administradores usar o controle de acesso baseado em função (RBAC) para configurar a representação por meio do Shell de gerenciamento do Exchange. 
  
Quando representação é usada, os orçamentos para todos os limites de limitação aplicam formas diferentes dependendo da versão do Exchange. O orçamento é calculado ou contra a conta que é representada, ou a conta de serviço. Se seu aplicativo é multithreaded e torna solicitações simultâneas em relação a várias caixas de correio, você deve considerar como o limite da limitação afetará o desempenho do seu aplicativo. Em geral, esteja ciente dos seguintes limites em contas de serviço quando você cria um aplicativo baseado no serviço que usa a representação para acessar todas as caixas de correio: 
  
- Quando você usa a representação, a conta de serviço tem um orçamento separado para os seguintes parâmetros de política:
    
  - **EWSMaxConcurrency**
    
  - **EWSPercentTimeInAD**
    
  - **EWSPercentTimeInCAS**
    
  - **EWSPercentTimeInMailboxRPC**
    
  - **EWSMaxSubscriptions**
    
  - **EWSFastSearchTimeoutInSeconds**
    
  - **EWSFindCountLimit**
    
- O orçamento **EWSMaxConcurrency** é compartilhado para a conta de serviço e a conta que está sendo representada para todas as conexões com versões anteriores ao Exchange 2010 Service Pack 2 (SP2) cumulativo de atualizações 4 (RU4) do Exchange. Começando com o Exchange 2010 SP2 RU4 e incluindo o Exchange Online, o acesso à conta de serviço usa um orçamento separado do orçamento **EWSMaxConcurrency** usuário. Para obter mais informações sobre a atualização para a diretiva de limitação de conexão simultâneas do Exchange para o EWS, consulte [Descrição do Update Rollup 4 para Exchange Server 2010 Service Pack 2](http://support.microsoft.com/kb/2706690).
    
    EWS streaming notificações nas versões do Exchange, começando com o Exchange 2010 e incluindo o Exchange Online, tem um orçamento de **EWSMaxConcurrency** clonado adicional de todas as outras conexões de cliente do EWS. Streaming de conexões de notificação são contados contra um orçamento separado que todas as outras operações de EWS. O orçamento de simultaneidade máximo de notificação streaming é realmente dois diferentes orçamentos: um orçamento é para todas as contas de serviço e um orçamento é para a conta sendo representada. Notificações de fluxo no Exchange Online e versões do Exchange, começando com o Exchange 2013 usam o [HangingConnectionLimit](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) para limitar o número de conexões. 
    
    Por exemplo, vamos supor que **EWSMaxConcurrency** é igual a cinco. Um usuário pode ter cinco conexões de notificação de recepção open, enquanto uma conta de serviço pode ter cinco conexões de notificação de recepção simultâneas em relação a caixa de correio do usuário ao mesmo tempo que o usuário. 
    
- A tabela a seguir identifica como orçamentos de limitação de **EWSMaxSubscriptions** são calculados entre a conta de serviço e a conta para representar. 
    
   **Tabela 2: Estatísticas de orçamento de EWSMaxSubscriptions**

   |**Versão do Exchange**|**EWSMaxSubscriptions estatísticas de orçamento de limitação**|
   |:-----|:-----|
   |Exchange Online  <br/> |Cobrado contra a caixa de correio de destino.  <br/> |
   |Exchange 2013  <br/> |Cobrado contra a caixa de correio de destino.  <br/> |
   |Exchange 2010 SP3  <br/> |Cobrado contra a caixa de correio de destino.  <br/> |
   |Exchange 2010 SP3  <br/> |Cobrado contra a conta de chamada. Iniciando com o Exchange 2010 SP2 RU4, o orçamento é cobrado contra a caixa de correio de destino.  <br/> |
   |Exchange 2010 SP1  <br/> |Cobrado contra a conta de chamada.  <br/> |
   |Exchange 2010  <br/> |Cobrado contra a conta de chamada.  <br/> |
   
- Como o **EWSMaxSubscriptions** limitação orçamento é cobrado contra a conta que está sendo representada, não há nenhum limite no número de caixas de correio de uma conta de serviço pode assinar e receber notificações de streaming, desde que seja de representação sendo usado. Para a conta que está sendo representada, você não pode ter mais de _n_ de solicitações simultâneas por caixa de correio de destino, onde _n_ é o valor de **EWSMaxSubscriptions** . Se você não estivesse usando representação, a mesma conta de serviço não poderia ter mais do que o total de solicitações simultâneas _n_ . Portanto, o argumento é que usando representação em uma conta de serviço, você exponencial aumenta o número de caixas de correio que você pode atender. Para obter mais informações, consulte [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md).
    
- Os parâmetros de política **EWSPercentTimeInMailboxRPC**, **EWSPercentTimeInCAS**e **EWSPercentTimeInAD** consultem ações executadas por um único segmento. Quando um aplicativo realiza várias operações simultâneas, você deve levar em consideração o efeito cumulativo dessas operações na cota de recursos do usuário. 
    
## <a name="throttling-implications-for-ews-batch-requests"></a>Limitação implicações para solicitações de lote EWS
<a name="bk_ThrottlingBatch"> </a>

EWS permite várias solicitações de item de lote em uma única solicitação que é executada pelo servidor de acesso para cliente. Isso permite maior eficiência e o desempenho. Quando um servidor Exchange executa uma solicitação em lote, ele verifica orçamento de usuário depois da execução de cada item no lote. Se o aplicativo estiver acima do orçamento, o processamento do próximo item no lote foi adiado até que o orçamento para que o usuário tem recarregada. Para garantir que aplicativos que usam operações em lotes é executado com êxito, limite o número de solicitações de item que pode ser incluído em um único lote e dividir grandes lotes entre vários lotes menores para aumentar a confiabilidade dos resultados. O efeito que uma operação em lote tem nos limites de limitação determinados depende do tipo da solicitação, o tamanho dos itens a serem processados (por exemplo, em operações **UploadItems** ou **ExportItems** ) e o conteúdo de caixa de correio. Políticas de limitação afetam operações em lotes, fazendo com que a solicitação para levar mais tempo para o processo. O chamador, portanto, será necessário aguardar pela resposta mais e, como EWS limita o tempo de execução de uma solicitação de lote um minuto, a chamada poderá expirar. 
  
Para determinar o tamanho de lote ideal para um aplicativo, execute a unidade teste usando que diversas entradas define para garantir que o aplicativo não encontrar erros em um ambiente de produção. 
  
## <a name="throttling-policy-parameters-that-affect-ews-search-operations"></a>Parâmetros de política de limitação que afetam o EWS operações de pesquisa
<a name="bk_ThrottlingSearch"> </a>

[Operações de pesquisa no EWS](search-and-ews-in-exchange.md) pode exigir grandes quantidades de tempo e recursos, dependendo de como a pesquisa é executada e quais informações são solicitadas. Para controlar o uso do recurso durante as pesquisas, dois parâmetros de diretiva entrem em vigor: **EWSFastSearchTimeoutInSeconds** e **EWSFindCountLimit**. 
  
O parâmetro de política **EWSFastSearchTimeoutInSeconds** Especifica a quantidade de tempo, em segundos, que pesquisas rápidas do EWS (também conhecido como conteúda pesquisa indexação) executado antes que o tempo limite é ultrapassado. Uma pesquisa rápida é uma pesquisa feita por meio de uma cadeia de caracteres de consulta de sintaxe de consulta avançada (AQS) em uma [operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
  
Você pode pesquisar uma pasta de caixa de correio do Exchange de duas maneiras:
  
- Usando uma pesquisa de repositório do Exchange, que executa um exame sequencial de todas as mensagens no escopo da pesquisa de destino.
    
- Usando o serviço de pesquisa do Exchange (indexação de conteúdo).
    
Ambos os tipos de pesquisas podem resultar em tempos limite. Quando possível, use o serviço de pesquisa do Exchange porque essas pesquisas frequentemente visadas nos índices de caixa de correio e usam AQS consultas. O exemplo a seguir mostra como executar uma pesquisa AQS da caixa de entrada usando o EWS e o serviço de pesquisa do Exchange.
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiitems = service.FindItems(WellKnownFolderName.Inbox, "subject:football", iv);
```

Se você não pode usar uma pesquisa AQS, evite usar filtros de pesquisa muito complexa. Além disso, tente evitar a criação de filtros de pesquisa com base em valores computados, se a consulta envolve as propriedades estendidas de MAPI. Pesquisa AQS foi introduzida no Exchange 2010.
  
> [!NOTE]
> Na primeira vez que você executar uma consulta de pesquisa de repositório Exchange complexa, ele é executado muito lentamente e talvez o tempo limite. Depois disso, a consulta responderá mais rapidamente. Para obter mais informações sobre o back-end Exchange processos do servidor que ocorrem durante o intercâmbio de armazenar consultas de pesquisa, consulte [Noções básicas sobre o desempenho do impacto de alta Item contagens e exibições restritas](http://technet.microsoft.com/en-us/library/cc535025%28EXCHG.80%29.aspx) no TechNet. Usar um **SearchFilter** cria uma restrição dinâmica que ajuda a consultas semelhantes no futuro, mas como essas restrições são dinâmicas de natureza temporária, eles não são permanente ou confiável e são excluídos após um máximo de três dias. 
  
O parâmetro de política de **EWSFindCountLimit** Especifica o número máximo de itens dos resultados de uma operação de **FindItem** ou **FindFolder** que podem existir na memória em um servidor de acesso para cliente ao mesmo tempo para um único usuário. Cada item ou a pasta que o EWS processa em uma solicitação **FindItem** ou **FindFolder** é contada em relação ao orçamento especificado no elemento **EWSFindCountLimit** . Quando a resposta será enviada para o solicitante, a carga de contagem de localização para a chamada atual é liberada. A resposta, que o servidor retorna para um solicitante quando o orçamento é excedido baseia-se o valor do elemento **RequestServerVersion** e se o solicitante especificado paginação. Quando o valor do elemento **RequestServerVersion** indica o Exchange 2010 ou uma versão anterior do Exchange, o servidor envia uma resposta de falha com o código de erro **ErrorServerBusy**. Se o valor do elemento **RequestServerVersion** indica uma versão do Exchange começando com o Exchange 2010 SP1 ou Exchange Online e o cliente está usando paginação, EWS pode retornar um conjunto, em vez de um erro de resultados parcial. Seu aplicativo deve esperar que o EWS não pode retornar todos os itens. Se o valor do elemento **IncludesLastItemInRange** for false, o aplicativo deve fazer outra solicitação **FindItem** ou **FindFolder** com o deslocamento de novo e continue até que o elemento **IncludesLastItemInRange** retornará true. 
  
Quando você usa uma operação **FindItem** ou **FindFolder** , é importante usar paginação. A API gerenciada de EWS impõe o uso de paginação, mas se você estiver usando outros métodos, como objetos de proxy do EWS ou bruto SOAP, você precisará definir explicitamente a paginação. O exemplo a seguir mostra como usar a paginação na API gerenciada do EWS. 
  
```cs
ItemView iv = new ItemView(1000);
FindItemsResults<Item> fiFindItemResults = service.FindItems(WellKnownFolderName.Inbox, iv);
```

> [!NOTE]
> A política padrão no Exchange limita o tamanho de página para itens de 1000. Definir o tamanho da página como um valor que for maior do que esse número tem nenhum efeito prático. 
  
Aplicativos também deve levar em consideração o fato de que o _EWSFindCountLimit_ limitação do valor do parâmetro pode resultar em um conjunto que está sendo retornada para aplicativos que fazem solicitações simultâneas de resultados parcial. O exemplo a seguir mostra como usar a propriedade **MoreAvailable** na API gerenciada do EWS para garantir que todos os resultados são incluídos em uma consulta. 
  
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
<a name="bk_ThrottlingConcurrency"> </a>

Simultaneidade refere-se ao número de conexões de um usuário específico. Uma conexão é mantido desde o momento em que uma solicitação for recebida até que uma resposta é enviada ao solicitante. Se os usuários tentarem tornar mais solicitações simultâneas que permite a sua política, a nova tentativa de conexão falha. No entanto, as conexões existentes permanecerão válidas. Políticas de limitação pode afetar simultaneidade de várias maneiras diferentes.
  
O parâmetro de política de limitação **EWSMaxConcurrency** define o número de conexões simultâneas que um usuário específico pode ter ao mesmo tempo em relação a um servidor Exchange. Para determinar o número máximo de conexões simultâneas para permitir, considere as conexões que os clientes do Outlook usará. Outlook 2007 e Outlook 2010 usam o EWS para acessar informações de disponibilidade e ausência temporária. Mac Outlook 2011 usa o EWS para todas as funcionalidades de acesso do cliente. Dependendo do número de clientes do Outlook que está se conectando ativamente a caixa de correio do usuário, o número de conexões simultâneas disponíveis para um usuário pode ser limitado. Além disso, se seu aplicativo tiver conectem a várias caixas de correio simultaneamente durante o uso de um contexto de segurança único, é importante ser o valor da política **EWSMaxConcurrency** analisadas. Para obter mais informações sobre como usar um contexto de segurança único com conexões simultâneas, consulte [Considerações de aceleração para aplicativos que utilizam a representação EWS](http://msdn.microsoft.com/library/961f773a-8b8e-4b4f-a4b9-64305e107ca4.aspx#bk_ThrottlingConsiderations) anteriormente neste artigo. 
  
Aplicativos que se conectam simultaneamente para várias caixas de correio precisam ser capaz de rastrear o uso de recursos no lado do cliente. Como operações do EWS são baseados em solicitação/resposta, você pode assegurar que seus aplicativos funcionam bem dentro do limite de **EWSMaxConcurrency** controlando o número de conexões que ocorrem entre o início de uma solicitação e a resposta é recebidos e garantir que não mais de dez abrir solicitações ocorrer simultaneamente. 
  
O parâmetro de política de **EWSFindCountLimit** Especifica o tamanho máximo de resultado que uma operação **FindItem** ou **FindFolder** pode usar em um servidor de acesso para cliente ao mesmo tempo para um usuário. Se um aplicativo (ou potencialmente vários aplicativos) faz duas solicitações simultâneas do EWS **FindItem** que retornam 100 itens, cada um para um usuário específico, a carga de **EWSFindCountLimit** contra orçamento específico do usuário será 200. Quando a primeira solicitação retorna, o orçamento cai para 100 e quando a segunda solicitação retorna, o orçamento cai para zero. Se o mesmo aplicativo fosse fazer duas solicitações simultâneas para itens de 1000, o valor do orçamento seria itens 2000, que excede o valor de **EWSFindCountLimit** . Se o orçamento do usuário para itens cair abaixo de zero, a próxima solicitação resulta em erro até que o orçamento de usuário é recarregada a uma ou mais. 
  
## <a name="throttling-considerations-for-ews-notification-applications"></a>Considerações de limitação para aplicativos de notificação de EWS
<a name="bk_ThrottlingNotifications"> </a>

Se você estiver criando notificação EWS aplicativos que usam de envio, recepção ou streaming notificações, você deve considerar as implicações do **EWSMaxSubscriptions** e as políticas de limitação de **EWSMaxConcurrency** e o ** HangingConnectionLimit**. 
  
O parâmetro de política de **EWSMaxSubscriptions** Especifica o número máximo de inscrições de streaming que um usuário pode ter em um servidor de acesso para cliente específico ao mesmo tempo, recepção e push ativo. Versões diferentes do Exchange têm valores padrão diferente para esse parâmetro. Um usuário pode inscrever-se a todas as pastas em uma caixa de correio usando a propriedade **SubscribeToAllFolders** - usa a uma única assinatura em relação ao orçamento **EWSMaxSubscriptions** . Os usuários podem assinar pastas individuais, com cada pasta rumo o orçamento **EWSMaxSubscriptions** , até o limite de contagem de assinatura definida pelo valor do parâmetro **EWSMaxSubscriptions** (por exemplo, os usuários podem se inscrever no calendário 20 pastas nas caixas de correio diferentes se **EWSMaxSubscriptions** for definido como 20). 
  
Para obter informações sobre representação e o parâmetro **EWSMaxSubscriptions** , consulte [Considerações de aceleração para aplicativos que utilizam a representação EWS](ews-throttling-in-exchange.md#bk_ThrottlingConsiderations) anteriormente neste artigo. 
  
O parâmetro de política **EWSMaxConcurrency** também pode ser um problema para notificações do EWS; Por exemplo: 
  
- Quando o EWS incrementa a contagem de conexão para o proprietário da assinatura, enquanto a notificação está sendo gerada por uma inscrição de envio.
    
- Quando um aplicativo foi projetado para escutar a caixas de correio de vários usuários e os usuários recebem notificações simultâneas para uma instância de uma mensagem que será enviada para uma lista de distribuição.
    
Se o aplicativo de notificação é multithreaded e faz solicitações simultâneas de conexão para obter mais informações sobre uma determinada mensagem foi recebida por uma conta de usuário, o limite de política **EWSMaxConcurrency** pode ser excedido. Para justificar isso, considere as conexões simultâneas em seu aplicativo de monitoramento, inclusive aquelas que poderiam ser usadas pelo servidor e implementando a solicitação de enfileiramento de mensagens no cliente. 
  
O **HangingConnectionLimit** só é aplicável a notificações de fluxo contínuo. Esse limite é definido no arquivo Web. config, que significa que um administrador do Exchange pode definir esse valor em um servidor do Exchange local, mas as caixas de correio Exchange Online devem usar o valor padrão para esse limite, que é 3 para Exchange Online e Exchange 2013. Para saber mais, consulte [quais valores limitação eu preciso levar em consideração?](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).
  
## <a name="throttling-policy-and-application-performance"></a>Limitação de desempenho de política e do aplicativo
<a name="bk_PercentTimeIn"> </a>

Os seguintes três parâmetros de **PercentTimeIn** política de limitação afetam a quantidade de tempo que um aplicativo do EWS pode consumir em um servidor de acesso para cliente: 
  
- **EWSPercentTimeInAD**
    
- **EWSPercentTimeInCAS**
    
- **EWSPercentTimeInMailboxRPC**
    
Os valores especificados nos parâmetros de política de **PercentTimeIn** indicam a quantidade de tempo que é alocado fazendo uma solicitação de um segmento. Por exemplo, supondo que um valor de **EWSPercentTimeInCAS** de 90, se um processo faz duas solicitações simultâneas que gastam 54 segundos cada código em execução no servidor de acesso para cliente, o processo usa 108 segundos em um segundo 60 janela. Isso representa um valor de parâmetro **EWSPercentTimeInCAS** de 180%. 
  
> [!NOTE]
> O valor do parâmetro **EWSPercentTimeInCAS** é um subconjunto de sobreposição dos valores de parâmetro **EWSPercentTimeInAD** e **EWSPercentTimeInMailboxRPC** . Isso significa que as despesas em tempo de processamento do servidor de acesso para cliente sempre ser maior do que as despesas em **EWSPercentTimeInAD** e **EWSPercentTimeInMailboxRPC**. Isso ocorre porque para o componente do Exchange para um Active Directory ou uma chamada de RPC, ele deve já estar executando código do servidor de acesso para cliente. Além disso, as despesas no tempo de processamento para **EWSPercentTimeInCAS** não será interrompida enquanto LDAP ou chamadas RPC são feitas. Embora a solicitação de maneira síncrona pode estar aguardando por uma resposta do serviços de domínio Active Directory (AD DS) ou o armazenamento do Exchange, o processo ainda está consumindo um segmento no servidor e, portanto, o thread deve continuar a ser cobrado por esse uso. 
  
A quantidade de tempo de CPU, que um aplicativo pode levar em um período de 60 segundos pode exceder essas redução dos limites; Portanto, é importante considerar o volume e o tipo de solicitações que estão sendo feitos. Por exemplo, um lote grande de operações de **ResolveNames** que são feitas simultaneamente pode exceder o valor do parâmetro **EWSPercentTimeInAD** política. Os valores de política que estão contidos na política de limitação padrão foram projetados para permitir a maioria dos aplicativos do EWS funcionar sem problemas; No entanto, quando os aplicativos de alto volume multithread colocar um grande volume de solicitações em um determinado servidor de acesso para cliente, isso pode criar problemas. Para evitar isso, considere a possibilidade de limitar o tamanho de lotes que irá executar com base no servidor. 
  
## <a name="throttling-policies-and-applications-that-send-a-large-volume-of-email"></a>Políticas de limitação e aplicativos que enviam um grande volume de email
<a name="bk_RateLimits"> </a>

As políticas de limitação padrão incluem três parâmetros de política de limite de taxa que podem afetar a aplicativos que usam o EWS para enviar um grande volume de mensagens ou enviar mensagens em grandes lotes em um curto período de tempo. 
  
> [!NOTE]
> Em geral, é recomendável que você não usar o EWS para enviar emails em massa. Use um host de SMTP especializada em serviços de email em massa para enviar mensagens de email em massa de grandes frequentes. 
  
O parâmetro de política de **MessageRateLimit** Especifica o número de mensagens por minuto que possa ser enviado por qualquer cliente do Exchange, incluindo o EWS. Por padrão, essa diretiva estiver definida como 30 mensagens por minuto. Para usuários comuns, isso é geralmente suficiente. No entanto, aplicativos que enviam grandes lotes das mensagens de email, por exemplo, como parte de um programa de faturamento, poderá ter problemas. Quando esse limite de política for excedido, a entrega de mensagens da caixa de correio foi adiada. Especificamente, as mensagens serão exibidas na pasta Rascunhos ou de caixa de saída por longos períodos de tempo quando um usuário ou aplicativo envia um número maior de mensagens que o valor especificado pelo parâmetro **MessageRateLimit** . Certifique-se de considerar isso quando você estiver desenvolvendo uma entrega acompanhamento do sistema, especialmente se o aplicativo usa uma caixa de correio que os usuários se conectam por meio do Outlook. Quando itens adiadas são armazenados na pasta Rascunhos ou de caixa de saída, os usuários podem interpretar como um erro. 
  
O parâmetro de política **RecipientRateLimit** Especifica o limite no número de destinatários que um usuário pode endereçar em um período de 24 horas. Por exemplo, se esse valor é definido como 500, isso significa que uma única conta de caixa de correio do Exchange pode enviar mensagens para nenhum dia de mais de 500 destinatários. Esse limite é aplicável às mensagens para destinatários que estão dentro e fora da organização. Esse limite padrão pode causar problemas para alguns aplicativos de linha de negócios que faça execuções de faturas do final do mês e precisam enviar mensagens para maior do que esse número de destinatários. Você pode usar os serviços externos que permitem o processamento em lotes de mensagens ou soluções de retransmissão de saída de locais separados para contornar esta limitação. 
  
O parâmetro de política de **ForwardeeLimit** Especifica o número máximo de destinatários que as mensagens podem ser encaminhadas ou redirecionadas para por meio de regras de caixa de entrada. Esse parâmetro não limita o número de mensagens que podem ser encaminhadas ou redirecionados para os destinatários. 
  
## <a name="errors-generated-when-throttling-limits-are-exceeded"></a>Erros gerados quando os limites de limitação são excedidos
<a name="bk_ThrottlingErrors"> </a>

Quando limitação as diretivas são excedidos, EWS gera um dos erros listados na tabela a seguir.
  
**Tabela 3: Erros de limite limitação**

|**Erro**|**Parâmetro de política de limitação**|**Descrição**|
|:-----|:-----|:-----|
|ErrorExceededConnectionCount  <br/> |**EWSMaxConcurrency** <br/> |Indica que não existem mais solicitações simultâneas com base no servidor que o permitido pela política do usuário.  <br/> |
|ErrorExceededSubscriptionCount  <br/> |**EWSMaxSubscriptions** <br/> |Indica que um usuário da contagem de assinatura máximo foi excedida de política de limitação.  <br/> |
|ErrorExceededFindCountLimit  <br/> |**EWSFindCountLimit** <br/> |Indica que uma chamada de operação de pesquisa excedeu o número total de itens que podem ser retornadas.  <br/> |
|ErrorServerBusy  <br/> |**EWSPercentTimeInMailboxRPC** **EWSPercentTimeInCAS** **EWSPercentTimeInAD**                   <br/> |Ocorre quando o servidor está ocupado. O valor de BackOffMilliseconds retornado com erros ErrorServerBusy indica para o cliente a quantidade de tempo que ele deve aguardar até que ele deve reenviar a solicitação que causou a resposta que retornou este código de erro.  <br/> |
   
A tabela a seguir lista os códigos de status HTTP que são retornados por erros de limitação.
  
**Tabela 4: Códigos de status HTTP retornados por erros de limitação**

|**Código de status HTTP**|**Descrição**|
|:-----|:-----|
|HTTP 503  <br/> |Indica que o EWS solicitações são enfileiramento com o IIS. O cliente deve atrasar a enviar solicitações adicionais até um momento posterior.  <br/> |
|HTTP 500  <br/> |Indica um erro de servidor interno com o código de erro ErrorServerBusy. Isso indica que o cliente deve atrasar enviando solicitações adicionais até um momento posterior. A resposta pode conter uma dica chamada BackOffMilliseconds de retirada. Se presente, o valor da BackOffMilliseconds deverão ser usado como a duração, até que o cliente reenvia uma solicitação.  <br/> |
|HTTP 200  <br/> |Contém uma resposta de erro baseada em esquema EWS com um código de erro ErrorInternalServerError. Um código de erro ErrorServerBusy inner pode estar presente. Isso indica que o cliente deve atrasar enviando solicitações adicionais até um momento posterior.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Gerenciamento de carga de trabalho do Exchange](http://technet.microsoft.com/en-us/library/jj150503.aspx)
- [Cmdlet New-ThrottlingPolicy](http://technet.microsoft.com/en-us/library/dd351045.aspx)
- [Noções básicas sobre políticas de limitação do cliente](http://technet.microsoft.com/en-us/library/dd297964.aspx)
- [Classe de ThrottlingPolicy](http://msdn.microsoft.com/en-us/library/ff342496%28v=EXCHG.140%29.aspx)
- [Políticas de limitação e o EWSFindCountLimit](http://blogs.msdn.com/b/exchangedev/archive/2010/03/12/throttling-policies-and-the-ewsfindcountlimit.aspx)
- [Instantâneos de orçamento nos Logs do IIS](http://blogs.msdn.com/b/exchangedev/archive/2010/03/10/budget-snapshots-in-the-iis-logs.aspx)
- [Efeitos da limitação na sua implantação do Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/27/456040.aspx)
- [Associações de política de limitação no Exchange 2010 SP1](http://msexchangeteam.com/archive/2010/08/02/455707.aspx)
- [Políticas de limitação e CPUStartPercent](http://blogs.msdn.com/b/exchangedev/archive/2010/03/11/throttling-policies-and-cpustartpercent.aspx)
- [Representação e EWS no Exchange](impersonation-and-ews-in-exchange.md)
    

