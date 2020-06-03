---
title: Usar a Descoberta Automática para localizar os pontos de conexão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Descubra como usar o serviço de descoberta automática para direcionar seu aplicativo cliente para o servidor Exchange correto.
localization_priority: Priority
ms.openlocfilehash: c1895fa0d2cce489467a726614e9457052624ef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527590"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="47f6f-103">Usar a Descoberta Automática para localizar os pontos de conexão</span><span class="sxs-lookup"><span data-stu-id="47f6f-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="47f6f-104">Descubra como usar o serviço de descoberta automática para direcionar seu aplicativo cliente para o servidor Exchange correto.</span><span class="sxs-lookup"><span data-stu-id="47f6f-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="47f6f-105">O serviço de descoberta automática do Exchange fornece ao aplicativo cliente definições de configuração para contas de email hospedadas no Exchange Online, Exchange Online como parte do Office 365 ou um servidor Exchange executando uma versão do Exchange a partir do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="47f6f-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="47f6f-106">O serviço de descoberta automática é um serviço Web que fornece definições de configuração.</span><span class="sxs-lookup"><span data-stu-id="47f6f-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="47f6f-107">O serviço de descoberta automática é um serviço Web que fornece informações de configuração do Exchange Server para o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="47f6f-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="47f6f-108">Os aplicativos cliente usam a descoberta automática para determinar o ponto de extremidade do serviço de descoberta automática para uma caixa de correio específica.</span><span class="sxs-lookup"><span data-stu-id="47f6f-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="47f6f-109">Este artigo explica como seguir as respostas de um servidor do Exchange para encontrar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="47f6f-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="47f6f-110">Para obter informações sobre como obter definições de configuração de endereço de email, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e [obter as configurações de domínio de um servidor Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="47f6f-111">O processo para localizar o ponto de extremidade correto faz parte da solicitação de configurações de usuário ou domínio.</span><span class="sxs-lookup"><span data-stu-id="47f6f-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="47f6f-112">O serviço de descoberta automática usa uma série de respostas de redirecionamento para enviar o aplicativo cliente para o ponto de extremidade correto para um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="47f6f-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="47f6f-113">Você pode usar uma das seguintes tecnologias de desenvolvimento do Exchange para acessar o serviço de descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="47f6f-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>

- <span data-ttu-id="47f6f-114">A API gerenciada dos serviços Web do Exchange (EWS)</span><span class="sxs-lookup"><span data-stu-id="47f6f-114">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="47f6f-115">EWS</span><span class="sxs-lookup"><span data-stu-id="47f6f-115">EWS</span></span>
    
<span data-ttu-id="47f6f-116">Se estiver usando o EWS, você poderá usar os seguintes métodos para recuperar as configurações do usuário:</span><span class="sxs-lookup"><span data-stu-id="47f6f-116">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
- <span data-ttu-id="47f6f-117">O serviço de descoberta automática baseado em SOAP</span><span class="sxs-lookup"><span data-stu-id="47f6f-117">The SOAP-based Autodiscover service</span></span>
    
- <span data-ttu-id="47f6f-118">O serviço de descoberta automática de XML (POX)</span><span class="sxs-lookup"><span data-stu-id="47f6f-118">The XML (POX) Autodiscover service</span></span>
    
- <span data-ttu-id="47f6f-119">Um proxy gerado automaticamente a partir do serviço de descoberta automática SOAP ou XML</span><span class="sxs-lookup"><span data-stu-id="47f6f-119">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
<span data-ttu-id="47f6f-120">Para obter mais informações sobre esses métodos, consulte [autodiscover for Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-120">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>

<span data-ttu-id="47f6f-121">Para obter mais informações sobre essas tecnologias de desenvolvimento do Exchange, consulte [explorar a API gerenciada do EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-121">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 

<span data-ttu-id="47f6f-122">A API gerenciada do EWS fornece uma interface baseada em objeto para recuperar as configurações do usuário.</span><span class="sxs-lookup"><span data-stu-id="47f6f-122">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="47f6f-123">Se seu aplicativo cliente usa código gerenciado, recomendamos que você use a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="47f6f-123">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="47f6f-124">A interface de API gerenciada do EWS é melhor otimizada para um modelo de objeto simples do que o proxy de serviço Web do autogerable típico.</span><span class="sxs-lookup"><span data-stu-id="47f6f-124">The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="47f6f-125">Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática do SOAP, pois ele oferece suporte a um conjunto mais amplo de recursos do que o serviço de descoberta automática do POX.</span><span class="sxs-lookup"><span data-stu-id="47f6f-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="47f6f-126">Pré-requisitos para localizar um ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="47f6f-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="47f6f-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="47f6f-127"><a name="bk_Prereq"> </a></span></span>

<span data-ttu-id="47f6f-128">Antes de poder criar um aplicativo cliente que usa o serviço de descoberta automática, você precisa ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="47f6f-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="47f6f-129">Exchange Online ou um servidor que esteja executando uma versão do Exchange a partir do Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="47f6f-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="47f6f-130">Se você estiver usando o serviço de descoberta automática baseado em SOAP, o Exchange Online ou uma versão do Exchange a partir do Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="47f6f-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="47f6f-131">Um servidor do Exchange que é configurado para aceitar conexões do seu aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="47f6f-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="47f6f-132">Para obter informações sobre como configurar seu servidor Exchange, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="47f6f-133">Uma conta que está autorizada a usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="47f6f-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="47f6f-134">Para obter informações sobre como configurar uma conta, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="47f6f-135">Se você estiver usando a API gerenciada do EWS, deverá fornecer um retorno de chamada de validação de certificado em algumas circunstâncias.</span><span class="sxs-lookup"><span data-stu-id="47f6f-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="47f6f-136">Você também pode precisar de um retorno de chamada de validação de certificado com algumas bibliotecas de proxy geradas, como as criadas pelo Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="47f6f-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="47f6f-137">Para saber mais, confira [validar um certificado de servidor para a API gerenciada do EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="47f6f-138">Principais conceitos para localizar um ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="47f6f-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="47f6f-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="47f6f-139"><a name="bk_Core"> </a></span></span>

<span data-ttu-id="47f6f-140">Antes de usar a descoberta automática para localizar um ponto de extremidade, você deve estar familiarizado com os conceitos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="47f6f-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="47f6f-141">**Conceito**</span><span class="sxs-lookup"><span data-stu-id="47f6f-141">**Concept**</span></span>|<span data-ttu-id="47f6f-142">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f6f-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f6f-143">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="47f6f-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="47f6f-144">Fornece uma visão geral de como o serviço de descoberta automática funciona.</span><span class="sxs-lookup"><span data-stu-id="47f6f-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="47f6f-145">Se você estiver usando a API gerenciada do EWS, use a classe [Microsoft. Exchange. WebServices. Data. ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) no namespace [Microsoft. Exchange. WebServices. Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão com o EWS.</span><span class="sxs-lookup"><span data-stu-id="47f6f-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="47f6f-146">Para usar os exemplos de código da API gerenciada do EWS neste artigo, você precisa fazer referência aos seguintes namespaces no seu código:</span><span class="sxs-lookup"><span data-stu-id="47f6f-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="47f6f-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="47f6f-147">**System.Net**</span></span>
    
- <span data-ttu-id="47f6f-148">**Microsoft. Exchange. WebServices. Data. ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="47f6f-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="47f6f-149">Encontre o ponto de extremidade correto usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="47f6f-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="47f6f-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="47f6f-150"><a name="bk_Managed"> </a></span></span>

<span data-ttu-id="47f6f-151">Se você estiver usando a API gerenciada do EWS, as chamadas para o serviço de descoberta automática serão tratadas pela classe **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="47f6f-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="47f6f-152">Para determinar o ponto de extremidade correto para uma conta de email, chame o método **AutodiscoverUrl** em um objeto **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="47f6f-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="47f6f-153">O exemplo de código a seguir mostra como definir o ponto de extremidade do serviço Web EWS para um endereço de email para o arquivo Exchange. asmx no servidor de acesso para cliente correto usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="47f6f-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="47f6f-154">Encontre o ponto de extremidade correto usando o EWS</span><span class="sxs-lookup"><span data-stu-id="47f6f-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="47f6f-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="47f6f-155"><a name="bk_SOAP"> </a></span></span>

<span data-ttu-id="47f6f-156">O serviço de descoberta automática do SOAP pode usar uma série de solicitações e respostas para direcionar seu aplicativo para o ponto de extremidade correto do EWS.</span><span class="sxs-lookup"><span data-stu-id="47f6f-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="47f6f-157">Para obter informações sobre o processo para determinar o ponto de extremidade correto para uma conta de email, consulte [autodiscover for Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="47f6f-158">Os exemplos de XML a seguir mostram a série de solicitações e respostas que você pode esperar ao fazer uma solicitação de descoberta automática do SOAP para localizar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="47f6f-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="47f6f-159">Solicitação de ponto de extremidade de descoberta automática SOAP</span><span class="sxs-lookup"><span data-stu-id="47f6f-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="47f6f-160">O exemplo a seguir mostra uma solicitação XML que é enviada para o serviço de descoberta automática para localizar o ponto de extremidade correto.</span><span class="sxs-lookup"><span data-stu-id="47f6f-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="47f6f-161">Resposta de redirecionamento de descoberta automática SOAP</span><span class="sxs-lookup"><span data-stu-id="47f6f-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="47f6f-162">O serviço de descoberta automática pode responder com uma de duas respostas de redirecionamento: um HTTP 302 Redirect ou uma resposta de redirecionamento SOAP.</span><span class="sxs-lookup"><span data-stu-id="47f6f-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="47f6f-163">Se a resposta do servidor Exchange for um redirecionamento HTTP 302, o aplicativo cliente deverá validar que o endereço de redirecionamento é aceitável e, em seguida, seguir a resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="47f6f-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="47f6f-164">Para saber mais sobre como validar uma resposta de redirecionamento, confira [descoberta automática do Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47f6f-164">For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="47f6f-165">Se o serviço descoberta automática retornar uma resposta de redirecionamento, indicada pelo elemento [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento **userresponse** , seu aplicativo cliente deverá usar o elemento **RedirectTarget** para construir uma nova solicitação de configurações que será enviada ao servidor especificado na resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="47f6f-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="47f6f-166">O exemplo a seguir mostra uma resposta de redirecionamento do servidor.</span><span class="sxs-lookup"><span data-stu-id="47f6f-166">The following example shows a redirection response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="47f6f-167">Após um redirecionamento, o cliente usa a URL de redirecionamento para preparar outra solicitação.</span><span class="sxs-lookup"><span data-stu-id="47f6f-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="47f6f-168">O código a seguir mostra um exemplo da solicitação que você cria a partir da resposta de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="47f6f-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="47f6f-169">Quando o aplicativo cliente tiver sido direcionado para o ponto de extremidade correto para o serviço de descoberta automática, o servidor enviará uma resposta com o elemento [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento **userresponse** definido como **NOERROR** e que contém as configurações de usuário solicitadas.</span><span class="sxs-lookup"><span data-stu-id="47f6f-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="47f6f-170">Somente as configurações de usuário solicitadas, **InternalEwsUrl** e **ExternalEwsUrl**, são retornadas.</span><span class="sxs-lookup"><span data-stu-id="47f6f-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="47f6f-171">O exemplo a seguir mostra a resposta do servidor.</span><span class="sxs-lookup"><span data-stu-id="47f6f-171">The following example shows the response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

## <a name="next-steps"></a><span data-ttu-id="47f6f-172">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="47f6f-172">Next steps</span></span>
<span data-ttu-id="47f6f-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="47f6f-173"><a name="bk_Next"> </a></span></span>

<span data-ttu-id="47f6f-174">Localizar o ponto de extremidade seguindo o processo de descoberta automática retorna as configurações de domínio ou usuário solicitadas.</span><span class="sxs-lookup"><span data-stu-id="47f6f-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="47f6f-175">Para obter informações sobre como fazer uma solicitação para configurações específicas, consulte os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="47f6f-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="47f6f-176">Obter as configurações de domínio de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="47f6f-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)    
- [<span data-ttu-id="47f6f-177">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="47f6f-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="47f6f-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="47f6f-178">See also</span></span>

- [<span data-ttu-id="47f6f-179">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="47f6f-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="47f6f-180">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="47f6f-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="47f6f-181">Referência do serviço Web de descoberta automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="47f6f-181">Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [<span data-ttu-id="47f6f-182">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="47f6f-182">EWS reference for Exchange</span></span>](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

