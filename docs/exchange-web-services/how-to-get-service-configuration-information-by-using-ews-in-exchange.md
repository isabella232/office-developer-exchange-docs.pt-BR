---
title: Obter informações de configuração de serviço usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Descubra como obter informações de configuração do serviço de Unificação de mensagens, pedidos de atenção de política, dicas de email e regras de proteção do EWS no Exchange.
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750719"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="4e218-103">Obter informações de configuração de serviço usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4e218-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="4e218-104">Descubra como obter informações de configuração do serviço de Unificação de mensagens, pedidos de atenção de política, dicas de email e regras de proteção do EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e218-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="4e218-105">Seu aplicativo EWS funciona com a Unificação de mensagens (UM), pedidos de atenção de política, dicas de email ou regras de proteção?</span><span class="sxs-lookup"><span data-stu-id="4e218-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="4e218-106">Nesse caso, o seu aplicativo precisará chamar a [operação GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para obter as informações de configuração de serviço que ele precisa.</span><span class="sxs-lookup"><span data-stu-id="4e218-106">If so, your application will need to call the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="4e218-107">A operação **GetServiceConfiguration** retorna informações de configuração que são específicas para cada um desses recursos do EWS.</span><span class="sxs-lookup"><span data-stu-id="4e218-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4e218-108">A API gerenciada EWS não implementa essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="4e218-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="4e218-109">**Tabela 1. Informações de configuração que a operação GetServiceConfiguration retorna**</span><span class="sxs-lookup"><span data-stu-id="4e218-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="4e218-110">Recurso EWS</span><span class="sxs-lookup"><span data-stu-id="4e218-110">EWS feature</span></span>|<span data-ttu-id="4e218-111">Retorna a operação GetServiceConfiguration …</span><span class="sxs-lookup"><span data-stu-id="4e218-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e218-112">UM</span><span class="sxs-lookup"><span data-stu-id="4e218-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="4e218-113">Um valor que indica se a Unificação de mensagens está habilitada.</span><span class="sxs-lookup"><span data-stu-id="4e218-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="4e218-114">Um valor que indica se a opção Tocar no telefone está habilitada.</span><span class="sxs-lookup"><span data-stu-id="4e218-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="4e218-115">Tocar no sequência de discagem do telefone.</span><span class="sxs-lookup"><span data-stu-id="4e218-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="4e218-116">Deslocar da diretiva</span><span class="sxs-lookup"><span data-stu-id="4e218-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="4e218-117">Política desloca para exibição no seu cliente.</span><span class="sxs-lookup"><span data-stu-id="4e218-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="4e218-118">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="4e218-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="4e218-119">Um valor que indica se as dicas de email estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="4e218-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="4e218-120">O número máximo de destinatários por solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e218-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="4e218-121">O tamanho máximo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4e218-121">The maximum message size.</span></span></li><li><span data-ttu-id="4e218-122">O limite de grande público.</span><span class="sxs-lookup"><span data-stu-id="4e218-122">The large audience threshold.</span></span></li><li><span data-ttu-id="4e218-123">Um valor que indica se o número de destinatários externos é mostrado.</span><span class="sxs-lookup"><span data-stu-id="4e218-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="4e218-124">Uma lista de domínios internos.</span><span class="sxs-lookup"><span data-stu-id="4e218-124">A list of internal domains.</span></span></li><li><span data-ttu-id="4e218-125">Um valor que indica se as dicas de política estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="4e218-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="4e218-126">O limite de cobrir grande público para indicando se o seu email é considerado como tiver um grande número de destinatários.</span><span class="sxs-lookup"><span data-stu-id="4e218-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="4e218-127">Regras de proteção</span><span class="sxs-lookup"><span data-stu-id="4e218-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="4e218-128">Configuração de regras de proteção para seu cliente.</span><span class="sxs-lookup"><span data-stu-id="4e218-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="4e218-129">Uma lista de domínios que são internos para sua organização.</span><span class="sxs-lookup"><span data-stu-id="4e218-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="4e218-130">Exemplo de código: obter informações de configuração do serviço de dicas de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4e218-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="4e218-131">O exemplo de código a seguir usa a [operação GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para solicitar informações de configuração de serviço para dicas de email.</span><span class="sxs-lookup"><span data-stu-id="4e218-131">The following code example uses the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="4e218-132">Você pode solicitar informações de configuração de serviço adicionais, adicionando mais elementos [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) com valores diferentes.</span><span class="sxs-lookup"><span data-stu-id="4e218-132">You can request additional service configuration information by adding more [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a><span data-ttu-id="4e218-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4e218-133">Next steps</span></span>

<span data-ttu-id="4e218-134">Depois de solicitar informações de configuração de serviço, use a [classe XmlDocument](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) para carregar a resposta XML para que você possa analisá-lo.</span><span class="sxs-lookup"><span data-stu-id="4e218-134">After you request service configuration information, use the [XmlDocument class](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="4e218-135">Em seguida, dependendo do cenário, você pode fazer um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4e218-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="4e218-136">Use a [operação GetMailTips](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) para obter dicas de email para aplicativos de cliente exibir aos usuários.</span><span class="sxs-lookup"><span data-stu-id="4e218-136">Use the [GetMailTips operation](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="4e218-137">Se UM estiver habilitado, [Saiba mais sobre como reproduzir itens da caixa de correio](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) seu telefone.</span><span class="sxs-lookup"><span data-stu-id="4e218-137">If UM is enabled, [learn about how to play mailbox items](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="4e218-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="4e218-138">See also</span></span>

- [<span data-ttu-id="4e218-139">Opções de configuração para o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4e218-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="4e218-140">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="4e218-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="4e218-141">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="4e218-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

