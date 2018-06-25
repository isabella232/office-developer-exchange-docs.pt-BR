---
title: Instrumentação solicitações de clientes para o EWS e REST no Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Saiba mais sobre os cabeçalhos HTTP nas solicitações EWS e REST e respostas que podem ajudá-lo a monitorar e solucionar problemas de seu aplicativo do Exchange.
ms.openlocfilehash: bcf362952c29956729c44397043a56bf3603d0af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750852"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Instrumentação solicitações de clientes para o EWS e REST no Exchange

Saiba mais sobre os cabeçalhos HTTP nas solicitações EWS e REST e respostas que podem ajudá-lo a monitorar e solucionar problemas de seu aplicativo do Exchange.
  
Isso já aconteceu para você? Um usuário do seu aplicativo relata um erro inesperado. Você deseja investigar, mas você não pode reproduzi-lo. O erro desapareceu para o usuário e fica com muito pouco dados acionáveis. Frustrante, não é? Vejamos como você pode preparar proativamente para este cenário e esperamos evitar aborrecimento no futuro.
  
## <a name="add-instrumentation-to-requests"></a>Adicione instrumentação às solicitações

Recomendamos que você adicione os cabeçalhos HTTP adicionais às suas solicitações para facilitar a solução de problemas. Você deve manter um registro dessas informações em qualquer lugar (por exemplo, em um arquivo de log), para que possa recuperá-lo mais tarde se precisar. Isso é útil quando examinando o tráfego de rede e também é útil se você contatar o suporte da Microsoft para obter assistência.
  
**Tabela 1. Cabeçalhos de solicitação para solução de problemas**

|**Cabeçalho HTTP (EWS)**|**API gerenciada de EWS equivalente**|**Notes**|
|:-----|:-----|:-----|
|Agente do usuário  <br/> |[ExchangeService.UserAgent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Defina esta opção para um valor exclusivo que identifica o aplicativo cliente.<br/><br/> Usando o mesmo valor para todas as solicitações de seu aplicativo envia permite que a Microsoft ajudar a solucionar problemas de falhas de chamada, eles ocorrer.  <br/> |
|id de solicitação do cliente  <br/> |[ExchangeService.ClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Defina esta opção para um valor exclusivo diferente para cada solicitação que envia seu aplicativo.<br/><br/> Recomendamos que você use um GUID. Este identificador exclusivo é destinado a serem usadas para correlacionar atividades entre dois sistemas que algo saia errado.  <br/> |
|retorno-client-id de solicitação  <br/> |[ExchangeService.ReturnClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Defina como **true** para sinalizar para o servidor do Exchange que ele deve retornar o valor da sua id de cliente-solicitação na resposta correspondente.<br/><br/> Você pode usar esse para correlacionar solicitações e respostas de rastreamentos de rede ou rastreamentos de API gerenciada de EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Usado para [as latências EWS do relatório](#bk_ReportLatency) para a Microsoft se seu aplicativo estiver acessando o Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Informações de logs de respostas

Assim como seu cliente pode adicionar instrumentação adicionais às solicitações de que ele envia, Exchange adiciona instrumentação adicionais para as respostas no formato dos cabeçalhos HTTP. Seu cliente deve capturar essas informações para ir junto com as informações de instrumentação de solicitação.
  
> [!NOTE]
> Se você estiver usando a API gerenciada de EWS, não há nenhum equivalente direto para os cabeçalhos HTTP. No entanto, todos os cabeçalhos de resposta HTTP podem ser acessados por meio da propriedade [ExchangeService.HttpResponseHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) . 
  
**Tabela 2. Cabeçalhos de resposta HTTP**

|**Cabeçalho HTTP**|**Descrição**|
|:-----|:-----|
|id de solicitação  <br/> |Uma ID para a solicitação que corresponde a essa resposta gerados pelo servidor.  <br/> |
|id de solicitação do cliente  <br/> |O valor do cabeçalho na solicitação de id de solicitação do cliente.<br/><br/> Este cabeçalho só estará presente se a solicitação contém o cabeçalho de retorno-client-id de solicitação com um valor **true**.  <br/> |
|X-FEServer  <br/> |O FQDN do servidor acesso para cliente que processaram a solicitação.  <br/> |
|X-TargetBEServer  <br/> |O FQDN do servidor de caixa de correio que processaram a solicitação.  <br/> |
|X-DiagInfo  <br/> |Informações de diagnósticos adicionais, dependendo da solicitação.  <br/> |
|x-ms-diagnostics  <br/> | Este cabeçalho é aplicável somente se a autenticação OAuth é usada na solicitação.<br/><br/> Ele contém um código de erro explícita que especifica por que uma autenticação OAuth falhou.<br/><br/> Ele usa o seguinte formato:`errorId;reason="reason"error_type="error type"`<br/><br/> O campo **motivo** é uma legíveis descrição do erro.<br/><br/> O campo **identificação de erro** é um inteiro e o **erro\_tipo** campo é a representação de cadeia de caracteres desse número inteiro, da seguinte maneira:<ul><li>2000000: inválido\_assinatura</li><li>2000001: inválido\_token</li><li>  2000002: token\_expirou</li><li>2000003: inválido\_recurso</li><li>2000004: inválido\_locatário  </li><li>2000005: inválido\_usuário</li><li>2000006: inválido\_cliente</li><li>2000007: interno\_erro</li><li>2000008: inválido\_conceder</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Latência do EWS de relatório para a Microsoft
<a name="bk_ReportLatency"> </a>

Se seu aplicativo usa a API gerenciada de EWS ou o EWS para se conectar ao Exchange Online, é possível denunciar a latência em solicitações EWS diretamente à Microsoft. As informações são passadas por meio do cabeçalho de solicitação X-ClientStatistics. Se você estiver usando a API gerenciada de EWS, tudo o que você deve fazer é definir a propriedade [ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) como **true**. Se você estiver usando o EWS, você precisará medir o tempo entre emitindo uma solicitação e recebimento de uma resposta, em seguida, adicione o cabeçalho X-ClientStatistics para a próxima solicitação EWS envia seu aplicativo, usando o seguinte formato.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Podemos manter relatórios para esses latências e usá-los para melhorar continuamente os serviços do EWS no Exchange Online.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_ReportLatency"> </a>

Depois que você adicionou instrumentação de cliente para seu aplicativo, você está preparado melhor caso algo saia errado. Se isso ocorrer, você pode usar os dados de instrumentação para [Solucionar problemas de seu aplicativo](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md).
  
## <a name="see-also"></a>Confira também

- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
- [Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Ferramentas e recursos para solucionar problemas de aplicativos do EWS do Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

