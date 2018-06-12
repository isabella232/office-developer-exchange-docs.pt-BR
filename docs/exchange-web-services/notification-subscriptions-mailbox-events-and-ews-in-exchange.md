---
title: Inscrições de notificação, eventos de caixa de correio e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Saiba mais sobre inscrições de notificação e evento de caixa de correio no EWS no Exchange.
ms.openlocfilehash: 4f466c6cc01af410807948a9fec40c2af399c3e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750949"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Inscrições de notificação, eventos de caixa de correio e EWS no Exchange

Saiba mais sobre inscrições de notificação e evento de caixa de correio no EWS no Exchange.
  
Você pode usar a API gerenciada de EWS e os serviços Web do Exchange (EWS) para inscrever-se para receber notificações quando ocorrem eventos em uma caixa de correio ou em uma ou mais das pastas em uma caixa de correio. Existem três tipos de assinatura: streaming notificações, recebam notificações e notificações de push. Cada um desses tipos de assinatura usa diferentes técnicas para receber ou recuperar as notificações.
  
## <a name="getting-notifications---what-are-my-options"></a>Obtendo notificações - quais são minhas opções?
<a name="bk_notiftypes"> </a>

EWS inclui três tipos de assinatura que funcionam de forma independente para notificar o cliente de alterações no servidor. Não importa qual tipo de assinatura que você escolher, você vai têm acesso a todos os mesmos eventos de notificação no final - é apenas uma questão de como conectá-los.
  
**Tabela 1. Tipos de assinatura**

|**Opção**|**Descrição**|**É certo para mim?**|
|:-----|:-----|:-----|
|Notificações de fluxo contínuo  <br/> |Notificações enviadas pelo servidor por meio de uma conexão que permanece aberta por um período de tempo especificado.  <br/> |Notificações de streaming geralmente são recomendadas para a maioria dos aplicativos. Eles são semelhantes às notificações de recepção e envio e oferecem o melhor dos dois mundos. Depois de estabelecer sua assinatura de notificação, a conexão permanecerá aberta para até 30 minutos permitir que o servidor as notificações por push para o cliente. Não há necessidade para solicitar atualizações, como faria com uma inscrição de recepção e você não precisa criar um aplicativo de escuta do serviço web como você faria com uma inscrição de envio.  <br/> |
|Notificações de recepção  <br/> |Notificações que solicitou (ou extraídas) pelo cliente.  <br/> |Notificações de recepção são geralmente mais apropriadas para clientes menos rígidos, onde o cliente não é confiável conectado à rede. Notificações de recepção podem criar o excesso de tráfego entre o cliente e o servidor porque o cliente está enviando solicitações frequentes no servidor para recuperar as notificações e nem todas as solicitações resultam em notificações recuperadas.  <br/> |
|Push notifications  <br/> |Notificações que são enviadas (ou enviadas) pelo servidor para um cliente web service através de um endereço de retorno de chamada.  <br/> |Geralmente, as notificações por push fornecem para a menor latência de notificação que as notificações de recepção e são adequadas para a ligação estreita clientes para o qual o servidor tem acesso confiável e o cliente for IP endereçável. No entanto, as notificações por push tem saído favorecer desde o advento do streaming notificações no Exchange 2010. Se possível, recomendamos que você use as notificações de streaming em vez de notificações de push no futuro. As notificações por push exigem que você escreva um aplicativo de escuta, que é onde as notificações são enviadas para. Isso tem um pequeno benefício sobre notificações de recepção em que ele reduz o tráfego de transmissão, mas ele adiciona sobrecarga exigindo um aplicativo separado.  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>Quais eventos EWS pode assinar para?
<a name="bk_eventtypes"> </a>

Os tipos de eventos do EWS que clientes assinam são definidos pela enumeração [EventType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) para a API gerenciada de EWS ou o elemento [EventType](http://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx) para o EWS. Os eventos EWS a seguir estão disponíveis para a assinatura: 
  
- NewMail — Uma nova mensagem chegou na caixa de entrada.
    
- Excluído — Uma mensagem era difícil excluído da caixa de entrada. Para saber mais sobre as notificações de item excluído, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md) e [receber notificações de eventos de caixa de correio relacionadas a exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md).
    
- Modificado — Um item ou pasta foi alterada.
    
- Movido — Um item ou pasta foi movida. 
    
- Copiada — Um item ou pasta foi copiada.
    
- Criada — Um item ou pasta foi criada. 
    
- FreeBusyChanged — Informações de disponibilidade do usuário foi alteradas.
    
Outro tipo de evento do EWS, o evento de Status, é definido pelo elemento [EventType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) , mas você não assinar este evento. Em vez disso, ele é enviado pelo servidor para verificar o status do cliente para notificações de push e de fluxo contínuo apenas. O cliente precisa responder a este evento necessidades ou o tempo limite de cliente. 
  
Uma ação do usuário único frequentemente resulta na criação de várias notificações. Para ilustrar isso, a figura a seguir mostra alguns cenários comuns e as notificações criadas para cada um deles. Configurações do cliente tem um impacto sobre as notificações recebidas, para que isso não é uma lista completa de todas as opções de configuração e notificações resultantes.
  
**Figura 1. Tipos de evento retornados pela inscrições de notificação**

![A table that shows the notifications sent in common user scenarios, such as receiving new email, creating a new folder, moving a folder, and so on.](media/Exchange2013_Notifications_Events.png)
  
Figura 1 simplifica o processo de notificação. Na realidade, várias notificações (até mesmo várias notificações do mesmo tipo) podem ser criadas para uma ação de usuário único. Por exemplo, no caso de uma operação de movimentação de pasta, três eventos de pasta são criados: um para a pasta que está sendo modificada, um para a pasta pai antiga e outro para a nova pasta pai. Porque numerosos eventos podem ser disparados para uma única operação, recomendamos que você [Crie um tempo de espera de alguns segundos em suas operações de sincronização](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices), para que você sincronizará apenas quando a ação for concluída, em vez de parcialmente até a operação.
  
Também é importante perceber que as definições de configuração que cada usuário escolhe afetará a qual as notificações são criadas. Por exemplo, dados de ocupado livre de alguns dos usuários serão atualizados automaticamente e o evento FreeBusyChanged é criado quando uma nova solicitação de reunião é recebida, mesmo antes que eles tenha lido o item. Para outros usuários, dados ocupados livres não estão atualizados e o evento FreeBusyChanged não for criado até depois que a reunião foi aceita. Essas configurações podem ter um impacto considerável sobre as notificações criadas pelo servidor.
  
## <a name="how-do-ews-notifications-work"></a>Como funcionam as notificações de EWS?
<a name="bk_howwork"> </a>

Notificações de EWS são manipuladas por assinatura. Geralmente, há uma inscrição por caixa de correio e na assinatura de caixa de correio você pode se inscrever para algumas ou todas as pastas. Você decide qual tipo de notificação para assinar (streaming, pull ou push) e que tipo de eventos você gostaria de receber (NewMail, criado, Deleted, modificado, etc.) e, em seguida, você pode criar uma assinatura. Os eventos do EWS, em seguida, são enviados assincronamente do servidor de caixa de correio para o cliente. (Lição de histórico: eventos são síncronos no Exchange 2007 - e eventos são armazenados no servidor de acesso para cliente no Exchange 2010, mas não mais!).
  
Dependendo do tipo de assinatura que você tem, das maneiras em que as notificações são enviadas para o cliente variam. Esta seção descreve como cada tipo de assinatura funciona em mais detalhes.
  
### <a name="ews-streaming-notifications"></a>Notificações de streaming do EWS
<a name="bk_streamnotif"> </a>

Notificações de streaming dependem de um deslocado solicitação get, no servidor para manter uma conexão de assinatura streaming aberta, para que todos os eventos que ocorrem durante a conexão está ativo são transmitidos para o cliente imediatamente. Várias notificações podem ser enviadas ao longo de uma conexão único e o permanece conexão aberta até que o intervalo expirar, ou para um máximo de 30 minutos. Depois que a conexão expira, o cliente envia o deslocado novamente a solicitação get. A Figura 2 mostra como streaming assinaturas e notificações de streaming funcionam.
  
**Figura 2. Visão geral de notificação de streaming**

![An illustration that shows how streaming notifications work. To set up streaming notifications: 1. Subscribe, 2. Open connection, 3. Wait for events, 4. Receive events, repeat 3 and 4, 5. Close or keep connection, 6. Unsubscribe or timeout.](media/Exchange2013_Notifications_StreamSub.png)
  
Para obter informações sobre a criação de notificações de streaming, consulte [notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-pull-notifications"></a>Notificações de recepção EWS
<a name="bk_pullnotif"> </a>

Notificações de recepção baseiam-se no cliente solicitando as notificações em um intervalo que gerencia o cliente. Isso pode resultar em respostas GetEvents com nenhuma notificação. A Figura 3 mostra como notificações de recepção e inscrições de recepção funcionam.
  
**Figura 3. Visão geral de notificação de recepção**

![An illustration that shows how pull notifications work. To set up pull notifications: 1. Subscribe, 2. Send GetEvents, 3. Receive response, repeat 2 and 3, 4. Close or keep connection, 5. Unsubscribe or timeout.](media/Exchange2013_Notifications_PullSub.png)
  
Para obter informações sobre a criação de notificações de recepção, consulte [notificações de recepção sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-push-notifications"></a>Notificações de push do EWS
<a name="bk_pushnotif"> </a>

As notificações por push contam com o servidor de envio de notificações de volta para o cliente. Não há tráfego somente se houver uma notificação. Figura 4 mostra como inscrições de envio e notificações por push trabalham.
  
**Figura 4. Visão geral de notificação de push**

![An illustration that shows how push notifications work. To setup push notifications: 1. Create listener, 2. Subscribe, 3. Wait for events, 4. Receive events, 5. Send "OK" response, repeat 3, 4, and 5, 6. Unsubscribe or timeout.](media/Exchange2013_Notifications_PushSub.png)
  
Se você estiver usando [as notificações por push com o Exchange 2010](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx), considere a atualização do seu aplicativo para [usar notificações de streaming](http://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5), para que você não precisa de um aplicativo separado para receber os eventos.
  
## <a name="how-do-i-subscribe-to-notifications"></a>Como se inscrever para notificações?
<a name="bk_notifoperations"> </a>

Dependendo do tipo de assinatura que você gostaria de criar, você tem um número de opções à sua escolha para a assinatura de notificações.
  
**Tabela 2. Operações e métodos para a assinatura de notificações**

|**Tipo de assinatura**|**Operação do EWS**|**Métodos de API gerenciada de EWS**|**O que ele faz**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Inscrever-se a operação](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService.BeginSubscribeToStreamingNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BeginSubscribeToStreamingNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToStreamingNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar notificações de fluxo contínuo.  <br/> |
|Recepção  <br/> |[Inscrever-se a operação](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService.BeginSubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BeginSubscribeToPullNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPullNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar notificações de recepção.  <br/> |
|Push  <br/> |[Inscrever-se a operação](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService.BeginSubscribeToPushNotifications sobrecarregado](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método de sobrecarga de ExchangeService.BeginSubscribeToPushNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPushNotifications sobrecarregado](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPushNotificationsOnAllFolders sobrecarregado](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar notificações por push.  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>Como posso obter eventos EWS?
<a name="bk_getevents"> </a>

Depois que a assinatura é criada, o modo no qual os eventos reais são enviados para o cliente depende do tipo de assinatura. 
  
Para notificações de fluxo contínuo, uma conexão streaming de assinatura deve ser criado e, em seguida, a assinatura é adicionada para a conexão. Você pode ler mais sobre esse processo em [notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Para notificações de recepção, o objeto de inscrição foi inicializado quando a assinatura foi criada, portanto, você tem apenas chamar o método **GetEvent** ou a operação para recuperar os eventos do servidor. Você pode ler mais sobre isso em [receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
A tabela a seguir lista as operações e classes exigidas para recuperar eventos. 
  
**Tabela 3. Elementos e classes para criar uma conexão e Obtendo eventos**

|**Tipo de assinatura**|**Operação do EWS**|**Método API gerenciada de EWS**|**O que ele faz**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |[Método StreamingSubscriptionConnection.AddSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |Cria um deslocado solicitação get no servidor, o que é respondida quando ocorrem eventos.  <br/> |
|Recepção  <br/> |[Operação GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |[Método PullSubscription.GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |Obtém recebam eventos de notificação do servidor.  <br/> |
|Push  <br/> |Não aplicável.  <br/> |Não aplicável.  <br/> |As notificações por push são enviadas automaticamente ao ouvinte de serviço da web (a URL de retorno de chamada especificado na solicitação de assinatura). Nenhuma operações ou métodos adicionais precisam ser chamado.  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>Como cancelar a notificações?
<a name="bk_notifunsubscribe"> </a>

A tabela a seguir lista as maneiras em que você pode cancelar a cada tipo de assinatura.
  
**Tabela 4. Operações e métodos para cancelar a assinatura de notificações**

|**Tipo de assinatura**|**EWS**|**API gerenciada do EWS**||
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Cancelar a operação](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método StreamingSubscription.BeginUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription.EndUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription.Unsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Recepção  <br/> |[Cancelar a operação](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método PullSubscription.BeginUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription.EndUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription.Unsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Push  <br/> |Retornar o **cancelamento da assinatura** no elemento [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) do [SendNotificationResponseMessage](http://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) <br/> |Não aplicável. Permitir que o tempo limite de inscrição em vez disso.  <br/> ||
   
Como alternativa, você pode permitir que cada um do tempo limite de assinaturas. 
  
**Tabela 5. Tempos limites de assinatura**

|**Tipo de assinatura**|**Valor de tempo limite no EWS**|**Valor de tempo limite da API gerenciada do EWS**|**Manipulação de tempo limite**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |Elemento [ConnectionTimeout](http://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx)  <br/> | parâmetro de *tempo de vida* do construtor [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx)  <br/> |Para a API gerenciada de EWS, depois o valor de tempo limite, o evento [OnDisconnect](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx) é gerado. Se o método [StreamingSubscriptionConnection.Open](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) não for chamado, a conexão será fechada.  <br/> Para o EWS, depois o valor de tempo limite, a mensagem [GetUserConfigurationResponse](http://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) retorna um valor de [ConnectionStatus](http://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) fechado.  <br/> |
|Recepção  <br/> |Elemento de [tempo limite](http://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx)  <br/> | parâmetro de *tempo limite* do método [SubscribeToPullNotification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  <br/> |Depois que o valor de tempo limite estiver esgotado, o servidor exclui a assinatura.  <br/> |
|Push  <br/> |Elemento [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)  <br/> | *frequência* de parâmetro do método [SubscribeToPushNotification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  <br/> |Se o servidor não recebe uma resposta a uma notificação de push ou ping de status, ele repete enviando a notificação várias vezes, antes de parar o envio de notificações. Para obter mais informações, consulte [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx).  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>Pode limitar o assinaturas?
<a name="bk_limitsubs"> </a>

Em uma implantação local, você pode limitar o número de inscrições por usuário com o [parâmetro de limitação de EwsMaxSubscriptions](ews-throttling-in-exchange.md) da diretiva de limitação. Essa diretiva pode ser aplicada a todos os usuários ou apenas determinados usuários. **EwsMaxSubscriptions** política de limitação não é configurável para o Exchange Online. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_limitsubs"> </a>

- [Notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
- [Referência de serviços Web do Exchange](../web-service-reference/web-services-reference-for-exchange.md)
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
- [Aplicativo de amostra de notificação de push](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

