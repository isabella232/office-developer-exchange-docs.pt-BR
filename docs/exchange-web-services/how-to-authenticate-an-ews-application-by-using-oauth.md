---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 795cbcc3dd1c895850086ebf0e23da905c1c99b7
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254962"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Autenticar um aplicativo EWS usando o OAuth
<!-- markdownlint-enable MD025 -->

Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.

Você pode usar o serviço de autenticação OAuth fornecido com o Azure Active Directory para permitir que os aplicativos da API gerenciada EWS acessem o Exchange Online no Office 365. Para usar o OAuth com o aplicativo, você precisará:

1. [Registrar o aplicativo](#register-your-application) com o Azure Active Directory.

2. [Adicione um código para obter um token de autenticação](#add-code-to-get-an-authentication-token) de um servidor de token.

3. [Adicione um token de autenticação a solicitações do EWS](#add-an-authentication-token-to-ews-requests) que você enviar.

> [!NOTE]
> A autenticação OAuth para o EWS só está disponível no Exchange como parte do Office 365. Os aplicativos do EWS que usam o OAuth devem ser registrados com o Azure Active Directory.

Para usar o código desse artigo, você precisará ter acesso ao seguinte:

- Uma conta do Office 365 com uma caixa de correio do Exchange Online. Se você não tiver uma conta do Office 365, você pode [inscrever-se no programa para desenvolvedores do Office 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Office 365.

- A [biblioteca de autenticação da Microsoft para .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).

- A [API gerenciada do EWS](https://github.com/officedev/ews-managed-api).


Existem dois tipos de permissões OAuth que podem ser usadas para acessar as APIs do EWS no Exchange Online. Antes de prosseguir com o tutorial, você precisará escolher o tipo de permissão que deseja usar.

* As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente. Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo pode agir como o usuário conectado ao fazer chamadas API. 
* As **permissões de aplicativo** são usadas pelos aplicativos que são executados sem um usuário conectado. Por exemplo, aplicativos executados em segundo plano ou como daemons e podem acessar várias caixas de correio.

## <a name="register-your-application"></a>Registre seu aplicativo

Para usar o OAuth, um aplicativo deve ter uma ID de aplicativo emitida pelo Azure Active Directory. Neste tutorial, presume-se que o aplicativo seja um aplicativo de console, para que você precise registrá-lo como um cliente público com o Azure Active Directory.

1. Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta da Microsoft) ou **Conta Corporativa ou de Estudante**.

1. Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.

1. Selecione **Novo registro**. Na página **Registrar um aplicativo**, defina os valores da seguinte forma.

    - Defina **Nome** como um nome amigável para o seu aplicativo.
    - Defina **tipos de conta com suporte** como a opção que faz sentido para o seu cenário.
    - Para a **URI de redirecionamento**, altere a lista suspensa para **cliente público (móvel e área de trabalho)** e defina o valor para `urn:ietf:wg:oauth:2.0:oob`.

1. Escolha **Registrar**. Na página seguinte, copie e salve o valor da **ID do aplicativo (cliente)**, você precisará dele na próxima etapa.

1. Selecione **Permissões de API** na navegação à esquerda em **Gerenciar**. 

1. Selecione **Adicionar uma permissão**. Na página **Solicitar permissões da API**, selecione **Exchange**em **APIs herdadas com suporte**. 

1. Para usar permissões delegadas, selecione **Permissões delegadas** e, em seguida, selecione **EWS.AccessAsUser.All** em **EWS**. Clique em **Adicionar permissões**. 

Para usar as permissões do aplicativo, siga estas etapas.

1. Marque **permissões do aplicativo** e, em seguida, selecione **full_access_as_app**. Clique em **Adicionar permissões**.

1. Selecione **Conceder consentimento de administrador para a organização** e aceite o diálogo de consentimento. 

1. Selecione **Certificados e segredos** na navegação à esquerda em **Gerenciar**. 

1. Selecione **Novo segredo do cliente**, insira uma breve descrição e selecione **Adicionar**.

1. Copie e salve o **valor** do segredo do cliente recém-adicionado, você precisará dele mais tarde. 

## <a name="add-code-to-get-an-authentication-token"></a>Adicionar código para obter um token de autenticação

Os trechos de código a seguir mostram como usar a biblioteca de autenticação da Microsoft para obter tokens de autenticação para permissões delegadas e permissões de aplicativo. Esses trechos presumem que as informações necessárias para fazer a solicitação de autenticação sejam armazenadas no arquivo **App.config** do aplicativo. Esses exemplos não incluem a verificação de erros, confira o [exemplos de códigos](#code-samples) para o código completo.

### <a name="delegated-permissions"></a>Permissões delegadas

```cs
// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="application-permissions"></a>Permissões de aplicativos

```cs
// Configure the MSAL client to get tokens
var app = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"]).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/.default" };

//Make the token request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a>Adicione um token de autenticação a solicitações do EWS.

Depois de receber o objeto**AuthenticationResult**, você pode usar a propriedade **AcessToken** para obter o token emitido pelo serviço de token.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Para usar as permissões do aplicativo, você também precisará explicitamente representar uma caixa de correio que você deseja acessar. 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Exemplos de código

### <a name="delegated-permissions"></a>Permissões delegadas

A seguir, exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando permissões delegadas.

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }

        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

            try
            {
                // Make the interactive token request
                var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

### <a name="application-permissions"></a>Permissões de aplicativos

A seguir, um exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando permissões de aplicativo.

> [!NOTE]
> Ao usar a representação, você sempre deve usar o cabeçalho da solicitação X-AnchorMailbox, que deve ser definido como o SMTP da caixa de correio representada.

```cs
using System;
using System.Configuration;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;

namespace ews_oauth_samples
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
        
        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var ewsScopes = new string[] { "https://outlook.office.com/.default" };

            var app = ConfidentialClientApplicationBuilder.Create(ConfigurationManager.AppSettings["appId"])
                .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .Build();

            AuthenticationResult result = null;

            try
            {
                // Make the interactive token request
                result = await app.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(result.AccessToken);

                //Impersonate the mailbox you'd like to access.
                ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "test@demotenant.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach (var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

O código de exemplo em ambos os casos exige um arquivo **App.config** com as seguintes entradas:

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>Confira também

- [Autenticação e EWS no Exchange](authentication-and-ews-in-exchange.md)
