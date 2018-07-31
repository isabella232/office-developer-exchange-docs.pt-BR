---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Saiba como usar a autenticação OAuth com seus aplicativos do EWS Managed API.
ms.openlocfilehash: 8b6a3fd72e42a36e31f261205292de28ef341270
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353578"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="a90ea-103">Autenticar um aplicativo EWS usando o OAuth</span><span class="sxs-lookup"><span data-stu-id="a90ea-103">Authenticate an EWS application by using OAuth</span></span>

<span data-ttu-id="a90ea-104">Saiba como usar a autenticação OAuth com seus aplicativos do EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="a90ea-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>
  
<span data-ttu-id="a90ea-105">Você pode usar o serviço de autenticação OAuth fornecido pelo Windows Azure Active Directory para integrar seus aplicativos do EWS Managed API com o mesmo modelo de autenticação usado pelas APIs do restante do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a90ea-105">You can use the OAuth authentication service provided by Azure Active Directory to integrate your EWS Managed API applications with the same authentication model used by the Office 365 REST APIs.</span></span> <span data-ttu-id="a90ea-106">Para usar OAuth com seu aplicativo, que você precisará:</span><span class="sxs-lookup"><span data-stu-id="a90ea-106">To use OAuth with your application you will need to:</span></span>
  
1. <span data-ttu-id="a90ea-107">[Registre seu aplicativo](#bk_register) com o Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a90ea-107">[Register your application](#bk_register) with Azure Active Directory.</span></span> 
    
2. <span data-ttu-id="a90ea-108">[Adicionar código para obter um token de autenticação](#bk_getToken) para obter uma autenticação de token de um servidor de token.</span><span class="sxs-lookup"><span data-stu-id="a90ea-108">[Add code to get an authentication token](#bk_getToken) to get an authentication token from a token server.</span></span> 
    
3. <span data-ttu-id="a90ea-109">[Adicionar um token de autenticação para solicitações EWS](#bk_useToken) que você enviar.</span><span class="sxs-lookup"><span data-stu-id="a90ea-109">[Add an authentication token to EWS requests](#bk_useToken) that you send.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a90ea-110">Autenticação OAuth para EWS só está disponível no Exchange como parte do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a90ea-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="a90ea-111">Aplicativos de EWS exigem a permissão "Acesso total às caixas de correio do usuário".</span><span class="sxs-lookup"><span data-stu-id="a90ea-111">EWS applications require the "Full access to user's mailbox" permission.</span></span> 
  
<span data-ttu-id="a90ea-112">Para usar o código neste artigo, você precisará ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="a90ea-112">To use the code in this article, you will need to have access to the following:</span></span>
  
- <span data-ttu-id="a90ea-113">Uma [conta de desenvolvedor do Office 365](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span><span class="sxs-lookup"><span data-stu-id="a90ea-113">An [Office 365 developer account](https://docs.microsoft.com/en-us/office/developer-program/office-365-developer-program).</span></span> <span data-ttu-id="a90ea-114">Você pode usar uma conta de avaliação para testar seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a90ea-114">You can use a trial account to test your application.</span></span>
    
- <span data-ttu-id="a90ea-115">A [biblioteca de autenticação do Azure AD para .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span><span class="sxs-lookup"><span data-stu-id="a90ea-115">The [Azure AD Authentication Library for .NET](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-libraries).</span></span>
    
- <span data-ttu-id="a90ea-116">[API gerenciada do EWS](https://github.com/officedev/ews-managed-api.aspx).</span><span class="sxs-lookup"><span data-stu-id="a90ea-116">[The EWS Managed API](https://github.com/officedev/ews-managed-api.aspx).</span></span>

<span data-ttu-id="a90ea-117"><a name="bk_register"> </a></span><span class="sxs-lookup"><span data-stu-id="a90ea-117"></span></span>

## <a name="register-your-application"></a><span data-ttu-id="a90ea-118">Registre seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="a90ea-118">Register your application</span></span>

<span data-ttu-id="a90ea-119">Para usar OAuth, um aplicativo deve ter um identificador de cliente e um URI que identifica o aplicativo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a90ea-119">To use OAuth, an application must have a client identifier and an application URI that identifies the application.</span></span> <span data-ttu-id="a90ea-120">Se você ainda não registrou seu aplicativo com serviços do Azure Active Directory, você precisará adicionar manualmente o seu aplicativo seguindo as etapas em [registrar seu aplicativo](https://apps.dev.microsoft.com/#/appList).</span><span class="sxs-lookup"><span data-stu-id="a90ea-120">If you have not yet registered your application with Azure Active Directory Services, you'll need to manually add your application by following the steps at [Register your app](https://apps.dev.microsoft.com/#/appList).</span></span>

<span data-ttu-id="a90ea-121"><a name="bk_getToken"> </a></span><span class="sxs-lookup"><span data-stu-id="a90ea-121"></span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="a90ea-122">Adicionar código para obter um token de autenticação</span><span class="sxs-lookup"><span data-stu-id="a90ea-122">Add code to get an authentication token</span></span>

<span data-ttu-id="a90ea-123">Biblioteca de autenticação de AD do Windows Azure para .NET simplifica a obtenção de um token de autenticação do Windows Azure Active Directory para que você possa usar o token em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a90ea-123">The Azure AD Authentication Library for .NET simplifies getting an authentication token from Azure Active Directory so that you can use the token in your application.</span></span> <span data-ttu-id="a90ea-124">Você precisa fornecer quatro partes de informações para obter o token:</span><span class="sxs-lookup"><span data-stu-id="a90ea-124">You need to provide four pieces of information to get the token:</span></span>
  
1. <span data-ttu-id="a90ea-125">O URI do servidor de token.</span><span class="sxs-lookup"><span data-stu-id="a90ea-125">The URI of the token server.</span></span> <span data-ttu-id="a90ea-126">O servidor de token é a **autoridade** que autentica o usuário e retorna um token que seu aplicativo pode usar para acessar o EWS.</span><span class="sxs-lookup"><span data-stu-id="a90ea-126">The token server is the **authority** that authenticates the user and returns a token that your application can use to access EWS.</span></span> 
    
2. <span data-ttu-id="a90ea-127">A ID do aplicativo cliente criada quando você registrou seu aplicativo com o Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a90ea-127">The application client ID created when you registered your application with Azure Active Directory.</span></span>
    
3. <span data-ttu-id="a90ea-128">O cliente do aplicativo URI criado quando você registrou seu aplicativo com o Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a90ea-128">The application client URI created when you registered your application with Azure Active Directory.</span></span>
    
4. <span data-ttu-id="a90ea-129">O URI do servidor EWS e o URI do ponto de extremidade do EWS.</span><span class="sxs-lookup"><span data-stu-id="a90ea-129">The URI of the EWS server and the URI of the EWS endpoint.</span></span> <span data-ttu-id="a90ea-130">Para o Exchange como parte do Office 365, este será `https://<server name>/ews/exchange.asmx`.</span><span class="sxs-lookup"><span data-stu-id="a90ea-130">For Exchange as part of Office 365, this will be  `https://<server name>/ews/exchange.asmx`.</span></span>
    
<span data-ttu-id="a90ea-131">O código a seguir mostra como usar a biblioteca de autenticação do Windows Azure AD para obter um token de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a90ea-131">The following code shows how to use the Azure AD Authentication Library to get an authentication token.</span></span> <span data-ttu-id="a90ea-132">Ele pressupõe que as informações necessárias para fazer a solicitação de autenticação são armazenadas no arquivo de App. config do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a90ea-132">It assumes that the information required to make the authentication request is stored in the application's App.config file.</span></span> <span data-ttu-id="a90ea-133">Este exemplo não incluem a verificação de erros, consulte o [exemplo de código](#bk_codeSample) para o código completo.</span><span class="sxs-lookup"><span data-stu-id="a90ea-133">This example does not include error checking, see the [Code sample](#bk_codeSample) for the complete code.</span></span> 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<span data-ttu-id="a90ea-134"><a name="bk_useToken"> </a></span><span class="sxs-lookup"><span data-stu-id="a90ea-134"></span></span>

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="a90ea-135">Adicionar um token de autenticação às solicitações EWS</span><span class="sxs-lookup"><span data-stu-id="a90ea-135">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="a90ea-136">Depois que você recebeu o objeto **AuthenticationResult** que você pode usar a propriedade **AccessToken** para obter o token emitido pelo serviço de token.</span><span class="sxs-lookup"><span data-stu-id="a90ea-136">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span> 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<span data-ttu-id="a90ea-137"><a name="bk_codeSample"> </a></span><span class="sxs-lookup"><span data-stu-id="a90ea-137"></span></span>

## <a name="code-sample"></a><span data-ttu-id="a90ea-138">Exemplo de código</span><span class="sxs-lookup"><span data-stu-id="a90ea-138">Code sample</span></span>

<span data-ttu-id="a90ea-139">A seguir está um exemplo de código completo que demonstra como fazer uma solicitação de autenticação OAuth EWS.</span><span class="sxs-lookup"><span data-stu-id="a90ea-139">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.Configuration;
using System.Globalization;
using System.Linq;
using System.Text;
using System.Threading;
using System.Threading.Tasks;
using System.Web.Script.Serialization;
using Microsoft.Exchange.WebServices.Autodiscover;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.IdentityModel.Clients.ActiveDirectory;
namespace TestV1App
{
    class Program
    {
        static void Main(string[] args)
        {
            var t = new Thread(Run);
            t.SetApartmentState(ApartmentState.STA);
            t.Start();
            t.Join();
        }
        static void Run()
        {
           string authority = ConfigurationManager.AppSettings["authority"];
           string clientID = ConfigurationManager.AppSettings["clientID"];
           Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
           string serverName = ConfigurationManager.AppSettings["serverName"];
            AuthenticationResult authenticationResult = null;
            AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
            
            string errorMessage = null;
            try
            {
                Console.WriteLine("Trying to acquire token");
                authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);
            }
                catch (AdalException ex)
            {
                errorMessage = ex.Message;
                if (ex.InnerException != null)
                {
                    errorMessage += "\nInnerException : " + ex.InnerException.Message;
                }
            }
            catch (ArgumentException ex)
            {
                errorMessage = ex.Message;
            }
            if (!string.IsNullOrEmpty(errorMessage))
            {
                Console.WriteLine("Failed: {0}" + errorMessage);
                return;
            }
            Console.WriteLine("\nMaking the protocol call\n");
            ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
            exchangeService.Url = new Uri(resource + "ews/exchange.asmx");
            exchangeService.TraceEnabled = true;
            exchangeService.TraceFlags = TraceFlags.All;
            exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken);
            exchangeService.FindFolders(WellKnownFolderName.Root, new FolderView(10));
        }
    }
}

```

<span data-ttu-id="a90ea-140">O código de exemplo requer um arquivo App. config com as seguintes entradas:</span><span class="sxs-lookup"><span data-stu-id="a90ea-140">The sample code requires an App.config file with the following entries:</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.5" />
  </startup>
  <appSettings>
    <add key="authority" value="http://login.windows.net/<devAccountName>.onmicrosoft.com" />
    <add key="clientId" value="<ID generated by Azure Active Directory"/>
    <add key="clientAppUri" value="<URI registered with Azure Active Directory"/>
    <add key="serverName" value="outlook.office365.com" />
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="a90ea-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="a90ea-141">See also</span></span>

- [<span data-ttu-id="a90ea-142">Autenticação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a90ea-142">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)    

    

