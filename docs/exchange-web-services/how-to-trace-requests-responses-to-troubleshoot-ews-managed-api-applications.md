---
title: Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Descubra como EWS solicitações e respostas para solucionar erros no seu aplicativo do EWS Managed API de rastreamento.
ms.openlocfilehash: 056a1f84c4172b0404975d6fc35f9ecd7395ecdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750825"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento

Descubra como EWS solicitações e respostas para solucionar erros no seu aplicativo do EWS Managed API de rastreamento.
  
Depurar um aplicativo baseado no serviço da web pode ser difícil porque está sendo executada em um computador remoto que talvez você não tenha acesso à parte do processamento. Porque você não pode percorrer o código no servidor, ele pode ser útil ver as solicitações XML e respostas enviadas entre o cliente e o servidor para determinar qual parte do aplicativo está causando um erro. 
  
Se você estiver usando o EWS, você já tem acesso à solicitação XML e resposta; Você pode colocar um ponto de interrupção em seu código para analisar a resposta do servidor à sua solicitação para solucionar um problema. Se você estiver usando a API gerenciada de EWS, você não tem acesso direto para a solicitação do EWS e a resposta. No entanto, você pode usar os métodos de rastreamento no objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para capturar a solicitação XML e a resposta e, em seguida, você pode usar o XML para determinar porque seu código não está funcionando. 

Por exemplo, se você não definir uma propriedade corretamente, você pode receber uma resposta inesperada e você pode usar a saída de rastreamento para examinar a solicitação XML e a resposta para identificar o erro. A saída do rastreamento da API gerenciada do EWS pode ajudá-lo a criar manualmente a solicitação XML para criar o seu aplicativo do EWS. Se você estiver usando o EWS, você pode criar um aplicativo pequeno usando o EWS Managed API, rastreá-lo e, em seguida, use as informações de solicitação XML para ajudar a construir sua solicitação EWS. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>A habilitação do rastreamento no objeto ExchangeService
<a name="bk_EnableTracing"> </a>

Para habilitar o rastreamento, crie um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para seu aplicativo e definir as propriedades de rastreamento, conforme mostrado no exemplo a seguir. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

Depois de definir a propriedade [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true**, todas as solicitações que coincidem com os sinalizadores de rastreamento serão enviadas ao ouvinte de rastreamento especificado. Você pode especificar um sinalizador de rastreamento único, ou você pode especificar vários sinalizadores de rastreamento, combinando-os com uma lógica **OR**. Você pode usar a [enumeração TraceFlags](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) para especificar valores para o EWS e respostas e solicitações de descoberta automática. 
  
## <a name="implementing-a-tracelistener-object"></a>Implementação de um objeto TraceListener
<a name="bk_traceListener"> </a>

Você pode definir a propriedade [TraceEnabled](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true** para as solicitações XML e respostas para seu aplicativo, como uma janela do console de saída. Se você quiser controlar a saída de rastreamento e salvá-lo em um arquivo, recomendamos que você implemente um objeto de [classe TraceListener](http://msdn.microsoft.com/en-us/library/system.diagnostics.tracelistener.aspx) . O exemplo de código a seguir mostra um objeto simple que implementa a interface [ITraceListener](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) e armazena as rastreados solicitações e respostas em arquivos XML ou de texto. 
  
```cs
class TraceListener : ITraceListener
{
    #region ITraceListener Members
    public void Trace(string traceType, string traceMessage)
    {
      CreateXMLTextFile(traceType, traceMessage.ToString());
    }
    #endregion
    private void CreateXMLTextFile(string fileName, string traceContent)
    {
      // Create a new XML file for the trace information.
      try
      {
        // If the trace data is valid XML, create an XmlDocument object and save.
        XmlDocument xmlDoc = new XmlDocument();
        xmlDoc.Load(traceContent);
        xmlDoc.Save(fileName + ".xml");
      }
      catch
      {
        // If the trace data is not valid XML, save it as a text document.
        System.IO.File.WriteAllText(fileName + ".txt", traceContent);
      }
    }
}

```

## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)    
- [Faça referência ao conjunto de API gerenciada de EWS](how-to-reference-the-ews-managed-api-assembly.md)    
- [Comunicar-se com o EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

