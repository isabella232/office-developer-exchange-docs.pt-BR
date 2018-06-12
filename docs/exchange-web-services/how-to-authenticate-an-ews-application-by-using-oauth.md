---
title: Autenticar um aplicativo do EWS usando OAuth
manager: sethgros
ms.date: 1/15/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Saiba como usar a autenticação OAuth com seus aplicativos do EWS Managed API.
ms.openlocfilehash: 66bbc0525ecf78407e853da0c8dcdec92791ca56
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750687"
---
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Autenticar um aplicativo do EWS usando OAuth

Saiba como usar a autenticação OAuth com seus aplicativos do EWS Managed API.
  
Você pode usar o serviço de autenticação OAuth fornecido pelo Windows Azure Active Directory para integrar seus aplicativos do EWS Managed API com o mesmo modelo de autenticação usado pelas APIs do restante do Office 365. Para usar OAuth com seu aplicativo, que você precisará:
  
1. [Registre seu aplicativo](#bk_register) com o Windows Azure Active Directory. 
    
2. [Adicionar código para obter um token de autenticação](#bk_getToken) para obter uma autenticação de token de um servidor de token. 
    
3. [Adicionar um token de autenticação para solicitações EWS](#bk_useToken) que você enviar. 
    
> [!NOTE]
> Autenticação OAuth para EWS só está disponível no Exchange como parte do Office 365. Aplicativos de EWS exigem a permissão "Acesso total às caixas de correio do usuário". 
  
Para usar o código neste artigo, você precisará ter acesso ao seguinte:
  
- Uma [conta de desenvolvedor do Office 365](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx.aspx). Você pode usar uma conta de avaliação para testar seu aplicativo
    
- A [biblioteca de autenticação do Azure AD para .NET](http://msdn.microsoft.com/en-us/library/office/jj573266.aspx.aspx).
    
- [API gerenciada do EWS](https://github.com/officedev/ews-managed-api.aspx).

<a name="bk_register"> </a>

## <a name="register-your-application"></a>Registre seu aplicativo

Para usar OAuth, um aplicativo deve ter um identificador de cliente e um URI que identifica o aplicativo do aplicativo. Se você ainda não registrou seu aplicativo com serviços do Azure Active Directory, você precisará adicionar manualmente o seu aplicativo seguindo as etapas em [registrar você aplicativo](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx).

<a name="bk_getToken"> </a>

## <a name="add-code-to-get-an-authentication-token"></a>Adicionar código para obter um token de autenticação

Biblioteca de autenticação de AD do Windows Azure para .NET simplifica a obtenção de um token de autenticação do Windows Azure Active Directory para que você possa usar o token em seu aplicativo. Você precisa fornecer quatro partes de informações para obter o token:
  
1. O URI do servidor de token. O servidor de token é a **autoridade** que autentica o usuário e retorna um token que seu aplicativo pode usar para acessar o EWS. 
    
2. A ID do aplicativo cliente criada quando você registrou seu aplicativo com o Windows Azure Active Directory.
    
3. O cliente do aplicativo URI criado quando você registrou seu aplicativo com o Windows Azure Active Directory.
    
4. O URI do servidor EWS e o URI do ponto de extremidade do EWS. Para o Exchange como parte do Office 365, este será `https://<server name>/ews/exchange.asmx`.
    
O código a seguir mostra como usar a biblioteca de autenticação do Windows Azure AD para obter um token de autenticação. Ele pressupõe que as informações necessárias para fazer a solicitação de autenticação são armazenadas no arquivo de App. config do aplicativo. Este exemplo não incluem a verificação de erros, consulte o [exemplo de código](#bk_codeSample) para o código completo. 
  
```cs
string authority = ConfigurationManager.AppSettings["authority"];
string clientID = ConfigurationManager.AppSettings["clientID"];
Uri clientAppUri = new Uri(ConfigurationManager.AppSettings["clientAppUri"];
string serverName = ConfigurationManager.AppSettings["serverName"];
AuthenticationContext authenticationContext = new AuthenticationContext(authority, false);
AuthenticationResult authenticationResult = authenticationContext.AcquireToken(serverName, clientId, clientAppUri);

```

<a name="bk_useToken"> </a>

## <a name="add-an-authentication-token-to-ews-requests"></a>Adicionar um token de autenticação às solicitações EWS

Depois que você recebeu o objeto **AuthenticationResult** que você pode usar a propriedade **AccessToken** para obter o token emitido pelo serviço de token. 
  
```cs
ExchangeService exchangeService = new ExchangeService(ExchangeVersion.Exchange2013);
exchangeService.Url = new Uri(ConfigurationManager.AppSettings["serverName"]+"ews/exchange.asmx");
exchangeService.TraceEnabled = true;
exchangeService.TraceFlags = TraceFlags.All;
exchangeService.Credentials = new OAuthCredentials(authenticationResult.AccessToken));
exchangeService.FindFolders(WellKnownFolderName.Root, new Folderview(10));
```

<a name="bk_codeSample"> </a>

## <a name="code-sample"></a>Exemplo de código

A seguir está um exemplo de código completo que demonstra como fazer uma solicitação de autenticação OAuth EWS.
  
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

O código de exemplo requer um arquivo App. config com as seguintes entradas:
  
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

## <a name="see-also"></a>Confira também

- [Autenticação e EWS no Exchange](authentication-and-ews-in-exchange.md)    
- [Testar e implantar aplicativos do Office 365](http://msdn.microsoft.com/en-us/office/office365/howto/test-and-deploy-apps.aspx)
    

