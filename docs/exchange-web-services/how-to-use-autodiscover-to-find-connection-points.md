---
title: Usar descoberta automática para encontrar os pontos de conexão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Descubra como usar o serviço Descoberta automática para direcionar o seu aplicativo cliente para o servidor Exchange correto.
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750837"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="f00d3-103">Usar descoberta automática para encontrar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="f00d3-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="f00d3-104">Descubra como usar o serviço Descoberta automática para direcionar o seu aplicativo cliente para o servidor Exchange correto.</span><span class="sxs-lookup"><span data-stu-id="f00d3-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="f00d3-105">O serviço de descoberta automática do Exchange fornece seu aplicativo de cliente com as definições de configuração para contas de email hospedadas no Exchange Online, Exchange Online como parte do Office 365 ou um servidor do Exchange executando uma versão do Exchange, começando com o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="f00d3-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="f00d3-106">O serviço de descoberta automática é um serviço web que fornece configurações.</span><span class="sxs-lookup"><span data-stu-id="f00d3-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="f00d3-107">O serviço de descoberta automática é um serviço web que fornece informações de configuração de servidor do Exchange ao seu aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="f00d3-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="f00d3-108">Aplicativos clientes usam a descoberta automática para determinar o ponto de extremidade do serviço Descoberta automática para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="f00d3-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="f00d3-109">Este artigo explica como a seguir as respostas de um servidor Exchange para localizar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="f00d3-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="f00d3-110">Para obter informações sobre como obter as definições de configuração de endereço de email, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e [Obtenha as configurações de domínio de um servidor Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="f00d3-111">O processo para localizar o ponto de extremidade correto é parte da solicitação de usuário ou de configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="f00d3-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="f00d3-112">O serviço Descoberta automática usa uma série de respostas de redirecionamento para enviar o aplicativo cliente para o ponto de extremidade correto para um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="f00d3-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="f00d3-113">Você pode usar uma das seguintes tecnologias de desenvolvimento do Exchange para acessar o serviço de descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="f00d3-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>
  
> [!NOTE]
> <span data-ttu-id="f00d3-114">Para obter mais informações sobre essas tecnologias de desenvolvimento do Exchange, consulte a [explorar o EWS Managed API, EWS e web services no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-114">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 
  
- <span data-ttu-id="f00d3-115">Exchange Web Services API gerenciada de (EWS)</span><span class="sxs-lookup"><span data-stu-id="f00d3-115">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="f00d3-116">EWS</span><span class="sxs-lookup"><span data-stu-id="f00d3-116">EWS</span></span>
    
    <span data-ttu-id="f00d3-117">Se você estiver usando o EWS, você pode usar os seguintes métodos para recuperar as configurações do usuário:</span><span class="sxs-lookup"><span data-stu-id="f00d3-117">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
  - <span data-ttu-id="f00d3-118">O serviço Descoberta automática de baseados em SOAP</span><span class="sxs-lookup"><span data-stu-id="f00d3-118">The SOAP-based Autodiscover service</span></span>
    
  - <span data-ttu-id="f00d3-119">O serviço Descoberta automática de POX (XML)</span><span class="sxs-lookup"><span data-stu-id="f00d3-119">The XML (POX) Autodiscover service</span></span>
    
  - <span data-ttu-id="f00d3-120">Um proxy gerada automaticamente gerado a partir do serviço Descoberta automática de XML ou de SOAP</span><span class="sxs-lookup"><span data-stu-id="f00d3-120">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
    <span data-ttu-id="f00d3-121">Para obter mais informações sobre esses métodos, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-121">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>
    
<span data-ttu-id="f00d3-122">A API gerenciada de EWS fornece uma interface baseada no objeto para recuperar as configurações do usuário.</span><span class="sxs-lookup"><span data-stu-id="f00d3-122">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="f00d3-123">Se seu aplicativo cliente usa código gerenciado, é recomendável que você use a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="f00d3-123">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="f00d3-124">A interface de API gerenciada de EWS melhor é otimizada para um modelo de objeto simples que o proxy do serviço web gerado automaticamente típica.</span><span class="sxs-lookup"><span data-stu-id="f00d3-124">The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="f00d3-125">Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática de SOAP, porque ele oferece suporte a um conjunto avançado de recursos do serviço de descoberta automática de POX.</span><span class="sxs-lookup"><span data-stu-id="f00d3-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="f00d3-126">Pré-requisitos para localizar um ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f00d3-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="f00d3-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="f00d3-127"></span></span>

<span data-ttu-id="f00d3-128">Antes de criar um aplicativo cliente que usa o serviço de descoberta automática, você precisa ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="f00d3-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="f00d3-129">O Exchange Online ou um servidor que está executando uma versão do Exchange, começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f00d3-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="f00d3-130">Se você estiver usando o serviço de descoberta automática de baseados em SOAP, o Exchange Online ou uma versão do Exchange, começando com o Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="f00d3-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="f00d3-131">Um servidor do Exchange que está configurado para aceitar conexões de seu aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="f00d3-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="f00d3-132">Para obter informações sobre como configurar seu servidor do Exchange, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="f00d3-133">Uma conta que está autorizada a utilizar o EWS.</span><span class="sxs-lookup"><span data-stu-id="f00d3-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="f00d3-134">Para obter informações sobre como configurar uma conta, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f00d3-135">Se você estiver usando a API gerenciada de EWS, você deve fornecer um retorno de chamada de validação de certificado em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="f00d3-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="f00d3-136">Talvez seja necessário também um retorno de chamada de validação de certificado com bibliotecas de proxy gerado, como aqueles criados pelo Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="f00d3-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="f00d3-137">Para obter mais informações, consulte [Validar um certificado de servidor para a API gerenciada de EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="f00d3-138">Principais conceitos para localizar um ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f00d3-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="f00d3-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="f00d3-139"></span></span>

<span data-ttu-id="f00d3-140">Antes de você usar a descoberta automática para localizar um ponto de extremidade, você deve estar familiarizado com os conceitos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f00d3-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="f00d3-141">**Conceito**</span><span class="sxs-lookup"><span data-stu-id="f00d3-141">**Concept**</span></span>|<span data-ttu-id="f00d3-142">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f00d3-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f00d3-143">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f00d3-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="f00d3-144">Fornece uma visão geral de como funciona o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f00d3-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="f00d3-145">Se você estiver usando o EWS Managed API, use a classe [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) no namespace [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão para o EWS.</span><span class="sxs-lookup"><span data-stu-id="f00d3-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="f00d3-146">Para usar as amostras de código do API gerenciada de EWS neste artigo, você precisa fazer referência os seguintes namespaces em seu código:</span><span class="sxs-lookup"><span data-stu-id="f00d3-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="f00d3-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="f00d3-147">**System.Net**</span></span>
    
- <span data-ttu-id="f00d3-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="f00d3-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="f00d3-149">Encontre o ponto de extremidade correto usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="f00d3-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="f00d3-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="f00d3-150"></span></span>

<span data-ttu-id="f00d3-151">Se você estiver usando a API gerenciada de EWS, as chamadas para o serviço de descoberta automática são manipuladas pela classe **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="f00d3-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="f00d3-152">Para determinar o ponto de extremidade correto para uma conta de email, você pode chamar o método **AutodiscoverUrl** em um objeto **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="f00d3-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="f00d3-153">O exemplo de código a seguir mostra como definir o ponto de extremidade de serviço do EWS web para um endereço de email para o arquivo de Exchange.asmx no servidor de acesso para cliente correto usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="f00d3-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="f00d3-154">Localizar o ponto de extremidade correto usando o EWS</span><span class="sxs-lookup"><span data-stu-id="f00d3-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="f00d3-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="f00d3-155"></span></span>

<span data-ttu-id="f00d3-156">O serviço Descoberta automática do SOAP pode usar uma série de solicitações e respostas para direcionar o seu aplicativo para o ponto de extremidade correto para o EWS.</span><span class="sxs-lookup"><span data-stu-id="f00d3-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="f00d3-157">Para obter informações sobre o processo para determinar o ponto de extremidade correto para uma conta de email, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="f00d3-158">Os exemplos XML a seguir mostram a série de solicitações e respostas que você pode esperar quando você faz uma solicitação de descoberta automática do SOAP para localizar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="f00d3-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="f00d3-159">Solicitação de ponto de extremidade de descoberta automática do SOAP</span><span class="sxs-lookup"><span data-stu-id="f00d3-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="f00d3-160">O exemplo a seguir mostra uma solicitação XML que será enviada para o serviço Descoberta automática para localizar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="f00d3-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="f00d3-161">Resposta de redirecionamento de descoberta automática do SOAP</span><span class="sxs-lookup"><span data-stu-id="f00d3-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="f00d3-162">O serviço Descoberta automática pode responder com uma das duas respostas de redirecionamento: um redirecionamento HTTP 302 ou uma resposta de redirecionamento de SOAP.</span><span class="sxs-lookup"><span data-stu-id="f00d3-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="f00d3-163">Se a resposta do servidor Exchange for um redirecionamento HTTP 302, o aplicativo cliente deve validar que o endereço de redirecionamento é aceitável e siga a resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="f00d3-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [! Observação de segurança]<span data-ttu-id="f00d3-164"> para critérios para a validação de uma resposta de redirecionamento, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f00d3-164"> For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="f00d3-165">Se o serviço de descoberta automática retorna uma resposta de redirecionamento, indicada pelo [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento de **resposta** , o aplicativo cliente deve usar o elemento **RedirectTarget** construir uma nova solicitação de configurações é enviado para o servidor especificado na resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="f00d3-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="f00d3-166">O exemplo a seguir mostra uma resposta de redirecionamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="f00d3-166">The following example shows a redirection response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="f00d3-167">Após um redirecionamento, o cliente usa a URL de redirecionamento para preparar a solicitação de outra.</span><span class="sxs-lookup"><span data-stu-id="f00d3-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="f00d3-168">O código a seguir mostra um exemplo da solicitação que você cria com a resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="f00d3-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f00d3-169">Quando o aplicativo cliente foi direcionado para o ponto de extremidade correto para o serviço de descoberta automática, o servidor enviará uma resposta com o [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento de **resposta** definido como **NoError** e contendo os solicitados configurações de usuário.</span><span class="sxs-lookup"><span data-stu-id="f00d3-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="f00d3-170">Somente as usuário solicitado configurações, **InternalEwsUrl** e **ExternalEwsUrl**, são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f00d3-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="f00d3-171">O exemplo a seguir mostra a resposta do servidor.</span><span class="sxs-lookup"><span data-stu-id="f00d3-171">The following example shows the response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="f00d3-172">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f00d3-172">Next steps</span></span>
<span data-ttu-id="f00d3-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="f00d3-173"></span></span>

<span data-ttu-id="f00d3-174">Localizar o ponto de extremidade seguindo o processo de descoberta automática retorna as configurações de usuário ou de domínio solicitado.</span><span class="sxs-lookup"><span data-stu-id="f00d3-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="f00d3-175">Para obter informações sobre como fazer uma solicitação para configurações específicas, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="f00d3-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="f00d3-176">Fazer configurações de domínio a partir de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="f00d3-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="f00d3-177">Obter configurações de usuário do Exchange usando a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="f00d3-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="f00d3-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="f00d3-178">See also</span></span>


- [<span data-ttu-id="f00d3-179">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="f00d3-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    
- [<span data-ttu-id="f00d3-180">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f00d3-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="f00d3-181">Referência de web service de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f00d3-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [<span data-ttu-id="f00d3-182">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="f00d3-182">EWS reference for Exchange</span></span>](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

