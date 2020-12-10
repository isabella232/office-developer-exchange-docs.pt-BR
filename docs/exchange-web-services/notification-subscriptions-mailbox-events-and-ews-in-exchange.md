---
title: Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Saiba mais sobre assinaturas de notificação e evento de caixa de correio do EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 00a0941e615f35a46bb77c00648b75fcd2a45286
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603838"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange

Saiba mais sobre assinaturas de notificação e evento de caixa de correio do EWS no Exchange.
  
Você pode usar a API Gerenciada do EWS e os Serviços Web do Exchange (EWS) para assinar a fim de receber notificações quando ocorrerem eventos em uma caixa de correio ou em uma ou mais pastas de uma caixa de correio. Há três tipos de assinatura disponíveis: notificações de streaming, notificações por pull e notificações por push. Cada um desses tipos de assinatura usa técnicas diferentes para receber ou recuperar as notificações.
  
## <a name="getting-notifications---what-are-my-options"></a>Obtendo notificações – quais são as minhas opções?
<a name="bk_notiftypes"> </a>

O EWS inclui três tipos de assinatura que funcionam independentemente para notificar o cliente sobre alterações no servidor. Não importa o tipo de assinatura que você escolher, você terá acesso aos mesmos eventos de notificação no final - é apenas uma questão de como você os obtém.
  
**Tabela 1. Tipos de assinatura**

|**Opção**|**Descrição**|**É ideal para mim?**|
|:-----|:-----|:-----|
|Notificações de streaming  <br/> |Notificações enviadas pelo servidor por meio de uma conexão que permanece aberta por um determinado período de tempo.  <br/> |As notificações de streaming geralmente são recomendadas para a maioria dos aplicativos. Elas são semelhantes às notificações por push e pull e oferecem o melhor dos dois mundos. Depois de estabelecer sua assinatura de notificação, a conexão permanece aberta por até 30 minutos para permitir que o servidor envie notificações de volta para o cliente. Não há necessidade de solicitar atualizações, como faria com uma assinatura pull, e você não precisa criar um aplicativo ouvinte de serviço Web como faria com uma assinatura push.  <br/> |
|Notificações por pull  <br/> |Notificações que são solicitadas (ou extraídas) pelo cliente.  <br/> |As notificações por pull são geralmente mais apropriadas para clientes com acoplamento inflexível, onde o cliente não está conectado de forma confiável à rede. As notificações por pull podem criar tráfego excessivo entre o cliente e o servidor porque o cliente envia solicitações frequentes ao servidor para recuperar notificações e nem todas as solicitações resultam em notificações recuperadas.  <br/> |
|Notificações por push  <br/> |Notificações que são enviadas (ou empurradas) pelo servidor para um serviço Web do lado do cliente por meio de um endereço de retorno de chamada.  <br/> |Geralmente, as notificações por push fornecem latência de notificação menor do que as notificações por pull e são adequadas para clientes com acoplamento rígido aos quais o servidor tem acesso confiável e o cliente é endereçável por IP. No entanto, as notificações por push caíram em desuso desde o surgimento das notificações de streaming no Exchange 2010. Se possível, recomendamos que use as notificações de streaming em vez de notificações por push daqui para frente. As notificações por push exigem a criação de um aplicativo ouvinte, que é para onde as notificações são enviadas. Isso tem um pequeno benefício em relação às notificações por pull, pois reduz o tráfego de rede, mas adiciona sobrecarga ao exigir um aplicativo separado.  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>Quais eventos do EWS posso assinar?
<a name="bk_eventtypes"> </a>

Os tipos de eventos do EWS que os clientes assinam são definidos pela enumeração [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx) para a API Gerenciada do EWS ou o elemento [EventType](https://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx) do EWS. Os seguintes eventos do EWS estão disponíveis para assinatura: 
  
- NewMail – uma nova mensagem recebida na Caixa de Entrada.
    
- Excluído — uma mensagem foi excluída permanentemente da Caixa de Entrada. Para saber mais sobre as notificações de itens excluídos, confira [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md) e [Notificações por pull para eventos de caixa de correio relacionados à exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md).
    
- Modificado — um item ou pasta foi alterado.
    
- Movido — um item ou pasta foi movido. 
    
- Copiado — um item ou pasta foi copiado.
    
- Criado — um item ou pasta foi criado. 
    
- FreeBusyChanged – a informação de disponibilidade de um usuário foi alterada.
    
Outro tipo de evento do EWS, o evento Status, é definido pelo elemento [EventType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx), mas você não assina esse evento. Em vez disso, ele é enviado pelo servidor para verificar o status do cliente apenas para streaming e notificações por push. O cliente deve responder a este evento ou o cliente atingirá o tempo limite. 
  
Uma única ação do usuário geralmente resulta na criação de várias notificações. Para ilustrar isso, a figura a seguir mostra alguns cenários comuns e as notificações criadas para cada um deles. As configurações do cliente têm um impacto nas notificações recebidas, então essa não é uma lista completa de todas as opções de configuração e notificações resultantes.
  
**Figura 1. Tipos de eventos retornados por assinaturas de notificação**

![Uma tabela que mostra as notificações enviadas em situações comuns do usuários, como recebimento de novos emails, criação de uma nova pasta, movimentação de uma pasta e assim por diante.](media/Exchange2013_Notifications_Events.png)
  
A Figura 1 simplifica o processo de notificação. Na verdade, várias notificações (até mesmo diversas notificações do mesmo tipo) podem ser criadas para uma única ação do usuário. Por exemplo, no caso de uma operação de movimentação de pasta, são criados três eventos de pasta: um para a pasta sendo modificada, um para a pasta pai antiga e outro para a nova pasta pai. Como vários eventos podem ser disparados em uma única operação, recomendamos que você [compile o tempo de espera de alguns segundos em suas operações de sincronização](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices), de modo que só sincronize quando a ação for concluída, em vez de no meio da operação.
  
Também é importante observar que as definições de configuração que cada usuário escolhe afetarão as notificações criadas. Por exemplo, os dados de disponibilidade de alguns usuários são atualizados automaticamente e o evento FreeBusyChanged é criado quando uma nova solicitação de reunião é recebida, mesmo antes de ler o item. Para outros usuários, os dados de disponibilidade não são atualizados e o evento FreeBusyChanged não é criado até que a reunião seja aceita. Essas configurações podem ter um impacto considerável nas notificações criadas pelo servidor.
  
## <a name="how-do-ews-notifications-work"></a>Como funcionam as notificações do EWS?
<a name="bk_howwork"> </a>

As notificações do EWS são tratadas de acordo com a assinatura. Normalmente, há uma assinatura por caixa de correio e, na assinatura da caixa de correio, você pode assinar algumas ou todas as pastas. Você decide que tipo de notificação deseja assinar (streaming, pull ou push) e que tipo de eventos deseja receber (NewMail, Criado, Excluído, Modificado, etc.) e, em seguida, cria uma assinatura. Os eventos do EWS são então enviados de forma assíncrona do servidor de caixa de correio para o cliente. (Lição do histórico: os eventos são síncronos no Exchange 2007 - e os eventos são armazenados no servidor de Acesso para Cliente no Exchange 2010, mas não mais!).
  
Dependendo do tipo de assinatura que você possui, as formas como as notificações são enviadas ao cliente variam. Esta seção descreve como cada tipo de assinatura funciona com mais detalhes.
  
### <a name="ews-streaming-notifications"></a>Notificações de streaming do EWS
<a name="bk_streamnotif"> </a>

As notificações de streaming dependem de uma solicitação get deslocada no servidor para manter uma conexão de assinatura de streaming aberta, de modo que quaisquer eventos que ocorram enquanto a conexão estiver ativa sejam transmitidos ao cliente imediatamente. Várias notificações podem ser enviadas durante uma conexão simples, e a conexão permanece aberta até que o intervalo expire ou por, no máximo, 30 minutos. Após a conexão expirar, o cliente envia a solicitação get deslocada novamente. A Figura 2 mostra como as assinaturas de streaming e as notificações de streaming funcionam.
  
**Figura 2. Visão geral da notificação de streaming**

![Uma ilustração que mostra como as notificações de streaming funcionam. Para configurar notificações de streaming: 1. Assine, 2. Abra a conexão, 3. Espere por eventos, 4. Receba eventos, repita 3 e 4, 5. Feche ou mantenha a conexão, 6. Cancele a assinatura ou o tempo limite.](media/Exchange2013_Notifications_StreamSub.png)
  
Para saber mais sobre a criação de notificações de streaming, confira [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange.](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-pull-notifications"></a>Notificações por pull do EWS
<a name="bk_pullnotif"> </a>

As notificações por pull dependem do cliente solicitar as notificações em um intervalo gerenciado pelo cliente. Isso pode resultar em respostas GetEvents sem notificações. A Figura 3 mostra como as assinaturas pull e as notificações por pull funcionam.
  
**Figura 3. Visão geral da notificação por pull**

![Uma ilustração que mostra como as notificações por pull funcionam. Para configurar as notificações por pull: 1. Assine, 2. Envie GetEvents, 3. Receba resposta, repita 2 e 3, 4. Feche ou mantenha a conexão, 5. Cancele a assinatura ou o tempo limite.](media/Exchange2013_Notifications_PullSub.png)
  
Para saber mais sobre a criação de notificações por pull, confira [Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-push-notifications"></a>Notificações por push do EWS
<a name="bk_pushnotif"> </a>

As notificações por push contam com o servidor enviando notificações de volta ao cliente. Só há tráfego se houver uma notificação. A Figura 4 mostra como a assinatura push e as notificações por push funcionam.
  
**Figura 4. Visão geral da notificação por push**

![Uma ilustração que mostra como as notificações por push funcionam. Para configurar as notificações por push: 1. Crie o ouvinte, 2. Assine, 3. Aguarde eventos, 4. Receba eventos, 5. Envie resposta "OK", repita 3, 4 e 5, 6. Cancele a inscrição ou o tempo limite.](media/Exchange2013_Notifications_PushSub.png)

Se você estiver usando as [notificações por push com o Exchange 2010](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx), considere atualizar seu aplicativo para [usar notificações de streaming](https://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5), para que você não precise de um aplicativo separado para receber os eventos.

  
## <a name="how-do-i-subscribe-to-notifications"></a>Como assino as notificações?
<a name="bk_notifoperations"> </a>

Dependendo do tipo de assinatura que deseja criar, você tem várias opções de escolha para assinar as notificações.
  
**Tabela 2. Operações e métodos para assinar notificações**

|**Tipo de assinatura**|**Operação do EWS**|**Métodos da API Gerenciada do EWS**|**Função**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação de assinatura](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService.BeginSubscribeToStreamingNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BeginSubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToStreamingNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar as notificações de streaming.  <br/> |
|Efetuar pull  <br/> |[Operação de assinatura](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método ExchangeService.BeginSubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.BeginSubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> [Método ExchangeService.SubscribeToPullNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar as notificações por pull.  <br/> |
|Enviar por push  <br/> |[Operação de assinatura](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |[Método de sobrecarga ExchangeService.BeginSubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método de sobrecarga ExchangeService.BeginSubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> [Método de sobrecarga ExchangeService.SubscribeToPushNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> [Método de sobrecarga ExchangeService.SubscribeToPushNotificationsOnAllFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação para assinar as notificações por push.  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>Como obtenho os eventos do EWS?
<a name="bk_getevents"> </a>

Depois de criar a assinatura, a maneira como os eventos reais serão enviados ao cliente dependerá do tipo de assinatura. 
  
Para notificações de streaming, uma conexão de assinatura de streaming deve ser criada e, em seguida, a assinatura será adicionada à conexão. Você pode ler mais sobre esse processo em [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Para notificações por pull, o objeto de assinatura foi inicializado quando a assinatura foi criada, então você só precisa chamar o método ou operação **GetEvent** para recuperar os eventos do servidor. Você pode ler mais sobre isso em [Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
A tabela a seguir lista as operações e classes necessárias para recuperar eventos. 
  
**Tabela 3. Elementos e classes para criar uma conexão e obter eventos**

|**Tipo de assinatura**|**Operação do EWS**|**Método da API Gerenciada do EWS**|**Função**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação GetStreamingEvents](https://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |[Método StreamingSubscriptionConnection.AddSubscription method](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |Cria uma solicitação get deslocada no servidor, que é respondida quando os eventos ocorrem.  <br/> |
|Efetuar pull  <br/> |[Operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |[Método PullSubscription.GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |Obtém eventos de notificação por pull do servidor.  <br/> |
|Enviar por push  <br/> |Não aplicável.  <br/> |Não aplicável.  <br/> |As notificações por push são enviadas automaticamente ao ouvinte do serviço Web (a URL de retorno de chamada especificada na solicitação da assinatura). Não é necessário chamar nenhum outro método ou operação.  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>Como cancelo assinatura das notificações?
<a name="bk_notifunsubscribe"> </a>

A tabela a seguir lista as maneiras pelas quais você pode cancelar assinatura de cada tipo de assinatura.
  
**Tabela 4. Operações e métodos para cancelar assinatura das notificações**

|**Tipo de assinatura**|**EWS**|**API Gerenciada do EWS**||
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |[Operação de cancelamento de assinatura](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método StreamingSubscription.BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription.EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método StreamingSubscription.Unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Efetuar pull  <br/> |[Operação de cancelamento de assinatura](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |[Método PullSubscription.BeginUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription.EndUnsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> [Método PullSubscription.Unsubscribe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Enviar por push  <br/> |Retornar **Cancelar assinatura** no elemento [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) do [SendNotificationResponseMessage](https://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) <br/> |Não aplicável. Em vez disso, deixe a assinatura expirar.  <br/> ||
   
Como alternativa, você pode deixar cada uma das assinaturas expirar. 
  
**Tabela 5. Tempo limite da assinatura**

|**Tipo de assinatura**|**Valor de tempo limite no EWS**|**Valor de tempo limite na API Gerenciada do EWS**|**Tratamento de tempo limite**|
|:-----|:-----|:-----|:-----|
|Streaming  <br/> |Elemento [ConnectionTimeout](https://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx)  <br/> | Parâmetro de *tempo de vida* do construtor [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx)  <br/> |Para a API Gerenciada do EWS, depois que o valor de tempo limite expirar, o evento [OnDisconnect](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx) será gerado. Se o método [StreamingSubscriptionConnection.Open](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) não for chamado, a conexão será fechada.  <br/> Para o EWS, depois que o valor de tempo limite expira, a mensagem [GetUserConfigurationResponse](https://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) retorna um valor [ConnectionStatus](https://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) de fechado.  <br/> |
|Efetuar pull  <br/> |elemento [tempo limite](https://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx)  <br/> | parâmetro de *tempo limite* do método [SubscribeToPullNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  <br/> |Após o valor de tempo limite expirar, o servidor excluirá a assinatura.  <br/> |
|Enviar por push  <br/> |elemento [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)  <br/> | parâmetro de *frequência* do método [SubscribeToPushNotification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  <br/> |Se o servidor não receber uma resposta a uma notificação por push ou ping de status, ele tentará enviar a notificação várias vezes antes de interromper o envio. Para obter mais informações, confira [StatusFrequency](https://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx).  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>Posso limitar as assinaturas?
<a name="bk_limitsubs"> </a>

Em uma implantação local, você pode limitar o número de assinaturas por usuário com o [parâmetro de limitação EwsMaxSubscriptions](ews-throttling-in-exchange.md) da política de limitação. Essa política pode ser aplicada a todos os usuários ou apenas a usuários específicos. A política de limitação **EwsMaxSubscriptions** não é configurável para o Exchange Online. 
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_limitsubs"> </a>

- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Manipulação de erros relacionados a notificações no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
- [Referência de serviço Web do Exchange](../web-service-reference/web-services-reference-for-exchange.md)
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
- [Aplicativo de exemplo de notificações por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

