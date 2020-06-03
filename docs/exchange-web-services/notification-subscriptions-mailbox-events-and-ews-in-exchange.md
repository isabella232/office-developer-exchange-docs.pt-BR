---
title: Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Saiba mais sobre inscrições de notificação e evento de caixa de correio no EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 2a99b1922e021a8f5f221381d7f2965c3e1ab504
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459341"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange

Saiba mais sobre inscrições de notificação e evento de caixa de correio no EWS no Exchange.
  
Você pode usar a API gerenciada do EWS e o EWS (serviços Web do Exchange) para inscrever-se para receber notificações quando os eventos ocorrerem em uma caixa de correio ou em uma ou mais pastas de uma caixa de correio. Há três tipos de assinatura disponíveis: notificações de streaming, notificações de recebimento e notificações por push. Cada um desses tipos de assinatura usa diferentes técnicas para receber ou recuperar as notificações.
  
## <a name="getting-notifications---what-are-my-options"></a>Obtendo notificações – quais são as minhas opções?
<a name="bk_notiftypes"> </a>

O EWS inclui três tipos de assinatura que funcionam de forma independente para notificar o cliente sobre as alterações no servidor. Independentemente do tipo de assinatura escolhido, você terá acesso a todos os mesmos eventos de notificação no final-é apenas uma questão de como obtê-los.
  
**Tabela 1. Tipos de assinatura**

|**Opção**|**Descrição**|**Está certo para mim?**|
|:-----|:-----|:-----|
|Notificações de streaming  <br/> |Notificações enviadas pelo servidor por meio de uma conexão que permanece aberta por um período de tempo especificado.  <br/> |As notificações de streaming geralmente são recomendadas para a maioria dos aplicativos. Eles são semelhantes às notificações pull e push e oferecem o melhor de ambos os mundos. Após estabelecer sua assinatura de notificação, a conexão permanecerá aberta por até 30 minutos para permitir que o servidor envie notificações de volta para o cliente. Não é necessário solicitar atualizações, como faria com uma assinatura pull, e você não precisa criar um aplicativo de ouvinte de serviço Web como faria com uma assinatura push.  <br/> |
|Notificações de recepção  <br/> |Notificações que são solicitadas (ou puxadas) pelo cliente.  <br/> |As notificações de recebimento são geralmente mais apropriadas para clientes com rigidez de acoplamento, onde o cliente não está conectado à rede com segurança. As notificações de recepção podem criar tráfego em excesso entre o cliente e o servidor porque o cliente está enviando solicitações frequentes ao servidor para recuperar notificações, e nem todas as solicitações resultam em notificações recuperadas.  <br/> |
|Notificações de Push  <br/> |Notificações enviadas (ou enviadas) pelo servidor para um serviço Web no lado do cliente por meio de um endereço de retorno de chamada.  <br/> |Geralmente, as notificações por push fornecem latência de notificação menor do que as notificações de recebimento e são adequadas para clientes com acoplamento rígido para os quais o servidor tem acesso confiável e o cliente é endereçável por IP. No entanto, as notificações por push foram retiradas do favor desde o surgimento de notificações de streaming no Exchange 2010. Se possível, recomendamos que você use as notificações de streaming em vez de notificações por push no futuro. As notificações por push exigem que você crie um aplicativo de ouvinte, onde as notificações são enviadas. Isso tem um ligeiro benefício sobre as notificações de recebimento, pois reduz o tráfego de conexão, mas adiciona sobrecarga solicitando um aplicativo separado.  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>Quais eventos do EWS posso me inscrever?
<a name="bk_eventtypes"> </a>

Os tipos de eventos EWS nos quais os clientes se inscrevem são definidos pela enumeração [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) para a API gerenciada do EWS ou o elemento [EventType](https://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx) do EWS. Os eventos EWS a seguir estão disponíveis para assinatura: 
  
- NewMail — uma nova mensagem chegou na caixa de entrada.
    
- Excluído — uma mensagem foi excluída da caixa de entrada. Para saber mais sobre notificações de item excluído, consulte [excluindo itens usando EWS no Exchange](deleting-items-by-using-ews-in-exchange.md) e [notificações de recepção para eventos de caixa de correio relacionados à exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md).
    
- Modified — um item ou pasta foi alterado.
    
- Movido — um item ou pasta foi movido. 
    
- Copiado — um item ou pasta foi copiado.
    
- Criado — um item ou pasta foi criado. 
    
- FreeBusyChanged — as informações de disponibilidade de um usuário foram alteradas.
    
Outro tipo de evento do EWS, o evento status, é definido pelo elemento [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) , mas você não assina esse evento. Em vez disso, ele é enviado pelo servidor para verificar o status do cliente somente para notificações por push e streaming. O cliente precisa responder a essas necessidades de evento ou o cliente expirará. 
  
Uma ação única do usuário com frequência resulta na criação de várias notificações. Para ilustrar isso, a figura a seguir mostra alguns cenários comuns e as notificações criadas para cada um. As configurações do cliente têm um impacto nas notificações recebidas, portanto, esta não é uma lista completa de todas as opções de configuração e notificações resultantes.
  
**Figura 1. Tipos de eventos retornados por assinaturas de notificação**

![A table that shows the notifications sent in common user scenarios, such as receiving new email, creating a new folder, moving a folder, and so on.](media/Exchange2013_Notifications_Events.png)
  
A Figura 1 simplifica o processo de notificação. Na realidade, várias notificações (mesmo várias notificações do mesmo tipo) podem ser criadas para uma única ação do usuário. Por exemplo, no caso de uma operação de movimentação de pasta, três eventos de pasta são criados: um para a pasta que está sendo modificada, um para a pasta pai antiga e outro para a nova pasta pai. Como numerosos eventos podem ser disparados para uma única operação, recomendamos que você [crie um tempo de espera de alguns segundos em suas operações de sincronização](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices), para que você só sincronize quando a ação for concluída, em vez de partway por meio da operação.
  
Também é importante perceber que as definições de configuração que cada usuário escolhe irão afetar as notificações criadas. Por exemplo, os dados de disponibilidade de alguns usuários são atualizados automaticamente e o evento FreeBusyChanged é criado quando uma nova solicitação de reunião é recebida, mesmo antes de ler o item. Para outros usuários, os dados de disponibilidade não são atualizados e o evento FreeBusyChanged não é criado até que a reunião tenha sido aceita. Essas configurações podem ter um impacto considerável sobre as notificações criadas pelo servidor.
  
## <a name="how-do-ews-notifications-work"></a>Como funcionam as notificações do EWS?
<a name="bk_howwork"> </a>

As notificações do EWS são tratadas de acordo com a assinatura. Normalmente, há uma assinatura por caixa de correio e dentro da assinatura da caixa de correio você pode inscrever-se em algumas ou em todas as pastas. Você decide que tipo de notificação inscrever (transmitir, puxar ou enviar) e que tipo de eventos você gostaria de receber (NewMail, Created, Deleted, Modified etc.) e, em seguida, criar uma assinatura. Os eventos do EWS são enviados de forma assíncrona do servidor de caixa de correio para o cliente. (Lição de histórico: os eventos são síncronos no Exchange 2007-e os eventos são armazenados no servidor de acesso para cliente no Exchange 2010, mas não mais!).
  
Dependendo do tipo de assinatura que você tem, as maneiras nas quais as notificações são enviadas para o cliente variam. Esta seção descreve como cada tipo de assinatura funciona em mais detalhes.
  
### <a name="ews-streaming-notifications"></a>Notificações de streaming do EWS
<a name="bk_streamnotif"> </a>

As notificações de streaming contam com uma solicitação de Get suspensa no servidor para manter uma conexão de assinatura de streaming aberta, para que qualquer evento que ocorra enquanto a conexão estiver ativa será transmitido para o cliente imediatamente. Várias notificações podem ser enviadas durante uma única conexão, e a conexão permanece aberta até que o intervalo expire, ou por um máximo de 30 minutos. Depois que a conexão expirar, o cliente enviará a solicitação de obtenção suspensa novamente. A Figura 2 mostra como as assinaturas de streaming e as notificações de streaming funcionam.
  
**Figura 2. Visão geral da notificação de streaming**

![An illustration that shows how streaming notifications work. To set up streaming notifications: 1. Subscribe, 2. Open connection, 3. Wait for events, 4. Receive events, repeat 3 and 4, 5. Close or keep connection, 6. Unsubscribe or timeout.](media/Exchange2013_Notifications_StreamSub.png)
  
Para obter informações sobre a criação de notificações de streaming, consulte [Stream notifications about Mailbox Events by using EWS in Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-pull-notifications"></a>Notificações pull do EWS
<a name="bk_pullnotif"> </a>

As notificações de recebimento dependem do cliente que solicita as notificações em um intervalo que o cliente gerencia. Isso pode resultar em respostas GetEvents sem notificações. A Figura 3 mostra como funcionam as assinaturas pull e as notificações de recepção.
  
**Figura 3. Visão geral da notificação pull**

![An illustration that shows how pull notifications work. To set up pull notifications: 1. Subscribe, 2. Send GetEvents, 3. Receive response, repeat 2 and 3, 4. Close or keep connection, 5. Unsubscribe or timeout.](media/Exchange2013_Notifications_PullSub.png)
  
Para obter informações sobre como criar notificações pull, consulte [pull notifications about Mailbox Events by using EWS in Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-push-notifications"></a>Notificações por push do EWS
<a name="bk_pushnotif"> </a>

As notificações por push dependem do servidor enviando notificações de volta para o cliente. Há apenas tráfego se houver uma notificação. A Figura 4 mostra como as assinaturas push e as notificações por push funcionam.
  
**Figura 4. Visão geral da notificação por push**

![An illustration that shows how push notifications work. To setup push notifications: 1. Create listener, 2. Subscribe, 3. Wait for events, 4. Receive events, 5. Send "OK" response, repeat 3, 4, and 5, 6. Unsubscribe or timeout.](media/Exchange2013_Notifications_PushSub.png)

Se você estiver usando [notificações por push com o Exchange 2010](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx), considere atualizar seu aplicativo para [usar notificações de streaming](https://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5), para que você não precise de um aplicativo separado para receber os eventos.

  
## <a name="how-do-i-subscribe-to-notifications"></a>Como eu assino as notificações?
<a name="bk_notifoperations"> </a>

Dependendo do tipo de assinatura que você gostaria de criar, você tem várias opções para optar por assinar as notificações.
  
**Tabela 2. Operações e métodos para assinar notificações**

|**Tipo de assinatura**|**Operação do EWS**|**Métodos da API gerenciada do EWS**|**Função**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService. BeginSubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. BeginSubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. SubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar notificações de streaming.  <br/> |
|Receber  <br/> |[Operação Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService. BeginSubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. BeginSubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService. SubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para inscrever-se nas notificações de recepção.  <br/> |
|Coloca  <br/> |[Operação Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método sobrecarregado ExchangeService. BeginSubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método de sobrecarga ExchangeService. BeginSubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método sobrecarregado ExchangeService. SubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método sobrecarregado ExchangeService. SubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para inscrever-se nas notificações por push.  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>Como obtenho eventos do EWS?
<a name="bk_getevents"> </a>

Após a criação da assinatura, a maneira como os eventos reais são enviados para o cliente depende do tipo de assinatura. 
  
Para notificações de streaming, uma conexão de assinatura de streaming deve ser criada e, em seguida, a assinatura é adicionada à conexão. Você pode ler mais sobre esse processo em [notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Para notificações de recebimento, o objeto Subscription foi inicializado quando a assinatura foi criada, de modo que você só precisa chamar o método **GetEvent** ou a operação para recuperar os eventos do servidor. Você pode ler mais sobre isso em [notificações pull sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
A tabela a seguir lista as operações e as classes necessárias para recuperar eventos. 
  
**Tabela 3. Elementos e classes para criar uma conexão e obter eventos**

|**Tipo de assinatura**|**Operação do EWS**|**Método de API gerenciada do EWS**|**Função**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |[Método StreamingSubscriptionConnection. AddSubscription](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação get suspensa no servidor, que é respondida quando ocorre um evento.  <br/> |
|Receber  <br/> |[Operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |[Método PullSubscription. GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |Obtém eventos de notificação pull do servidor.  <br/> |
|Coloca  <br/> |Não aplicável.  <br/> |Não aplicável.  <br/> |As notificações por push são enviadas automaticamente para o ouvinte do serviço Web (a URL de retorno de chamada especificada na solicitação de assinatura). Nenhum método ou operação adicional precisa ser chamado.  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>Como cancelar a assinatura de notificações?
<a name="bk_notifunsubscribe"> </a>

A tabela a seguir lista as maneiras nas quais você pode cancelar a assinatura de cada tipo de assinatura.
  
**Tabela 4. Operações e métodos para inscrever-se em notificações**

|**Tipo de assinatura**|**EWS**|**API gerenciada do EWS**||
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Cancelar a operação](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método StreamingSubscription. BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription. EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription. unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Receber  <br/> |[Cancelar a operação](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método PullSubscription. BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription. EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription. unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Coloca  <br/> |Retornar **unsubscribe** no elemento [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) do [SendNotificationResponseMessage](https://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) <br/> |Não aplicável. Em vez disso, deixe o tempo limite da assinatura.  <br/> ||
   
Como alternativa, você pode deixar o tempo limite de cada assinatura. 
  
**Tabela 5. Tempo limite de assinatura**

|**Tipo de assinatura**|**Valor de tempo limite no EWS**|**Valor de tempo limite na API gerenciada do EWS**|**Tratamento de tempo limite**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |Elemento [connectionTimeout](https://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx)  <br/> | parâmetro *Lifetime* do construtor [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx)  <br/> |Para a API gerenciada do EWS, após o valor de tempo limite ser decorrido, o evento [OnDisconnect](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx) é gerado. Se o método [StreamingSubscriptionConnection. Open](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) não for chamado, a conexão será fechada.  <br/> Para o EWS, após o valor de tempo limite ser decorrido, a mensagem [GetUserConfigurationResponse](https://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) retorna um valor de [ConnectionStatus](https://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) de Closed.  <br/> |
|Receber  <br/> |Elemento [Timeout](https://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx)  <br/> | parâmetro *Timeout* do método [SubscribeToPullNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  <br/> |Depois que o valor de tempo limite expirar, o servidor excluirá a assinatura.  <br/> |
|Coloca  <br/> |Elemento [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)  <br/> | parâmetro *Frequency* do método [SubscribeToPushNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  <br/> |Se o servidor não receber uma resposta a uma notificação por Push ou o ping de status, ele tentará enviar a notificação várias vezes antes de parar de enviar as notificações. Para obter mais informações, consulte [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx).  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>Posso limitar as assinaturas?
<a name="bk_limitsubs"> </a>

Em uma implantação local, você pode limitar o número de assinaturas por usuário com o [parâmetro EwsMaxSubscriptions throttling](ews-throttling-in-exchange.md) da política de limitação. Essa política pode ser aplicada a todos os usuários ou apenas a usuários específicos. A política de limitação do **EwsMaxSubscriptions** não é configurável para o Exchange Online. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_limitsubs"> </a>

- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Tratamento de erros relacionados à notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
- [Referência de serviço Web do Exchange](../web-service-reference/web-services-reference-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
- [Aplicativo de amostra de notificação por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

