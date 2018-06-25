---
title: Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Saiba mais sobre como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.
ms.openlocfilehash: 7cfbfb5cc19e092c37e3d48a7fcc4f27023516e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750740"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange

Saiba mais sobre como manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio.
  
Afinidade é a associação de uma sequência de mensagens de solicitação e resposta com um determinado servidor de caixa de correio. Para a maioria das funcionalidades no Exchange, afinidade é manipulada pelo servidor. Notificações, no entanto, são uma exceção. O cliente é responsável por manter a afinidade com o servidor de caixa de correio para inscrições de notificação. Este afinidade permite que o balanceador de carga e servidores de acesso para cliente entre o cliente e o servidor de inscrições de notificação de rota e relacionadas solicitações para o servidor de caixa de correio que mantém a assinatura. Sem afinidade, a solicitação pode ser roteada para um servidor de caixa de correio diferente que não inclui as inscrições do cliente, que podem causar um erro de [ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) a ser retornado. 
  
## <a name="how-is-affinity-maintained"></a>Como a afinidade é mantida?
<a name="bk_howmaintained"> </a>

Afinidade no Exchange é baseadas em cookies. O cliente dispara a criação do cookie, incluindo cabeçalhos específicos na solicitação de assinatura e, em seguida, a resposta de assinatura conterá o cookie. O cliente envia esse cookie nas solicitações subsequentes para garantir que a solicitação é roteada para o servidor de caixa de correio à direita.
  
Mais especificamente, a afinidade no Exchange é tratada pelo seguinte: 
  
- X-AnchorMailbox — Um cabeçalho HTTP, que está incluído na solicitação de assinatura inicial. Identifica a primeira caixa de correio em um grupo de caixas de correio que compartilham a afinidade com o mesmo servidor de caixa de correio.
    
- X-PreferServerAffinity — Um cabeçalho HTTP que está incluído na solicitação de assinatura inicial com o cabeçalho X-AnchorMailbox e estiver definido como true para indicar que o cliente está solicitando que afinidade ser mantidas com o servidor de caixa de correio.
    
- X-BackEndOverrideCookie — Um cookie que está incluído na resposta assinatura inicial e contém um cookie que o balanceador de carga e o servidor de acesso para cliente usam para rotear solicitações subsequentes no mesmo servidor de caixa de correio.
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>Como manter a afinidade usando a API gerenciada de EWS ou EWS?
<a name="bk_howdoimaintain"> </a>

Você pode usar as mesmas etapas para manter a afinidade para diversas assinaturas de caixa de correio e de seus servidores de caixa de correio, não importa se você estiver usando o streaming, pull ou notificações de push, e independentemente se você está direcionando do Exchange no servidor local ou Exchange Online.
  
1. Para cada caixa de correio, [descoberta automática de chamadas](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e obtenha as configurações de usuário GroupingInformation e ExternalEwsUrl. Para descoberta automática do SOAP, você usar o elemento de [configuração](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) e de descoberta automática POX, você usar o elemento [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) . 
    
2. Usando as configurações de GroupingInformation e ExternalEwsUrl entre as respostas de descoberta automática, caixas de correio local com o mesmo ExternalEwsUrl e GroupingInformation concatenado valor no mesmo grupo. Se nenhum grupo tiver mais de 200 caixas de correio, se dividem os grupos de modo que cada grupo tenha não mais de 200 caixas de correio.
    
3. Criar e usar um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) para o restante do procedimento. Quando você usa o mesmo objeto **ExchangeService** , cookies e os cabeçalhos (quando eles estão definidos) são mantidos automaticamente. Observe que, se você não pretende inscrições de streaming de grupo em uma única conexão, você está livre para criar um objeto **ExchangeService** diferente para cada usuário representado. 
    
4. [Enviar uma assinatura de](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) solicitação para o usuário cujo nome de usuário aparece primeiro quando todos os usuários no grupo são classificados em ordem alfabética (vamos nos referir a esse usuário como o usuário de caixa de correio âncora). Faça o seguinte: 
    
  - Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário da caixa de correio âncora.
    
  - Inclua o cabeçalho X-PreferServerAffinity com um conjunto de valor como true.
    
  - Use a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (o tipo de [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
5. Em resposta a assinatura, obtenha o valor X-BackEndOverrideCookie. Inclua esse valor em cada uma das solicitações subsequentes de assinatura para os usuários deste grupo.
    
6. Para cada usuário adicional no grupo, enviar uma solicitação de assinatura e faça o seguinte:
    
  - Inclua o cabeçalho X-AnchorMailbox com um valor definido para o endereço SMTP do usuário âncora da caixa de correio para o grupo.
    
  - Inclua o cabeçalho X-PreferServerAffinity com um conjunto de valor como true.
    
  - Inclua o X-BackEndOverrideCookie foi retornado em resposta de assinatura do usuário de caixa de correio a âncora.
    
  - Use a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (o tipo de [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
    Observe que o servidor usará os valores de X-PreferServerAffinity e X-BackendOverrideCookie juntos para executar o roteamento para o servidor de caixa de correio. O cabeçalho X-AnchorMailbox também é necessário, mas é ignorado pelo servidor se os dois valores são válidos. Se X-AnchorMailbox e X-PreferServerAffinity estão em uma solicitação e X-BackendOverrideCookie não for incluído, o valor X-AnchorMailbox é usado para rotear solicitações.
    
    Como o X-PreferServerAffinity e os valores de X-BackendOverrideCookie executam o roteamento, se a caixa de correio âncora nunca mover para outro servidor ou um grupo, a lógica não altera porque o X-BackendOverrideCookie roteará a solicitação ao servidor correto para o grupo.
    
7. Enviar solicitações de [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) ou de um único [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) para o grupo e faça o seguinte: 
    
  - Inclua os valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) retornados em cada uma das respostas a inscrição individual para caixas de correio no grupo. 
    
  - Se mais de 200 assinaturas existirem para o grupo, criem várias solicitações. O número máximo de valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) a serem incluídos em uma solicitação é 200. 
    
  - Se você precisar de mais conexões que estão disponíveis para a caixa de correio de destino, use a conta de serviço para representar a caixa de correio para o grupo; âncora Caso contrário, não use a representação. O ideal é que você deseja representar uma caixa de correio exclusiva por solicitação [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) para que você nunca encontrar os limites de limitação. 
    
  - Use ApplicationImpersonation se precisar de [mais conexões que estão disponíveis para a caixa de correio de destino](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); Caso contrário, não use ApplicationImpersonation.
    
  - Incluir o cabeçalho X-PreferServerAffinity e defina-o como true. Esse valor é incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2. 
    
  - Inclua o X-BackEndOverrideCookie para o grupo (o X-BackEndOverrideCookie retornado na resposta de assinatura do usuário da caixa de correio âncora). Esse valor é incluído automaticamente se você estiver usando o objeto **ExchangeService** que você criou na etapa 2. 
    
8. Passe os eventos retornados para um thread separado para processamento.
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>Os valores de limitação para os quais é necessário levar em consideração?
<a name="bk_throttling"> </a>

Ao planejar a implementação de notificação, você vai querer leve em consideração as dois valores: o número de conexões e o número de assinaturas. A tabela a seguir lista os valores padrão para cada configuração de [limitação](ews-throttling-in-exchange.md) e como as configurações são usadas. Para cada valor, o orçamento é alocado para a caixa de correio de destino. Por esse motivo, usando a representação para obter conexões adicionais é uma etapa necessária em muitos cenários. 
  
**Tabela 1. Limitação de valores padrão**

|**Área de consideração**|**Configuração de limitação**|**Default value**|**Descrição**|
|:-----|:-----|:-----|:-----|
|Conexões de streaming  <br/> |Padrão deslocado limite de conexão  <br/> |10 para Exchange Online  <br/> 3 para Exchange 2013  <br/> |O número máximo de conexões simultâneas de streaming que uma conta pode ter abertos no servidor ao mesmo tempo. Para trabalhar nesse limite, use uma conta de serviço com a função ApplicationImpersonation atribuída para as caixas de correio de destino e representar o primeiro usuário em cada grupo de ID de assinatura quando obtendo transmitidas eventos.  <br/> |
|Conexões de recepção ou de envio  <br/> |EWSMaxConcurrency  <br/> |27  <br/> |O número máximo de conexões simultâneas de recepção ou de envio (solicitações que foram recebidas, mas ainda não respondidas) que uma conta pode ter abertas no servidor ao mesmo tempo.  <br/> |
|Assinaturas  <br/> |EWSMaxSubscriptions  <br/> |20 para o Exchange Online  <br/> 5000 para o Exchange 2013  <br/> |O número máximo de inscrições nonexpired que uma conta pode ter ao mesmo tempo. Esse valor é diminuído quando a assinatura é criada no servidor.  <br/> |
   
O exemplo a seguir mostra como os orçamentos são manipulados entre qualquer caixa de correio de destino e a conta de serviço que possui a função [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) atribuída para as caixas de correio de destino. 
  
- ServiceAccount1 (sa1) personifica muitos usuários (m1, m2, m3 e assim por diante) e cria assinaturas para cada caixa de correio. Observe que, quando as assinaturas são criadas, o proprietário da assinatura é sa1, portanto, quando sa1 abre uma conexão com as assinaturas, EWS impõe que as assinaturas pertencentes sa1.
    
- Sa1 pode abrir a conexão das seguintes maneiras:
    
1. Sem representação, portanto a conexão é cobrado contra sa1.
    
2. Ao representar qualquer um dos usuários — m1, por exemplo — para que a conexão é cobrado contra uma cópia do orçamento do m1. (M1 próprio pode abrir dez conexões usando o Exchange Online e todas as contas de serviço as representação m1 podem abrir dez conexões usando o orçamento copiado.)
    
- Se for atingido o limite de conexão, as seguintes soluções alternativas estão disponíveis:
    
  - Se a opção 1 é usada, o administrador pode criar várias contas de serviço para representar usuários adicionais.
    
  - Se a opção 2 é usada, o código pode representar outro usuário — m2 por exemplo.
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>Exemplo: Mantendo afinidade entre um grupo de assinaturas e o servidor de caixa de correio
<a name="bk_ce"> </a>

Okey, vamos vê-lo em ação. O exemplo de código a seguir mostra como agrupar usuários e usar os cabeçalhos X-AnchorMailbox e PreferServerAffinity-X e o cookie de X-BackendOverrideCookie para manter a afinidade com o servidor de caixa de correio. Como os cabeçalhos e o cookie são de importância principal no bloco afinidade, este exemplo enfoca as EWS XML solicitações e respostas. Para usar a API gerenciada de EWS para criar o corpo das solicitações de inscrição e respostas, consulte [notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) e [receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). Esta seção inclui etapas adicionais que sejam específicos para manutenção afinidade e adicionando os cabeçalhos às suas solicitações.
  
Este exemplo tem quatro usuários: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com e sadie@contoso.com. A figura a seguir mostra os GroupingInformation e ExternalEwsUrl [configurações de descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) para os usuários. 
  
**Figura 1. Usado para caixas de correio do grupo de definições de descoberta automática**

![A table that shows the GroupingInformation and ExternalEwsUrl values for each of the users.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
Usando as configurações das respostas de descoberta automática, as caixas de correio são agrupadas pelo valor concatenado das configurações de GroupingInformation e ExternalEwsUrl. Neste exemplo, Alfredo e Sadie tem os mesmos valores, para que eles estão em um grupo e Alisa e Ronnie compartilham os mesmos valores, portanto, eles estão em outro grupo.
  
**Figura 2. Criação de grupos de caixa de correio**

![A table that shows how mailbox groups are created using Autodiscover settings.](media/Exchange2013_NotificationAffinityGrouping.png)
  
Neste exemplo, para fins de focaremos na grupo. Podemos seria usar as mesmas etapas para o grupo B, mas use um valor diferente de X-AnchorMailbox para esse grupo.
  
Usando [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx), crie a solicitação de inscrição para a caixa de correio âncora (alfred@contoso.com), com o cabeçalho X-AnchorMailbox definido como o seu endereço de email e um valor de cabeçalho X-PreferServerAffinity verdadeiro. Configurar esses valores de dois cabeçalho irá disparar o servidor para criar um X-BackEndOverrideCookie para a resposta.
  
Se você estiver usando o EWS Managed API, use o método[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e) de [HttpHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)para adicionar os dois cabeçalhos à sua solicitação de assinatura, como mostrado. 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

Portanto solicitação de assinatura de Alfredo tem esta aparência.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

A seguinte mensagem XML é a resposta à solicitação de assinatura de Alfredo e inclui o X-BackEndOverrideCookie. Reenvie esse cookie para todas as solicitações subsequentes para os usuários deste grupo. Observe que a resposta também contém cookies adicionais, como o cookie exchangecookie usados pelo Exchange 2010. O Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013, ignorar exchangecookie se ela estiver incluída nas solicitações de inscrição subsequentes.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

Usando o X-BackEndOverrideCookie da resposta de Alfredo e cabeçalho X-AnchorMailbox, a solicitação de assinatura é criada para Sadie, o outro membro da solicitação de assinatura do grupo A. Sadie tem esta aparência.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@consoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@consoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

Resposta de assinatura de Sadie tem esta aparência. Observe que ele não inclui o X-BackEndOverrideCookie. O cliente é responsável para armazenar em cache o valor em solicitações futuras.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

Usando os valores de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) entre as respostas de inscrição, uma solicitação de operação [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) foi criada para todas as assinaturas no grupo. Como há menos de 200 assinaturas nesse grupo, eles são todos enviados em uma solicitação. O cabeçalho X-PreferServerAffinity estiver definido como true e o X-BackEndOverrideCookie está incluído. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

Os eventos retornados serão então passados a um segmento separado para processamento.
  
## <a name="how-has-affinity-changed"></a>Como a afinidade mudou?
<a name="bk_howchanged"> </a>

No Exchange 2010, as assinaturas são mantidas no servidor de acesso para cliente, conforme mostrado na Figura 3. Nas versões do Exchange mais recente do que o Exchange 2010, as assinaturas são mantidas no servidor de caixa de correio, conforme mostrado na Figura 4.
  
**Figura 3. Processo para manter a afinidade no Exchange 2010**

![An illustration that shows how the table of active subscriptions is maintained on the Client Access server in Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
**Figura 4. Processo para manter a afinidade no Exchange Online e Exchange 2013**

![An illustration that shows how the load balancer and the Client Access server route requests to the mailbox server that maintains the table of active subscriptions in Exchange Server and Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
No Exchange 2010, o cliente só sabe o endereço do balanceador de carga e o exchangecookie que é retornado pelo servidor garante que a solicitação é roteada para o servidor de acesso para cliente à direita. No entanto, em versões posteriores, o balanceador de carga e as funções de servidor acesso para cliente ter que rotear solicitações apropriadamente que eles cheguem ao servidor de caixa de correio. Para fazer o que, forem necessárias informações adicionais, que é o motivo pelo qual os novos cabeçalhos e cookie introduzidas. O artigo [inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explica como as assinaturas são mantidas no Exchange 2013. 
  
Você pode observar que o exchangecookie que usa o Exchange 2010 ainda será retornada por versões posteriores. Não há nenhuma danos esse cookie, incluindo solicitações de, mas as versões anteriores do Exchange ignorá-la.
  
## <a name="see-also"></a>Confira também

- [Inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
- [Alterações no gerenciamento de afinidade de assinaturas do EWS...](http://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [EWS limitação no Exchange](ews-throttling-in-exchange.md)
    

