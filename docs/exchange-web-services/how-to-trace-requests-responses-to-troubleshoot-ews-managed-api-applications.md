---
title: Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 186c1d1d-b8dc-4914-b3cd-6fada7ecd877
description: Descubra como rastrear solicitações e respostas do EWS para solucionar erros no seu aplicativo de API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: dd225030d62a2e8211b7063ee78a59fd1a070263
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455853"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a>Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS

Descubra como rastrear solicitações e respostas do EWS para solucionar erros no seu aplicativo de API gerenciada do EWS.
  
A depuração de um aplicativo baseado em serviço Web pode ser difícil porque parte do processamento é executada em um computador remoto que você pode não ter acesso. Como não é possível percorrer o código no servidor, pode ser útil ver as solicitações e respostas XML enviadas entre o cliente e o servidor para determinar qual parte do aplicativo está causando um erro. 
  
Se você estiver usando o EWS, você já tem acesso à solicitação e resposta XML; Você pode colocar um ponto de interrupção no seu código para revisar a resposta do servidor à sua solicitação, a fim de solucionar um problema. Se você estiver usando a API gerenciada do EWS, não terá acesso direto à solicitação e à resposta do EWS. No entanto, você pode usar os métodos de rastreamento no objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para capturar a solicitação e a resposta XML e, em seguida, pode usar o XML para determinar por que seu código não está funcionando. 

Por exemplo, se você não definiu uma propriedade corretamente, você pode receber uma resposta inesperada, e você pode usar a saída de rastreamento para examinar a solicitação e resposta XML para identificar o erro. A saída de rastreamento da API gerenciada do EWS também pode ajudá-lo a criar manualmente a solicitação XML para criar seu aplicativo do EWS. Se você estiver usando o EWS, é possível criar um pequeno aplicativo usando a API gerenciada do EWS, rastreá-lo e usar as informações de solicitação XML para ajudá-lo a criar sua solicitação do EWS. 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a>Habilitando o rastreamento no objeto ExchangeService
<a name="bk_EnableTracing"> </a>

Para habilitar o rastreamento, crie um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para o seu aplicativo e defina as propriedades de rastreamento, conforme mostrado no exemplo a seguir. 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

Depois de definir a propriedade [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true**, todas as solicitações que correspondam aos sinalizadores de rastreamento serão enviadas para o ouvinte de rastreamento especificado. Você pode especificar um único sinalizador de rastreamento ou pode especificar vários sinalizadores de rastreamento combinando-os com um **or**lógico. Você pode usar a [Enumeração TraceFlags](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) para especificar valores para EWS e para solicitações e respostas de descoberta automática. 
  
## <a name="implementing-a-tracelistener-object"></a>Implementar um objeto TraceListener
<a name="bk_traceListener"> </a>

Você pode definir a propriedade [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true** para gerar as solicitações e respostas XML para seu aplicativo, como uma janela do console. Se você quiser controlar a saída de rastreamento e salvá-la em um arquivo, recomendamos que você implemente um objeto de [classe TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) . O exemplo de código a seguir mostra um objeto simples que implementa a interface [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) e armazena as solicitações e respostas rastreadas em XML ou arquivos de texto. 
  
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

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)    
- [Fazer referência ao assembly da API gerenciada do EWS](how-to-reference-the-ews-managed-api-assembly.md)    
- [Comunicar-se com o EWS usando a API gerenciada do EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

