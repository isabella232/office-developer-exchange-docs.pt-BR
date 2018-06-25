---
title: Tratando erros relacionados a notificação no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Descubra como lidar com erros relacionados a notificação em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: cb0c16a74e68b5a16ef0f2011f65b22675950f58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750665"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Tratando erros relacionados a notificação no EWS no Exchange

Descubra como lidar com erros relacionados a notificação em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
  
Se seu aplicativo pode assinar e obtém notificações, você pode precisar manipular erros relacionados a notificação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.
  
**Tabela 1. Erros relacionados a notificação e como lidar com elas**

|Erro|Ocorre quando você tenta …|Manipulá-lo pelo …|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |Abra uma conexão para fazer a eventos quando a conta atingiu o limite de conexão de abrir conexões streaming. | <ul><li>Usando a [representação](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) para [Abrir conexões](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Usando menos conexões para obter os eventos. Maximize o número de inscrições em cada conexão [usando afinidade](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md) e [colocar um máximo de 200 assinatura IDs no mesmo grupo](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain). Em seguida, você pode usar a mesma conexão para recuperar eventos para todo o grupo, reduzindo o número de conexões necessárias.</li><li>  Alterando o valor do HangingConnectionLimit no arquivo Web. config do Exchange local para substituir o valor padrão de três conexões abertas. O Exchange Online tem um padrão HangingConnectionLimit de 10, que não é configurável.</li></ul> |
|**ErrorExceededSubscriptionCount** |Crie muitos inscrições. [EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) parâmetro política de limitação determina o número máximo de inscrições que uma conta pode criar. | <ul><li>Usando a [representação](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) para [criar inscrições](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Redução do número de assinaturas.</li></ul> |
|**ErrorInvalidSubscriptionRequest** |Crie assinaturas para várias caixas de correio ou de várias pastas em uma única solicitação.  |Criando uma inscrição de uma única pasta pública ou uma única caixa de correio em uma única solicitação.| 
|**ErrorInvalidWatermark** |Obtenha eventos usando uma marca d'água inválida.| <ul><li>Verificando a ID de assinatura retornados em uma resposta anterior.</li><li>Garantir que você está enviando a ID de assinatura para o objeto **ExchangeService** correto.</li><li>[Criando uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**ErrorMissedNotificationEvents** |Obtenha a eventos quando alguns eventos anteriores foram perdidos.   |Comparando as propriedades da pasta estendido **PR_LOCAL_COMMIT_TIME_MAX** (0x670a) e **PR_DELETED_COUNT_TOTAL** (0x670b) para determinar quais alterações foram perdidas e [Criando uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).  |
|**ErrorProxyRequestNotAllowed** |Assine eventos para um usuário em uma solicitação de lote cuja caixa de correio foi transferida para outro site.   |Usando a [descoberta automática](autodiscover-for-exchange.md) para detectar novamente o ExternalEwsUrl ou EwsPartnerUrl e criando uma nova assinatura.  |
|**ErrorReadEventsFailed** |Obtenha os eventos de uma assinatura que não pode ser encontrada.  |Usando a [descoberta automática](autodiscover-for-exchange.md) para detectar novamente o ExternalEwsUrl ou EwsPartnerUrl e criando uma nova assinatura.  |
|**ErrorServerBusy** | Exceda os limites de [limitação](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) . Lembre-se de limitação referente à seguinte:<ul><li>[EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) limite de limitação identifica o número máximo de push, pull ou streaming inscrições de notificação que podem estar ativas ao mesmo tempo. Esse é o valor de inscrições de caixa de correio, não o número de inscrições de pasta individual em uma assinatura de caixa de correio. Iniciando com versões de caixa de correio do serviço 14.16.0135 e 14.15.0057.000, uma caixa de correio hospedada pelo Exchange Online ou Exchange Online como parte do Office 365 pode ter até 20 assinaturas e um destino Exchange 2013 a caixa de correio pode ter até 5.000 inscrições no local.</li><li>[EwsMaxConcurrency](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) limite de limitação identifica o número máximo de solicitações ativas para conexões não-streaming e tem um valor padrão de 27.</li><li>O limite padrão para conexões abertas do streaming é dez.</li></ul> |<ul><li>[Considerando as implicações das políticas de limitação relacionadas a notificação](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) e limitar o número de inscrições ativas e as conexões ativas para que o aplicativo não seja restringido.</li><li>Usando menos conexões para obter os eventos. Maximize o número de inscrições em cada conexão colocando [um máximo de 200 assinatura IDs no mesmo grupo](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md). Em seguida, você pode usar a mesma conexão para recuperar eventos para todo o grupo, reduzindo o número de conexões necessárias.</li><li>Alterando o valor do HangingConnectionLimit no arquivo Web. config para substituir o valor padrão de dez conexões abertas do streaming.</li></ul>|
|**ErrorSubscriptionNotFound** |Obtenha os eventos de uma assinatura que não pode ser encontrada. A assinatura pode ter expirado, o processo EWS pode ter sido reiniciado, ou uma assinatura inválida foi passada. | <ul><li>Verificando que você está usando a mesma ID de assinatura que foi retornada em uma resposta anterior.</li><li>Garantir que você está enviando a ID de assinatura para o objeto **ExchangeService** correto.</li><li> [Criando uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**[ServiceLocalException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Adicione uma assinatura para uma nova pasta, enquanto uma conexão de inscrição está aberto em outra pasta.  |Alterando a sua assinatura para assinar todas as pastas na caixa de correio, em vez de uma pasta específica.  |
|**[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Obter eventos de uma assinatura que não pode ser localizada no armazenamento do Exchange.  | <ul><li>Verificando que você está usando a mesma ID de assinatura que foi retornada em uma resposta anterior.</li><li>Garantir que você está enviando a ID de assinatura para o objeto **ExchangeService** correto.</li></ul> |
   
## <a name="recovering-from-lost-subscriptions"></a>Recuperação de inscrições perdidas
<a name="bk_recover"> </a>

Quando uma assinatura é perdida ou não esteja mais acessível, é melhor criar uma nova assinatura e não incluir a marca d'água antiga em nova inscrição. Resubscribing com a marca d'água antiga faz uma verificação linear para eventos, que é dispendiosa. Em vez disso, crie uma nova inscrição e comparar as propriedades de pasta para procurar conteúdo for alterado que ocorreu entre a assinatura perdida e a nova assinatura. As propriedades da pasta estendidas que a Microsoft recomenda que você verifique são **PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040) e **PR_DELETED_COUNT_TOTAL** (0x670b0003). Você pode fazer isso criando [uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também

- [Inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    

