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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455853"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="bc907-103">Rastrear solicitações e respostas para solucionar problemas de aplicativos de API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="bc907-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="bc907-104">Descubra como rastrear solicitações e respostas do EWS para solucionar erros no seu aplicativo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="bc907-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="bc907-105">A depuração de um aplicativo baseado em serviço Web pode ser difícil porque parte do processamento é executada em um computador remoto que você pode não ter acesso.</span><span class="sxs-lookup"><span data-stu-id="bc907-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="bc907-106">Como não é possível percorrer o código no servidor, pode ser útil ver as solicitações e respostas XML enviadas entre o cliente e o servidor para determinar qual parte do aplicativo está causando um erro.</span><span class="sxs-lookup"><span data-stu-id="bc907-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="bc907-107">Se você estiver usando o EWS, você já tem acesso à solicitação e resposta XML; Você pode colocar um ponto de interrupção no seu código para revisar a resposta do servidor à sua solicitação, a fim de solucionar um problema.</span><span class="sxs-lookup"><span data-stu-id="bc907-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="bc907-108">Se você estiver usando a API gerenciada do EWS, não terá acesso direto à solicitação e à resposta do EWS.</span><span class="sxs-lookup"><span data-stu-id="bc907-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="bc907-109">No entanto, você pode usar os métodos de rastreamento no objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para capturar a solicitação e a resposta XML e, em seguida, pode usar o XML para determinar por que seu código não está funcionando.</span><span class="sxs-lookup"><span data-stu-id="bc907-109">However, you can use tracing methods on the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="bc907-110">Por exemplo, se você não definiu uma propriedade corretamente, você pode receber uma resposta inesperada, e você pode usar a saída de rastreamento para examinar a solicitação e resposta XML para identificar o erro.</span><span class="sxs-lookup"><span data-stu-id="bc907-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="bc907-111">A saída de rastreamento da API gerenciada do EWS também pode ajudá-lo a criar manualmente a solicitação XML para criar seu aplicativo do EWS.</span><span class="sxs-lookup"><span data-stu-id="bc907-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="bc907-112">Se você estiver usando o EWS, é possível criar um pequeno aplicativo usando a API gerenciada do EWS, rastreá-lo e usar as informações de solicitação XML para ajudá-lo a criar sua solicitação do EWS.</span><span class="sxs-lookup"><span data-stu-id="bc907-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="bc907-113">Habilitando o rastreamento no objeto ExchangeService</span><span class="sxs-lookup"><span data-stu-id="bc907-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="bc907-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="bc907-114"><a name="bk_EnableTracing"> </a></span></span>

<span data-ttu-id="bc907-115">Para habilitar o rastreamento, crie um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para o seu aplicativo e defina as propriedades de rastreamento, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="bc907-115">To enable tracing, create an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="bc907-116">Depois de definir a propriedade [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true**, todas as solicitações que correspondam aos sinalizadores de rastreamento serão enviadas para o ouvinte de rastreamento especificado.</span><span class="sxs-lookup"><span data-stu-id="bc907-116">After you set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="bc907-117">Você pode especificar um único sinalizador de rastreamento ou pode especificar vários sinalizadores de rastreamento combinando-os com um **or**lógico.</span><span class="sxs-lookup"><span data-stu-id="bc907-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="bc907-118">Você pode usar a [Enumeração TraceFlags](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) para especificar valores para EWS e para solicitações e respostas de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="bc907-118">You can use the [TraceFlags enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="bc907-119">Implementar um objeto TraceListener</span><span class="sxs-lookup"><span data-stu-id="bc907-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="bc907-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="bc907-120"><a name="bk_traceListener"> </a></span></span>

<span data-ttu-id="bc907-121">Você pode definir a propriedade [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true** para gerar as solicitações e respostas XML para seu aplicativo, como uma janela do console.</span><span class="sxs-lookup"><span data-stu-id="bc907-121">You can set the [TraceEnabled](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="bc907-122">Se você quiser controlar a saída de rastreamento e salvá-la em um arquivo, recomendamos que você implemente um objeto de [classe TraceListener](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bc907-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](https://msdn.microsoft.com/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="bc907-123">O exemplo de código a seguir mostra um objeto simples que implementa a interface [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) e armazena as solicitações e respostas rastreadas em XML ou arquivos de texto.</span><span class="sxs-lookup"><span data-stu-id="bc907-123">The following code example shows a simple object that implements the [ITraceListener](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="bc907-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc907-124">See also</span></span>

- [<span data-ttu-id="bc907-125">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="bc907-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="bc907-126">Manipulação de mensagens de erro de Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="bc907-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="bc907-127">Fazer referência ao assembly da API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="bc907-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="bc907-128">Comunicar-se com o EWS usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="bc907-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

