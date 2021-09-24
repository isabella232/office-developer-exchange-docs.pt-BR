---
title: Manipulação de erros relacionados a notificações no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Saiba como lidar com erros relacionados à notificação em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 7b49a57b7236318e08cb70ac2ac00edc4cf86363
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520210"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Manipulação de erros relacionados a notificações no EWS no Exchange

Saiba como lidar com erros relacionados à notificação em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.

Se o aplicativo se inscrever e receber notificações, talvez seja preciso lidar com erros relacionados à notificação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.

**Tabela 1. Erros relacionados à notificação e como lidar com eles**

|Erro|Ocorre quando você tenta...|Manipulá-lo pelo …|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |Abra uma conexão para obter eventos quando a conta atingiu seu limite de conexão de conexões de streaming abertas. | <ul><li>Usando [a representação para](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) abrir [conexões](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Usando menos conexões para obter eventos. Maximize o número de assinaturas em cada conexão usando [afinidade](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md) e colocando no máximo [200 IDs](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain)de assinatura no mesmo grupo . Em seguida, você pode usar a mesma conexão para recuperar eventos de todo o grupo, reduzindo o número de conexões necessárias.</li><li>  Alterar o valor do hangingConnectionLimit no arquivo web.config para Exchange local para substituir o valor padrão de três conexões abertas. Exchange Online tem um HangingConnectionLimit padrão de 10, que não é configurável.</li></ul> |
|**ErrorExceededSubscriptionCount** |Crie muitas assinaturas. O parâmetro de política de limite [EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) determina o número máximo de assinaturas que uma conta pode criar. | <ul><li>Usando [a representação](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) para criar [assinaturas](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Reduzindo o número de assinaturas.</li></ul> |
|**ErrorInvalidSubscriptionRequest** |Crie assinaturas para várias caixas de correio ou várias pastas de uma única solicitação.  |Criando uma assinatura para uma única pasta pública ou uma única caixa de correio em uma única solicitação.|
|**ErrorInvalidWatermark** |Obter eventos usando uma marca d'água inválida.| <ul><li>Verificando a ID da assinatura retornada em uma resposta anterior.</li><li>Garantindo que você esteja enviando a ID da assinatura para o objeto **ExchangeService** correto.</li><li>[Criando uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**ErrorMissedNotificationEvents** |Obter eventos quando alguns eventos anteriores foram perdidas.   |Comparando as propriedades  de pasta estendida PR_LOCAL_COMMIT_TIME_MAX (0x670a) e **PR_DELETED_COUNT_TOTAL** (0x670b) para determinar quais alterações foram perdidas e criar uma nova [assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).  |
|**ErrorProxyRequestNotAllowed** |Inscreva-se em eventos para um usuário em uma solicitação em lote cuja caixa de correio foi movida para outro site.   |Usando [a Descoberta Automática](autodiscover-for-exchange.md) para redescobrir ExternalEwsUrl ou EwsPartnerUrl e criar uma nova assinatura.  |
|**ErrorReadEventsFailed** |Obter eventos de uma assinatura que não pode ser encontrada.  |Usando [a Descoberta Automática](autodiscover-for-exchange.md) para redescobrir ExternalEwsUrl ou EwsPartnerUrl e criar uma nova assinatura.  |
|**ErrorServerBusy** | Exceder [limites de limitação.](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) Esteja ciente do seguinte em relação à throttling:<ul><li>O limite de limitação [EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) identifica o número máximo de assinaturas de notificação por push, pull ou streaming que podem estar ativas de uma vez. Esse é o valor das assinaturas de caixa de correio, não o número de assinaturas de pasta individuais em uma assinatura de caixa de correio. A partir das versões 14.16.0135 e 14.15.0057.000, uma caixa de correio hospedada pelo Exchange Online ou Exchange Online como parte do Office 365 pode ter até 20 assinaturas, e uma caixa de correio local de destino Exchange 2013 pode ter até 5.000 assinaturas.</li><li>O limite de limitação [EwsMaxConcurrency](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) identifica o número máximo de solicitações ativas para conexões não streaming e tem um valor padrão de 27.</li><li>O limite padrão para conexões de streaming abertas é dez.</li></ul> |<ul><li>[Considerando as implicações das](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) políticas de limitação relacionadas à notificação e limitando o número de assinaturas ativas e conexões ativas para que o aplicativo não seja limitado.</li><li>Usando menos conexões para obter eventos. Maximize o número de assinaturas em cada conexão colocando no máximo [200 IDs](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)de assinatura no mesmo grupo . Em seguida, você pode usar a mesma conexão para recuperar eventos de todo o grupo, reduzindo o número de conexões necessárias.</li><li>Alterar o valor do arquivo HangingConnectionLimit no arquivo web.config substituir o valor padrão de dez conexões de streaming abertas.</li></ul>|
|**ErrorSubscriptionNotFound** |Obter eventos para uma assinatura que não pode ser encontrada. A assinatura pode ter expirado, o processo EWS pode ter sido reiniciado ou uma assinatura inválida foi passada. | <ul><li>Verificando se você está usando a mesma ID de assinatura que foi retornada em uma resposta anterior.</li><li>Garantindo que você esteja enviando a ID da assinatura para o objeto **ExchangeService** correto.</li><li> [Criando uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**[ServiceLocalException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Adicione uma assinatura a uma nova pasta enquanto uma conexão de assinatura está aberta em outra pasta.  |Alterar sua assinatura para assinar todas as pastas na caixa de correio, em vez de uma pasta específica.  |
|**[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Obter eventos para uma assinatura que não pode ser localizada no Exchange store.  | <ul><li>Verificando se você está usando a mesma ID de assinatura que foi retornada em uma resposta anterior.</li><li>Garantindo que você esteja enviando a ID da assinatura para o objeto **ExchangeService** correto.</li></ul> |

## <a name="recovering-from-lost-subscriptions"></a>Recuperação de assinaturas perdidas
<a name="bk_recover"> </a>

Quando uma assinatura é perdida ou não está mais acessível, é melhor criar uma nova assinatura e não incluir a marca d'água antiga na nova assinatura. A nova assinatura com a marca d'água antiga causa uma verificação linear de eventos, o que é caro. Em vez disso, crie uma nova assinatura e compare as propriedades da pasta para procurar alterações de conteúdo que ocorreram entre a assinatura perdida e a nova assinatura. As propriedades de pasta estendidas  que recomendamos que você verifique são PR_LOCAL_COMMIT_TIME_MAX (0x670a0040) e **PR_DELETED_COUNT_TOTAL** (0x670b0003). Você pode fazer isso criando [uma definição de propriedade estendida.](properties-and-extended-properties-in-ews-in-exchange.md)

## <a name="see-also"></a>Confira também

- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)


