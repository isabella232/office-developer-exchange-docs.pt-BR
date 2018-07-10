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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750825"
---
# <a name="trace-requests-and-responses-to-troubleshoot-ews-managed-api-apps"></a><span data-ttu-id="30700-103">Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento</span><span class="sxs-lookup"><span data-stu-id="30700-103">Trace requests and responses to troubleshoot EWS Managed API apps</span></span>

<span data-ttu-id="30700-104">Descubra como EWS solicitações e respostas para solucionar erros no seu aplicativo do EWS Managed API de rastreamento.</span><span class="sxs-lookup"><span data-stu-id="30700-104">Find out how to trace EWS requests and responses to troubleshoot errors in your EWS Managed API application.</span></span>
  
<span data-ttu-id="30700-105">Depurar um aplicativo baseado no serviço da web pode ser difícil porque está sendo executada em um computador remoto que talvez você não tenha acesso à parte do processamento.</span><span class="sxs-lookup"><span data-stu-id="30700-105">Debugging a web service-based application can be difficult because part of the processing is performed on a remote computer that you might not have access to.</span></span> <span data-ttu-id="30700-106">Porque você não pode percorrer o código no servidor, ele pode ser útil ver as solicitações XML e respostas enviadas entre o cliente e o servidor para determinar qual parte do aplicativo está causando um erro.</span><span class="sxs-lookup"><span data-stu-id="30700-106">Because you cannot step through the code on the server, it can be helpful to see the XML requests and responses that are sent between the client and the server to determine which part of the application is causing an error.</span></span> 
  
<span data-ttu-id="30700-107">Se você estiver usando o EWS, você já tem acesso à solicitação XML e resposta; Você pode colocar um ponto de interrupção em seu código para analisar a resposta do servidor à sua solicitação para solucionar um problema.</span><span class="sxs-lookup"><span data-stu-id="30700-107">If you are using EWS, you already have access to the XML request and response; you can put a break point in your code to review the server's response to your request in order to troubleshoot an issue.</span></span> <span data-ttu-id="30700-108">Se você estiver usando a API gerenciada de EWS, você não tem acesso direto para a solicitação do EWS e a resposta.</span><span class="sxs-lookup"><span data-stu-id="30700-108">If you're using the EWS Managed API, you don't have direct access to the EWS request and response.</span></span> <span data-ttu-id="30700-109">No entanto, você pode usar os métodos de rastreamento no objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para capturar a solicitação XML e a resposta e, em seguida, você pode usar o XML para determinar porque seu código não está funcionando.</span><span class="sxs-lookup"><span data-stu-id="30700-109">However, you can use tracing methods on the [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object to capture the XML request and response, and you can then use the XML to determine why your code is not working.</span></span> 

<span data-ttu-id="30700-110">Por exemplo, se você não definir uma propriedade corretamente, você pode receber uma resposta inesperada e você pode usar a saída de rastreamento para examinar a solicitação XML e a resposta para identificar o erro.</span><span class="sxs-lookup"><span data-stu-id="30700-110">For example, if you did not set a property correctly, you might get an unexpected response, and you can use the trace output to look at the XML request and response to identify the error.</span></span> <span data-ttu-id="30700-111">A saída do rastreamento da API gerenciada do EWS pode ajudá-lo a criar manualmente a solicitação XML para criar o seu aplicativo do EWS.</span><span class="sxs-lookup"><span data-stu-id="30700-111">The trace output from the EWS Managed API can also help you manually build the XML request to create your EWS application.</span></span> <span data-ttu-id="30700-112">Se você estiver usando o EWS, você pode criar um aplicativo pequeno usando o EWS Managed API, rastreá-lo e, em seguida, use as informações de solicitação XML para ajudar a construir sua solicitação EWS.</span><span class="sxs-lookup"><span data-stu-id="30700-112">If you are using EWS, you can create a small application by using EWS Managed API, trace it, and then use the XML request information to help you build your EWS request.</span></span> 
  
## <a name="enabling-tracing-on-the-exchangeservice-object"></a><span data-ttu-id="30700-113">A habilitação do rastreamento no objeto ExchangeService</span><span class="sxs-lookup"><span data-stu-id="30700-113">Enabling tracing on the ExchangeService object</span></span>
<span data-ttu-id="30700-114"><a name="bk_EnableTracing"> </a></span><span class="sxs-lookup"><span data-stu-id="30700-114"></span></span>

<span data-ttu-id="30700-115">Para habilitar o rastreamento, crie um objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para seu aplicativo e definir as propriedades de rastreamento, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="30700-115">To enable tracing, create an [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for your application, and set the tracing properties as shown in the following example.</span></span> 
  
```cs
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2010);
service.TraceListener = ITraceListenerInstance;
// Optional flags to indicate the requests and responses to trace.
service.TraceFlags = TraceFlags.EwsRequest | TraceFlags.EwsResponse
service.TraceEnabled = true;

```

<span data-ttu-id="30700-116">Depois de definir a propriedade [TraceEnabled](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true**, todas as solicitações que coincidem com os sinalizadores de rastreamento serão enviadas ao ouvinte de rastreamento especificado.</span><span class="sxs-lookup"><span data-stu-id="30700-116">After you set the [TraceEnabled](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true**, all requests that match the trace flags will be sent to the specified trace listener.</span></span> <span data-ttu-id="30700-117">Você pode especificar um sinalizador de rastreamento único, ou você pode especificar vários sinalizadores de rastreamento, combinando-os com uma lógica **OR**.</span><span class="sxs-lookup"><span data-stu-id="30700-117">You can specify a single trace flag, or you can specify multiple trace flags by combining them with a logical **OR**.</span></span> <span data-ttu-id="30700-118">Você pode usar a [enumeração TraceFlags](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) para especificar valores para o EWS e respostas e solicitações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="30700-118">You can use the [TraceFlags enumeration](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.traceflags%28v=exchg.80%29.aspx) to specify values for EWS and for Autodiscover requests and responses.</span></span> 
  
## <a name="implementing-a-tracelistener-object"></a><span data-ttu-id="30700-119">Implementação de um objeto TraceListener</span><span class="sxs-lookup"><span data-stu-id="30700-119">Implementing a TraceListener object</span></span>
<span data-ttu-id="30700-120"><a name="bk_traceListener"> </a></span><span class="sxs-lookup"><span data-stu-id="30700-120"></span></span>

<span data-ttu-id="30700-121">Você pode definir a propriedade [TraceEnabled](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) como **true** para as solicitações XML e respostas para seu aplicativo, como uma janela do console de saída.</span><span class="sxs-lookup"><span data-stu-id="30700-121">You can set the [TraceEnabled](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.traceenabled%28v=exchg.80%29.aspx) property to **true** to output the XML requests and responses to your application, such as a console window.</span></span> <span data-ttu-id="30700-122">Se você quiser controlar a saída de rastreamento e salvá-lo em um arquivo, recomendamos que você implemente um objeto de [classe TraceListener](http://msdn.microsoft.com/pt-br/library/system.diagnostics.tracelistener.aspx) .</span><span class="sxs-lookup"><span data-stu-id="30700-122">If you want to control the trace output and save it to a file, we recommend that you implement a [TraceListener class](http://msdn.microsoft.com/pt-br/library/system.diagnostics.tracelistener.aspx) object.</span></span> <span data-ttu-id="30700-123">O exemplo de código a seguir mostra um objeto simple que implementa a interface [ITraceListener](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) e armazena as rastreados solicitações e respostas em arquivos XML ou de texto.</span><span class="sxs-lookup"><span data-stu-id="30700-123">The following code example shows a simple object that implements the [ITraceListener](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itracelistener%28v=exchg.80%29.aspx) interface and stores the traced requests and responses in XML or text files.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="30700-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="30700-124">See also</span></span>

- [<span data-ttu-id="30700-125">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="30700-125">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
- [<span data-ttu-id="30700-126">Manipulação de mensagens de erro de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="30700-126">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)    
- [<span data-ttu-id="30700-127">Faça referência ao conjunto de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="30700-127">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)    
- [<span data-ttu-id="30700-128">Comunicar-se com o EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="30700-128">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

