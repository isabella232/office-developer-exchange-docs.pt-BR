---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 11/25/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: a7b1d2a099cf5f3c95f8453605363de12ff33c54
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603824"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a>Autenticar um aplicativo EWS usando o OAuth
<!-- markdownlint-enable MD025 -->

Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.

Você pode usar o serviço de autenticação OAuth fornecido com o Azure Active Directory para permitir que os aplicativos da API gerenciada EWS acessem o Exchange Online no Office 365. Para usar o OAuth com o aplicativo, você precisará:

1. [Registrar o aplicativo](#register-your-application) com o Azure Active Directory.
1. [Adicione um código para obter um token de autenticação](#add-code-to-get-an-authentication-token) de um servidor de token.
1. [Adicione um token de autenticação a solicitações do EWS](#add-an-authentication-token-to-ews-requests) que você enviar.

> [!NOTE]
> A autenticação OAuth para o EWS só está disponível no Exchange Online como parte do Microsoft 365. Os aplicativos do EWS que usam o OAuth devem ser registrados com o Azure Active Directory.

Para usar o código desse artigo, você precisará ter acesso ao seguinte:

- Uma conta do Microsoft 365 com uma caixa de correio do Exchange Online. Se você não tiver uma conta do Microsoft 365, poderá [inscrever-se no programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program) para obter uma assinatura gratuita do Microsoft 365.
- A [biblioteca de autenticação da Microsoft para .NET](/dotnet/api/microsoft.identity.client).
- A [API gerenciada do EWS](https://github.com/officedev/ews-managed-api).

Existem dois tipos de permissões OAuth que podem ser usadas para acessar as APIs do EWS no Exchange Online. Antes de prosseguir com o tutorial, você precisará escolher o tipo de permissão que deseja usar.

- As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente. Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo pode agir como o usuário conectado ao fazer chamadas API.
- As **permissões de aplicativo** são usadas pelos aplicativos que são executados sem um usuário conectado. Por exemplo, aplicativos executados em segundo plano ou como daemons e podem acessar várias caixas de correio.

## <a name="register-your-application"></a>Registre seu aplicativo

Para usar o OAuth, um aplicativo deve ter uma ID de aplicativo emitida pelo Azure Active Directory. Neste tutorial, presume-se que o aplicativo seja um aplicativo de console, para que você precise registrá-lo como um cliente público com o Azure Active Directory. Você pode registrar um aplicativo no centro de administração do Azure Active Directory ou usando o Microsoft Graph.

1. Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta da Microsoft) ou **Conta Corporativa ou de Estudante**.

1. Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.

1. Selecione **Novo registro**. Na página **Registrar um aplicativo**, defina os valores da seguinte forma.

    - Defina **Nome** como um nome amigável para o seu aplicativo.
    - Defina **tipos de conta com suporte** como a opção que faz sentido para o seu cenário.
    - Para a **URI de redirecionamento**, altere a lista suspensa para **cliente público (móvel e área de trabalho)** e defina o valor para `urn:ietf:wg:oauth:2.0:oob`.

1. Escolha **Registrar**. Na página seguinte, copie os valores da **ID do aplicativo (cliente)** e da **ID do diretório (locatário)** e salve-os; você precisará deles mais tarde.

### <a name="configure-for-delegated-authentication"></a>Configurar para uma autenticação delegada

Se o aplicativo usar autenticação delegada, nenhuma configuração adicional será necessária. A [plataforma de identidade para desenvolvedores da Microsoft](/azure/active-directory/develop/v2-overview) permite aos aplicativos solicitar permissões de forma dinâmica, para que você não precise pré-configurar permissões no registro do aplicativo. No entanto, em alguns cenários (como o de [em nome do fluxo](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) é necessário pré-configurar permissões. Use as etapas a seguir para pré-configurar as permissões EWS.

1. Selecione **Manifesto** na navegação à esquerda em **Gerenciar**.

1. Localize a propriedade `requiredResourceAccess` no manifesto e adicione o seguinte dentro dos colchetes (`[]`):

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "3b5f3d61-589b-4a3c-a359-5dd4b5ee5bd5",
                "type": "Scope"
            }
        ]
    }
    ```

1. Selecione **Salvar**.

1. Selecione **Permissões de API** em **Gerenciar**. Confirme se a permissão **EWS.AccessAsUser.All** está listada.

### <a name="configure-for-app-only-authentication"></a>Configuração de autenticação somente para o aplicativo

Para usar as permissões do aplicativo, siga estas etapas adicionais.

1. Selecione **Manifesto** na navegação à esquerda em **Gerenciar**.

1. Localize a propriedade `requiredResourceAccess` no manifesto e adicione o seguinte dentro dos colchetes (`[]`):

    ```json
    {
        "resourceAppId": "00000002-0000-0ff1-ce00-000000000000",
        "resourceAccess": [
            {
                "id": "dc890d15-9560-4a4c-9b7f-a736ec74ec40",
                "type": "Role"
            }
        ]
    }
    ```

1. Selecione **Salvar**.

1. Selecione **Permissões de API** em **Gerenciar**. Verifique se a permissão **full_access_as_app** está listada.

1. Selecione **Conceder consentimento de administrador para a organização** e aceite o diálogo de consentimento.

1. Selecione **Certificados e segredos** na navegação à esquerda em **Gerenciar**.

1. Selecione **Novo segredo do cliente**, insira uma breve descrição e selecione **Adicionar**.

1. Copie e salve o **valor** do segredo do cliente recém-adicionado, você precisará dele mais tarde.

## <a name="add-code-to-get-an-authentication-token"></a>Adicionar código para obter um token de autenticação

Os trechos de código a seguir mostram como usar a biblioteca de autenticação da Microsoft para obter tokens de autenticação para permissões delegadas e permissões de aplicativo. Esses trechos presumem que as informações necessárias para fazer a solicitação de autenticação sejam armazenadas no arquivo **App.config** do aplicativo. Esses exemplos não incluem a verificação de erros, confira o [exemplos de códigos](#code-samples) para o código completo.

### <a name="get-a-token-with-delegated-auth"></a>Obter um token com autenticação delegada

```cs
// Using Microsoft.Identity.Client 4.22.0

// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a>Obter um token com autenticação somente para o aplicativo

```cs
// Using Microsoft.Identity.Client 4.22.0
var cca = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
    .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

//Make the token request
var authResult = await cca.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a>Adicione um token de autenticação a solicitações do EWS.

Depois de receber o objeto **AuthenticationResult**, você pode usar a propriedade **AcessToken** para obter o token emitido pelo serviço de token.

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

Para usar as permissões do aplicativo, você também precisará explicitamente representar uma caixa de correio que deseja acessar.

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a>Exemplos de código

### <a name="delegated-authentication"></a>Autenticação delegada

A seguir, um exemplo de código completo que demonstra a realização de uma solicitação do EWS autenticada pelo OAuth usando autenticação delegada.

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0

            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            // The permission scope required for EWS access
            var ewsScopes = new string[] { "https://outlook.office365.com/EWS.AccessAsUser.All" };

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
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
    }
}
```

### <a name="app-only-authentication"></a>Autenticação somente para o aplicativo

A seguir, um exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando autenticação somente para o aplicativo.

> [!NOTE]
> Ao usar a representação, você sempre deve usar o cabeçalho de solicitação X-AnchorMailbox, que deve ser definido como o SMTP da caixa de correio representada.

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static async System.Threading.Tasks.Task Main(string[] args)
        {
            // Using Microsoft.Identity.Client 4.22.0
            var cca = ConfidentialClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .WithTenantId(ConfigurationManager.AppSettings["tenantId"])
                .Build();

            var ewsScopes = new string[] { "https://outlook.office365.com/.default" };

            try
            {
                var authResult = await cca.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
                ewsClient.ImpersonatedUserId =
                    new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "meganb@contoso.onmicrosoft.com");

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "meganb@contoso.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex}");
            }

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
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
    <!-- The tenant ID copied from your app registration -->
    <add key="tenantId" value="YOUR_TENANT_ID_HERE"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a>Confira também

- [Autenticação e EWS no Exchange](authentication-and-ews-in-exchange.md)
