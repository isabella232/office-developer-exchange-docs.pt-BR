---
title: Instrumentação de solicitações de cliente para EWS e REST no Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Saiba mais sobre os cabeçalhos HTTP no EWS e as solicitações REST e respostas que podem ajudá-lo a monitorar e solucionar problemas do aplicativo Exchange.
ms.openlocfilehash: 3a8ce889ec7a6b9e70ec25a95ac248902f48ca6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456301"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Instrumentação de solicitações de cliente para EWS e REST no Exchange

Saiba mais sobre os cabeçalhos HTTP no EWS e as solicitações REST e respostas que podem ajudá-lo a monitorar e solucionar problemas do aplicativo Exchange.
  
Isso já aconteceu? Um usuário do seu aplicativo relata um erro inesperado. Você deseja investigar, mas não pode reproduzi-lo. O erro desapareceu para o usuário e você é deixado com poucos dados acionáveis. Frustrante, não é? Vamos ver como você pode se preparar proativamente para este cenário e, espero, evitar frustração no futuro.
  
## <a name="add-instrumentation-to-requests"></a>Adicionar instrumentação às solicitações

Recomendamos que você adicione outros cabeçalhos HTTP às suas solicitações para facilitar a solução de problemas. Você deve manter um registro dessas informações em algum lugar (por exemplo, em um arquivo de log) para que possa recuperá-lo posteriormente, se necessário. Isso é útil ao examinar o tráfego de rede e também é útil se você entrar em contato com o suporte da Microsoft para obter assistência.
  
**Tabela 1. Cabeçalhos de solicitação para solução de problemas**

|**Cabeçalho HTTP (EWS)**|**Equivalente à API gerenciada do EWS**|**Anotações**|
|:-----|:-----|:-----|
|Agente de usuário  <br/> |[ExchangeService. UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Defina isso como um valor exclusivo que identifique o aplicativo cliente.<br/><br/> Usar o mesmo valor para todas as solicitações que o seu aplicativo envia permite que a Microsoft ajude a solucionar problemas de falhas de chamada, caso ocorram.  <br/> |
|Client-Request-ID  <br/> |[ExchangeService. ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Defina isso como um valor exclusivo diferente para cada solicitação que seu aplicativo envia.<br/><br/> Recomendamos que você use um GUID. Esse identificador exclusivo deve ser usado para correlacionar atividades entre dois sistemas no caso de algo errado.  <br/> |
|retorno-Client-Request-ID  <br/> |[ExchangeService. ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Defina como **true** para sinalizar para o servidor Exchange que deve retornar o valor de seu Client-Request-ID na resposta correspondente.<br/><br/> Você pode usar isso para correlacionar solicitações e respostas em rastreamentos de rede ou rastreamentos de API gerenciada do EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService. SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Usado para [relatar latências de EWS](#bk_ReportLatency) para a Microsoft se seu aplicativo estiver acessando o Exchange Online ou o Exchange Online como parte do Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Informações de log de respostas

Assim que o cliente pode adicionar a instrumentação adicional às solicitações que envia, o Exchange adiciona instrumentação adicional às respostas na forma de cabeçalhos HTTP. O cliente deve capturar essas informações para acompanhar as informações de instrumentação de solicitação.
  
> [!NOTE]
> Se você estiver usando a API gerenciada do EWS, não haverá equivalente direto aos cabeçalhos HTTP. No entanto, todos os cabeçalhos de resposta HTTP podem ser acessados por meio da propriedade [ExchangeService. HttpResponseHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) . 
  
**Tabela 2. Cabeçalhos de resposta HTTP**

|**Cabeçalho HTTP**|**Descrição**|
|:-----|:-----|
|ID da solicitação  <br/> |Uma ID gerada pelo servidor para a solicitação que corresponde a essa resposta.  <br/> |
|Client-Request-ID  <br/> |O valor do cabeçalho Client-Request-ID na solicitação.<br/><br/> Este cabeçalho só estará presente se a solicitação contiver o cabeçalho Return-Client-Request-ID com um valor **true**.  <br/> |
|X-FEServer  <br/> |O FQDN do servidor de acesso para cliente que processou a solicitação.  <br/> |
|X-TargetBEServer  <br/> |O FQDN do servidor de caixa de correio que processou a solicitação.  <br/> |
|X-DiagInfo  <br/> |Informações adicionais de diagnóstico, dependendo da solicitação.  <br/> |
|x-MS-Diagnostics  <br/> | Esse cabeçalho só será aplicável se a autenticação OAuth for usada na solicitação.<br/><br/> Ele contém um código de erro explícito que especifica por que uma autenticação OAuth falhou.<br/><br/> Ele tem o seguinte formato:`errorId;reason="reason"error_type="error type"`<br/><br/> O campo de **motivo** é uma descrição legível do erro.<br/><br/> O campo **errorID** é um inteiro e o campo ** \_ tipo de erro** é a representação de cadeia de caracteres desse inteiro, da seguinte maneira:<ul><li>2 milhões: assinatura inválida \_</li><li>2000001: \_ token inválido</li><li>  2000002: token \_ expirado</li><li>2000003: \_ recurso inválido</li><li>2000004: \_ locatário inválido  </li><li>2000005: \_ usuário inválido</li><li>2000006: \_ cliente inválido</li><li>2000007: \_ erro interno</li><li>2000008: concessão inválida \_</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Relatar a latência do EWS para a Microsoft
<a name="bk_ReportLatency"> </a>

Se o aplicativo usar a API gerenciada do EWS ou o EWS para se conectar ao Exchange Online, você poderá relatar a latência em solicitações EWS diretamente à Microsoft. As informações são passadas pelo cabeçalho de solicitação X-ClientStatistics. Se você estiver usando a API gerenciada do EWS, tudo o que você precisa fazer é definir a propriedade [ExchangeService. SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) como **true**. Se você estiver usando o EWS, precisará medir o tempo entre a emissão de uma solicitação e o recebimento de uma resposta e, em seguida, adicione o cabeçalho X-ClientStatistics à próxima solicitação do EWS que seu aplicativo envia, usando o formato a seguir.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Mantemos relatórios para essas latências e os usam para melhorar continuamente os serviços do EWS no Exchange Online.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_ReportLatency"> </a>

Após ter adicionado a instrumentação do cliente ao seu aplicativo, você estará mais preparado se algo der errado. Se isso acontecer, você poderá usar seus dados de instrumentação para [solucionar problemas com o aplicativo](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md).
  
## <a name="see-also"></a>Confira também

- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
- [Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Ferramentas e recursos para a solução de problemas de aplicativos do EWS para Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

