---
title: Tratamento de erros relacionados à notificação no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Descubra como lidar com erros relacionados à notificação em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 60edb1344e6b0499ef6d2ed2aefaebde723b42cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528311"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Tratamento de erros relacionados à notificação no EWS no Exchange

Descubra como lidar com erros relacionados à notificação em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.

Se seu aplicativo assinar e receber notificações, talvez seja necessário lidar com erros relacionados à notificação. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.

**Tabela 1. Erros relacionados a notificação e como tratá-los**

|Erro|Ocorre quando você tenta...|Manipulá-lo pelo …|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |Abra uma conexão para obter eventos quando a conta atingiu seu limite de conexão de conexões de streaming abertas. | <ul><li>Usando [representação](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) para [abrir conexões](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Usando menos conexões para obter eventos. Maximize o número de assinaturas em cada conexão usando a [afinidade](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md) e [colocando um máximo de 200 IDs de assinatura no mesmo grupo](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain). Você pode usar a mesma conexão para recuperar eventos para todo o grupo, reduzindo o número de conexões necessárias.</li><li>  Alterar o valor do HangingConnectionLimit no arquivo Web. config para o Exchange local para substituir o valor padrão de três conexões abertas. O Exchange Online tem um HangingConnectionLimit padrão de 10, que não é configurável.</li></ul> |
|**ErrorExceededSubscriptionCount** |Criar muitas assinaturas. O parâmetro de política de limitação [EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) determina o número máximo de assinaturas que uma conta pode criar. | <ul><li>Usando [representação](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) para [criar assinaturas](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Reduzir o número de assinaturas.</li></ul> |
|**ErrorInvalidSubscriptionRequest** |Criar assinaturas para várias caixas de correio ou várias pastas a partir de uma única solicitação.  |Criar uma assinatura para uma única pasta pública ou uma única caixa de correio em uma única solicitação.|
|**ErrorInvalidWatermark** |Obter eventos usando uma marca d' água inválida.| <ul><li>Verificação da ID de assinatura retornada em uma resposta anterior.</li><li>Garantir que você esteja enviando a ID de assinatura para o objeto **ExchangeService** correto.</li><li>[Criar uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**ErrorMissedNotificationEvents** |Obter eventos quando alguns eventos anteriores foram perdidos.   |Comparando as propriedades de pasta estendida **PR_LOCAL_COMMIT_TIME_MAX** (0x670a) e **PR_DELETED_COUNT_TOTAL** (0x670b) para determinar quais alterações foram perdidas e [criar uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).  |
|**ErrorProxyRequestNotAllowed** |Inscrever-se em eventos para um usuário em uma solicitação em lote cuja caixa de correio foi movida para outro site.   |Usando a [descoberta automática](autodiscover-for-exchange.md) para redescobrir o ExternalEwsUrl ou o EwsPartnerUrl e criar uma nova assinatura.  |
|**ErrorReadEventsFailed** |Obter eventos de uma assinatura que não pode ser encontrado.  |Usando a [descoberta automática](autodiscover-for-exchange.md) para redescobrir o ExternalEwsUrl ou o EwsPartnerUrl e criar uma nova assinatura.  |
|**ErrorServerBusy** | Exceder limites de [limitação](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) . Esteja ciente do seguinte em relação à limitação:<ul><li>O limite de limitação [EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) identifica o número máximo de assinaturas de notificação de envio, recepção ou de fluxo contínuo que podem estar ativas de uma só vez. Esse é o valor das assinaturas de caixa de correio, não o número de assinaturas de pastas individuais em uma assinatura de caixa de correio. Iniciando com as versões de caixa de correio de serviço 14.16.0135 e 14.15.0057.000, uma caixa de correio hospedada pelo Exchange Online ou Exchange Online como parte do Office 365 pode ter até 20 assinaturas e uma caixa de correio local de destino do Exchange 2013 pode ter até 5000 assinaturas.</li><li>O limite de limitação [EwsMaxConcurrency](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) identifica o número máximo de solicitações ativas para conexões não streaming e tem um valor padrão de 27.</li><li>O limite padrão para conexões de streaming abertas é dez.</li></ul> |<ul><li>[Considerar as implicações das políticas de limitação relacionadas à notificação](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) e limitar o número de assinaturas ativas e as conexões ativas para que o aplicativo não fique limitado.</li><li>Usando menos conexões para obter eventos. Maximize o número de assinaturas em cada conexão, [colocando um máximo de 200 IDs de assinatura no mesmo grupo](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md). Você pode usar a mesma conexão para recuperar eventos para todo o grupo, reduzindo o número de conexões necessárias.</li><li>Alterar o valor do HangingConnectionLimit no arquivo Web. config para substituir o valor padrão de dez conexões de streaming abertas.</li></ul>|
|**ErrorSubscriptionNotFound** |Obter eventos para uma assinatura que não pode ser encontrada. A assinatura pode ter expirado, o processo EWS pode ter sido reiniciado ou uma assinatura inválida foi passada. | <ul><li>Verificar se você está usando a mesma ID de assinatura retornada em uma resposta anterior.</li><li>Garantir que você esteja enviando a ID de assinatura para o objeto **ExchangeService** correto.</li><li> [Criar uma nova assinatura](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**[Onlocalexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Adicione uma assinatura a uma nova pasta enquanto uma conexão de assinatura estiver aberta em outra pasta.  |Alterar sua assinatura para inscrever-se em todas as pastas da caixa de correio, em vez de uma pasta específica.  |
|**[Naresponseexception](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Obter eventos para uma assinatura que não pode ser localizada no repositório do Exchange.  | <ul><li>Verificar se você está usando a mesma ID de assinatura retornada em uma resposta anterior.</li><li>Garantir que você esteja enviando a ID de assinatura para o objeto **ExchangeService** correto.</li></ul> |

## <a name="recovering-from-lost-subscriptions"></a>Recuperando de assinaturas perdidas
<a name="bk_recover"> </a>

Quando uma assinatura é perdida ou não está mais acessível, é melhor criar uma nova assinatura e não incluir a marca d' água antiga na nova assinatura. Resubscribing com a marca d' água antiga causa uma verificação linear de eventos, o que é dispendioso. Em vez disso, crie uma nova assinatura e compare as propriedades da pasta para procurar alterações de conteúdo que ocorreram entre a assinatura perdida e a nova assinatura. As propriedades de pasta estendidas que recomendamos que você verifique são **PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040) e **PR_DELETED_COUNT_TOTAL** (0x670b0003). Você pode fazer isso [criando uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md).

## <a name="see-also"></a>Confira também

- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)


