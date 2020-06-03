---
title: Obter informações de configuração de serviço usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Descubra como obter informações de configuração de serviço para UM, deslocamentos de política, dicas de email e regras de proteção do EWS no Exchange.
ms.openlocfilehash: 7546d9524f1e004eda2bdc55687fb44beafa44af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528003"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="b96ae-103">Obter informações de configuração de serviço usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b96ae-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="b96ae-104">Descubra como obter informações de configuração de serviço para UM, deslocamentos de política, dicas de email e regras de proteção do EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b96ae-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="b96ae-105">O aplicativo EWS funciona com a Unificação de mensagens (UM), os deslocamentos de política, as dicas de email ou as regras de proteção?</span><span class="sxs-lookup"><span data-stu-id="b96ae-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="b96ae-106">Em caso afirmativo, o aplicativo precisará chamar a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para obter as informações de configuração de serviço de que precisa.</span><span class="sxs-lookup"><span data-stu-id="b96ae-106">If so, your application will need to call the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="b96ae-107">A operação **GetServiceConfiguration** retorna as informações de configuração específicas de cada um desses recursos do EWS.</span><span class="sxs-lookup"><span data-stu-id="b96ae-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b96ae-108">A API gerenciada EWS não implementa essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="b96ae-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="b96ae-109">**Tabela 1. Informações de configuração que a operação GetServiceConfiguration retorna**</span><span class="sxs-lookup"><span data-stu-id="b96ae-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="b96ae-110">Recurso EWS</span><span class="sxs-lookup"><span data-stu-id="b96ae-110">EWS feature</span></span>|<span data-ttu-id="b96ae-111">A operação GetServiceConfiguration retorna...</span><span class="sxs-lookup"><span data-stu-id="b96ae-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="b96ae-112">UM</span><span class="sxs-lookup"><span data-stu-id="b96ae-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="b96ae-113">Um valor que indica se a UM está habilitada.</span><span class="sxs-lookup"><span data-stu-id="b96ae-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="b96ae-114">Um valor que indica se tocar no telefone está habilitado.</span><span class="sxs-lookup"><span data-stu-id="b96ae-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="b96ae-115">A cadeia de caracteres de discagem por telefone.</span><span class="sxs-lookup"><span data-stu-id="b96ae-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="b96ae-116">Deslocamentos de política</span><span class="sxs-lookup"><span data-stu-id="b96ae-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="b96ae-117">Os deslocamentos de política para exibição no cliente.</span><span class="sxs-lookup"><span data-stu-id="b96ae-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="b96ae-118">Dicas de email</span><span class="sxs-lookup"><span data-stu-id="b96ae-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="b96ae-119">Um valor que indica se as dicas de email estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="b96ae-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="b96ae-120">O número máximo de destinatários por solicitação.</span><span class="sxs-lookup"><span data-stu-id="b96ae-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="b96ae-121">O tamanho máximo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b96ae-121">The maximum message size.</span></span></li><li><span data-ttu-id="b96ae-122">O limite grande de audiências.</span><span class="sxs-lookup"><span data-stu-id="b96ae-122">The large audience threshold.</span></span></li><li><span data-ttu-id="b96ae-123">Um valor que indica se o número de destinatários externos é mostrado.</span><span class="sxs-lookup"><span data-stu-id="b96ae-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="b96ae-124">Uma lista de domínios internos.</span><span class="sxs-lookup"><span data-stu-id="b96ae-124">A list of internal domains.</span></span></li><li><span data-ttu-id="b96ae-125">Um valor que indica se as dicas de política estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="b96ae-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="b96ae-126">O limite de grandes audiências para indicar se o email é considerado como tendo um grande número de destinatários.</span><span class="sxs-lookup"><span data-stu-id="b96ae-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="b96ae-127">Regras de proteção</span><span class="sxs-lookup"><span data-stu-id="b96ae-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="b96ae-128">Configuração de regras de proteção para o cliente.</span><span class="sxs-lookup"><span data-stu-id="b96ae-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="b96ae-129">Uma lista de domínios internos da sua organização.</span><span class="sxs-lookup"><span data-stu-id="b96ae-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="b96ae-130">Exemplo de código: obter informações de configuração de serviço para dicas de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="b96ae-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="b96ae-131">O exemplo de código a seguir usa a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para solicitar informações de configuração de serviço para dicas de email.</span><span class="sxs-lookup"><span data-stu-id="b96ae-131">The following code example uses the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="b96ae-132">Você pode solicitar informações adicionais de configuração de serviço adicionando mais elementos [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) com valores diferentes.</span><span class="sxs-lookup"><span data-stu-id="b96ae-132">You can request additional service configuration information by adding more [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
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

## <a name="next-steps"></a><span data-ttu-id="b96ae-133">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="b96ae-133">Next steps</span></span>

<span data-ttu-id="b96ae-134">Depois de solicitar informações de configuração de serviço, use a [classe XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) para carregar o XML de resposta para que você possa analisá-lo.</span><span class="sxs-lookup"><span data-stu-id="b96ae-134">After you request service configuration information, use the [XmlDocument class](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="b96ae-135">Em seguida, dependendo do seu cenário, você pode executar uma das seguintes ações:</span><span class="sxs-lookup"><span data-stu-id="b96ae-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="b96ae-136">Use a [operação](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) GetQuery para obter dicas de email para aplicativos cliente exibir aos usuários.</span><span class="sxs-lookup"><span data-stu-id="b96ae-136">Use the [GetMailTips operation](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="b96ae-137">Se a UM estiver habilitada, [saiba mais sobre como reproduzir itens de caixa de correio](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) pelo telefone.</span><span class="sxs-lookup"><span data-stu-id="b96ae-137">If UM is enabled, [learn about how to play mailbox items](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="b96ae-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="b96ae-138">See also</span></span>

- [<span data-ttu-id="b96ae-139">Opções de configuração do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b96ae-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="b96ae-140">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="b96ae-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="b96ae-141">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="b96ae-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

