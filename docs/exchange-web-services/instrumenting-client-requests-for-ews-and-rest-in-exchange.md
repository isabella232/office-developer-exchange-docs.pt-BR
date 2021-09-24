---
title: Instrumentando solicitações de cliente para EWS e REST Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Saiba mais sobre os cabeçalhos HTTP em solicitações e respostas REST e EWS que podem ajudá-lo a monitorar e solucionar problemas de seu Exchange aplicativo.
ms.openlocfilehash: f32a164436a1f8ab06192e71a287f5092fe9a6c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520987"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Instrumentando solicitações de cliente para EWS e REST Exchange

Saiba mais sobre os cabeçalhos HTTP em solicitações e respostas REST e EWS que podem ajudá-lo a monitorar e solucionar problemas de seu Exchange aplicativo.
  
Isso já aconteceu com você? Um usuário do aplicativo relata um erro inesperado. Você deseja investigar, mas não pode reproduzi-lo. O erro desapareceu para o usuário e você é deixado com muito pouco dados a ação. Frustrante, não é? Vamos ver como você pode se preparar proativamente para esse cenário e, com sorte, evitar frustração no futuro.
  
## <a name="add-instrumentation-to-requests"></a>Adicionar instrumentação a solicitações

Recomendamos adicionar cabeçalhos HTTP adicionais às suas solicitações para facilitar a solução de problemas. Você deve manter um registro dessas informações em algum lugar (por exemplo, em um arquivo de log) para que possa recuperá-las mais tarde, se precisar. Isso é útil ao examinar o tráfego de rede e também é útil se você contatar o suporte da Microsoft para assistência.
  
**Tabela 1. Solicitar headers para solução de problemas**

|**Cabeçalho HTTP (EWS)**|**Equivalente à API Gerenciada do EWS**|**Observações**|
|:-----|:-----|:-----|
|User-Agent  <br/> |[ExchangeService.UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |De definir isso como um valor exclusivo que identifique seu aplicativo cliente.<br/><br/> Usar o mesmo valor para todas as solicitações que seu aplicativo envia permite que a Microsoft ajude a solucionar falhas de chamada, caso elas surjam.  <br/> |
|client-request-id  <br/> |[ExchangeService.ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |De definir isso como um valor exclusivo diferente para cada solicitação que seu aplicativo envia.<br/><br/> Recomendamos que você use um GUID. Esse identificador exclusivo destina-se a ser usado para correlacionar atividades entre dois sistemas no caso de algo dar errado.  <br/> |
|return-client-request-id  <br/> |[ExchangeService.ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Dejuste isso **como true** para sinalizar para o servidor Exchange que ele deve retornar o valor do seu cliente-request-id na resposta correspondente.<br/><br/> Você pode usar isso para correlacionar solicitações e respostas em rastreamentos de rede ou rastreamentos de API gerenciada do EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Usado para [relatar latências do EWS](#bk_ReportLatency) à Microsoft se seu aplicativo estiver acessando Exchange Online ou Exchange Online como parte do Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Informações de log de respostas

Assim como seu cliente pode adicionar instrumentação adicional às solicitações que envia, Exchange adiciona instrumentação adicional às respostas na forma de cabeçalhos HTTP. Seu cliente deve capturar essas informações para acompanhar as informações de instrumentação de solicitação.
  
> [!NOTE]
> Se você estiver usando a API Gerenciada do EWS, não há equivalente direto para os cabeçalhos HTTP. No entanto, todos os cabeçalhos de resposta HTTP podem ser acessados por meio da [propriedade ExchangeService.HttpResponseHeaders.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) 
  
**Tabela 2. Cabeçalhos de resposta HTTP**

|**Cabeçalho HTTP**|**Descrição**|
|:-----|:-----|
|request-id  <br/> |Uma ID gerada pelo servidor para a solicitação que corresponde a essa resposta.  <br/> |
|client-request-id  <br/> |O valor do header client-request-id na solicitação.<br/><br/> Esse header só estará presente se a solicitação contiver o header return-client-request-id com um valor **true**.  <br/> |
|X-FEServer  <br/> |O FQDN do servidor de Acesso para Cliente que processou a solicitação.  <br/> |
|X-TargetBEServer  <br/> |O FQDN do servidor de caixa de correio que processou a solicitação.  <br/> |
|X-DiagInfo  <br/> |Informações de diagnóstico adicionais, dependendo da solicitação.  <br/> |
|x-ms-diagnostics  <br/> | Esse header só será aplicável se a autenticação OAuth for usada na solicitação.<br/><br/> Ele contém um código de erro explícito que especifica por que uma autenticação OAuth falhou.<br/><br/> Ele tem o seguinte formato: `errorId;reason="reason"error_type="error type"`<br/><br/> O **campo** motivo é uma descrição aceitável para humanos do erro.<br/><br/> O **campo errorId** é um inteiro e o campo de tipo **\_ de** erro é a representação de cadeia de caracteres desse inteiro, da seguinte forma:<ul><li>2000000: assinatura \_ inválida</li><li>2000001: \_ token inválido</li><li>  2000002: o token \_ expirou</li><li>2000003: recurso \_ inválido</li><li>2000004: \_ locatário inválido  </li><li>2000005: usuário \_ inválido</li><li>2000006: cliente \_ inválido</li><li>2000007: erro \_ interno</li><li>2000008: \_ concessão inválida</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Relatar latência do EWS para a Microsoft
<a name="bk_ReportLatency"> </a>

Se seu aplicativo usa a API Gerenciada do EWS ou o EWS para se conectar ao Exchange Online, você pode relatar latência em solicitações do EWS diretamente para a Microsoft. As informações são passadas por meio do header de solicitação X-ClientStatistics. Se você estiver usando a API Gerenciada do EWS, tudo o que você precisa fazer é definir a [propriedade ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) como **true**. Se você estiver usando o EWS, precisará medir o tempo entre a emissão de uma solicitação e o recebimento de uma resposta, em seguida, adicione o header X-ClientStatistics à próxima solicitação do EWS que seu aplicativo enviar, usando o seguinte formato.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Mantemos relatórios para essas latências e os usamos para melhorar continuamente os serviços EWS Exchange Online.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_ReportLatency"> </a>

Depois de adicionar instrumentação de cliente ao aplicativo, você está mais preparado se algo der errado. Se isso acontecer, você poderá usar seus dados de instrumentação para solucionar [problemas com seu aplicativo.](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
  
## <a name="see-also"></a>Confira também

- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
- [Rastrear solicitações e respostas para solucionar problemas de aplicativos da API Gerenciada do EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Ferramentas e recursos para solucionar problemas de aplicativos EWS para Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

