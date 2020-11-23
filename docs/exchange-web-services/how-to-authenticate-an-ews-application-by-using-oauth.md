---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 11/19/2020
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: c52b254f14cadd287a709bb68f8464e7cfe1837a
ms.sourcegitcommit: 2d16ba247a8cb4b6c8ca9941cb079f75202aae1e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49356490"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="190fc-103">Autenticar um aplicativo EWS usando o OAuth</span><span class="sxs-lookup"><span data-stu-id="190fc-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="190fc-104">Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="190fc-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="190fc-105">Você pode usar o serviço de autenticação OAuth fornecido com o Azure Active Directory para permitir que os aplicativos da API gerenciada EWS acessem o Exchange Online no Office 365.</span><span class="sxs-lookup"><span data-stu-id="190fc-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="190fc-106">Para usar o OAuth com o aplicativo, você precisará:</span><span class="sxs-lookup"><span data-stu-id="190fc-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="190fc-107">[Registrar o aplicativo](#register-your-application) com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="190fc-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="190fc-108">[Adicione um código para obter um token de autenticação](#add-code-to-get-an-authentication-token) de um servidor de token.</span><span class="sxs-lookup"><span data-stu-id="190fc-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>
1. <span data-ttu-id="190fc-109">[Adicione um token de autenticação a solicitações do EWS](#add-an-authentication-token-to-ews-requests) que você enviar.</span><span class="sxs-lookup"><span data-stu-id="190fc-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="190fc-110">A autenticação OAuth para o EWS só está disponível no Exchange Online como parte do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="190fc-110">OAuth authentication for EWS is only available in Exchange Online as part of Microsoft 365.</span></span> <span data-ttu-id="190fc-111">Os aplicativos do EWS que usam o OAuth devem ser registrados com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="190fc-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="190fc-112">Para usar o código desse artigo, você precisará ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="190fc-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="190fc-113">Uma conta do Microsoft 365 com uma caixa de correio do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="190fc-113">A Microsoft 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="190fc-114">Se você não tiver uma conta do Microsoft 365, poderá [inscrever-se no programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program) para obter uma assinatura gratuita do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="190fc-114">If you do not have a Microsoft 365 account, you can [sign up for the Microsoft 365 Developer Program](https://developer.microsoft.com/microsoft-365/dev-program) to get a free Microsoft 365 subscription.</span></span>
- <span data-ttu-id="190fc-115">A [biblioteca de autenticação da Microsoft para .NET](/dotnet/api/microsoft.identity.client).</span><span class="sxs-lookup"><span data-stu-id="190fc-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client).</span></span>
- <span data-ttu-id="190fc-116">A [API gerenciada do EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="190fc-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>

<span data-ttu-id="190fc-117">Existem dois tipos de permissões OAuth que podem ser usadas para acessar as APIs do EWS no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="190fc-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="190fc-118">Antes de prosseguir com o tutorial, você precisará escolher o tipo de permissão que deseja usar.</span><span class="sxs-lookup"><span data-stu-id="190fc-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

- <span data-ttu-id="190fc-119">As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente.</span><span class="sxs-lookup"><span data-stu-id="190fc-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="190fc-120">Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo pode agir como o usuário conectado ao fazer chamadas API.</span><span class="sxs-lookup"><span data-stu-id="190fc-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span>
- <span data-ttu-id="190fc-121">As **permissões de aplicativo** são usadas pelos aplicativos que são executados sem um usuário conectado. Por exemplo, aplicativos executados em segundo plano ou como daemons e podem acessar várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="190fc-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="190fc-122">Registre seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="190fc-122">Register your application</span></span>

<span data-ttu-id="190fc-123">Para usar o OAuth, um aplicativo deve ter uma ID de aplicativo emitida pelo Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="190fc-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="190fc-124">Neste tutorial, presume-se que o aplicativo seja um aplicativo de console, então você precisa registrá-lo como um cliente público com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="190fc-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span> <span data-ttu-id="190fc-125">Você pode registrar um aplicativo no centro de administração do Azure Active Directory ou usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="190fc-125">You can register an application in the Azure Active Directory admin center or by using Microsoft Graph.</span></span>

1. <span data-ttu-id="190fc-126">Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta Microsoft) ou **Conta Corporativa ou de Estudante**.</span><span class="sxs-lookup"><span data-stu-id="190fc-126">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="190fc-127">Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-127">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="190fc-128">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="190fc-128">Select **New registration**.</span></span> <span data-ttu-id="190fc-129">Na página **Registrar um aplicativo**, defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="190fc-129">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="190fc-130">Defina **Nome** como um nome amigável para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="190fc-130">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="190fc-131">Defina **tipos de conta com suporte** como a opção que faz sentido para o seu cenário.</span><span class="sxs-lookup"><span data-stu-id="190fc-131">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="190fc-132">Para a **URI de redirecionamento**, altere a lista suspensa para **cliente público (móvel e área de trabalho)** e defina o valor para `urn:ietf:wg:oauth:2.0:oob`.</span><span class="sxs-lookup"><span data-stu-id="190fc-132">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="190fc-133">Escolha **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-133">Choose **Register**.</span></span> <span data-ttu-id="190fc-134">Na página seguinte, copie os valores da **ID do aplicativo (cliente)** e da **ID do diretório (locatário)** e salve-os; você precisará deles mais tarde.</span><span class="sxs-lookup"><span data-stu-id="190fc-134">On the next page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them, you will need them later.</span></span>

### <a name="configure-for-delegated-authentication"></a><span data-ttu-id="190fc-135">Configurar para uma autenticação delegada</span><span class="sxs-lookup"><span data-stu-id="190fc-135">Configure for delegated authentication</span></span>

<span data-ttu-id="190fc-136">Se o aplicativo usar autenticação delegada, nenhuma configuração adicional será necessária.</span><span class="sxs-lookup"><span data-stu-id="190fc-136">If your application uses delegated authentication, no further configuration is required.</span></span> <span data-ttu-id="190fc-137">A [Plataforma de identidade da Microsoft] permite aos aplicativos solicitar permissões de forma dinâmica, para que você não precise pré-configurar permissões no registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="190fc-137">The [Microsoft identity platform] allows apps to request permissions dynamically, so you do not have to pre-configure permissions on the app registration.</span></span> <span data-ttu-id="190fc-138">No entanto, em alguns cenários (como o de [em nome do fluxo](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) é necessário pré-configurar permissões.</span><span class="sxs-lookup"><span data-stu-id="190fc-138">However, in some scenarios (like the [on-behalf-of flow](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)) pre-configuring permissions is required.</span></span> <span data-ttu-id="190fc-139">Use as etapas a seguir para pré-configurar as permissões EWS.</span><span class="sxs-lookup"><span data-stu-id="190fc-139">Use the following steps to pre-configure EWS permissions.</span></span>

1. <span data-ttu-id="190fc-140">Selecione **Manifesto** na navegação à esquerda em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-140">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="190fc-141">Localize a propriedade `requiredResourceAccess` no manifesto e adicione o seguinte dentro dos colchetes (`[]`):</span><span class="sxs-lookup"><span data-stu-id="190fc-141">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

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

1. <span data-ttu-id="190fc-142">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-142">Select **Save**.</span></span>

1. <span data-ttu-id="190fc-143">Selecione **Permissões de API** em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-143">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="190fc-144">Confirme se a permissão **EWS.AccessAsUser.All** está listada.</span><span class="sxs-lookup"><span data-stu-id="190fc-144">Confirm that the **EWS.AccessAsUser.All** permission is listed.</span></span>

### <a name="configure-for-app-only-authentication"></a><span data-ttu-id="190fc-145">Configuração de autenticação somente para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="190fc-145">Configure for app-only authentication</span></span>

<span data-ttu-id="190fc-146">Para usar as permissões do aplicativo, siga estas etapas adicionais.</span><span class="sxs-lookup"><span data-stu-id="190fc-146">To use application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="190fc-147">Selecione **Manifesto** na navegação à esquerda em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-147">Select **Manifest** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="190fc-148">Localize a propriedade `requiredResourceAccess` no manifesto e adicione o seguinte dentro dos colchetes (`[]`):</span><span class="sxs-lookup"><span data-stu-id="190fc-148">Locate the `requiredResourceAccess` property in the manifest, and add the following inside the square brackets (`[]`):</span></span>

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

1. <span data-ttu-id="190fc-149">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-149">Select **Save**.</span></span>

1. <span data-ttu-id="190fc-150">Selecione **Permissões de API** em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-150">Select **API permissions** under **Manage**.</span></span> <span data-ttu-id="190fc-151">Verifique se a permissão **full_access_as_app** está listada.</span><span class="sxs-lookup"><span data-stu-id="190fc-151">Confirm that the **full_access_as_app** permission is listed.</span></span>

1. <span data-ttu-id="190fc-152">Selecione **Conceder consentimento de administrador para a organização** e aceite o diálogo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="190fc-152">Select **Grant admin consent for org** and accept the consent dialog.</span></span>

1. <span data-ttu-id="190fc-153">Selecione **Certificados e segredos** na navegação à esquerda em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-153">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span>

1. <span data-ttu-id="190fc-154">Selecione **Novo segredo do cliente**, insira uma breve descrição e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="190fc-154">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="190fc-155">Copie e salve o **valor** do segredo do cliente recém-adicionado, você precisará dele mais tarde.</span><span class="sxs-lookup"><span data-stu-id="190fc-155">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span>

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="190fc-156">Adicionar código para obter um token de autenticação</span><span class="sxs-lookup"><span data-stu-id="190fc-156">Add code to get an authentication token</span></span>

<span data-ttu-id="190fc-157">Os trechos de código a seguir mostram como usar a biblioteca de autenticação da Microsoft para obter tokens de autenticação para permissões delegadas e permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="190fc-157">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="190fc-158">Esses trechos presumem que as informações necessárias para fazer a solicitação de autenticação sejam armazenadas no arquivo **App.config** do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="190fc-158">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="190fc-159">Esses exemplos não incluem a verificação de erros, confira os [Exemplos de códigos](#code-samples) para o código completo.</span><span class="sxs-lookup"><span data-stu-id="190fc-159">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="get-a-token-with-delegated-auth"></a><span data-ttu-id="190fc-160">Obter um token com autenticação delegada</span><span class="sxs-lookup"><span data-stu-id="190fc-160">Get a token with delegated auth</span></span>

```cs
// Using Microsoft.Identity.Client 4.22.0
var pca = PublicClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="get-a-token-with-app-only-auth"></a><span data-ttu-id="190fc-161">Obter um token com autenticação somente para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="190fc-161">Get a token with app-only auth</span></span>

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
var authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();
```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="190fc-162">Adicionar um token de autenticação a solicitações do EWS</span><span class="sxs-lookup"><span data-stu-id="190fc-162">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="190fc-163">Depois de receber o objeto **AuthenticationResult**, você pode usar a propriedade **AcessToken** para obter o token emitido pelo serviço de token.</span><span class="sxs-lookup"><span data-stu-id="190fc-163">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="190fc-164">Para usar as permissões do aplicativo, você também precisará explicitamente representar uma caixa de correio que deseja acessar.</span><span class="sxs-lookup"><span data-stu-id="190fc-164">To use application permissions, you will also need to explicitly impersonate a mailbox that you would like to access.</span></span>

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="190fc-165">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="190fc-165">Code samples</span></span>

### <a name="delegated-authentication"></a><span data-ttu-id="190fc-166">Autenticação delegada</span><span class="sxs-lookup"><span data-stu-id="190fc-166">Delegated authentication</span></span>

<span data-ttu-id="190fc-167">A seguir, um exemplo de código completo que demonstra a realização de uma solicitação do EWS autenticada pelo OAuth usando autenticação delegada.</span><span class="sxs-lookup"><span data-stu-id="190fc-167">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using delegated authentication.</span></span>

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
            var pca = PublicClientApplicationBuilder
                .Create(ConfigurationManager.AppSettings["appId"])
                .Build();

            var ewsScopes = new string[] { "EWS.AccessAsUser.All" };

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

### <a name="app-only-authentication"></a><span data-ttu-id="190fc-168">Autenticação somente para o aplicativo</span><span class="sxs-lookup"><span data-stu-id="190fc-168">App-only authentication</span></span>

<span data-ttu-id="190fc-169">A seguir, um exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando autenticação somente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="190fc-169">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using app-only authentication.</span></span>

> [!NOTE]
> <span data-ttu-id="190fc-170">Ao usar a representação, você sempre deve usar o cabeçalho de solicitação X-AnchorMailbox, que deve ser definido como o SMTP da caixa de correio representada.</span><span class="sxs-lookup"><span data-stu-id="190fc-170">When using impersonation you must always use the X-AnchorMailbox request header, which should be set to the SMTP address of the impersonated mailbox.</span></span>

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

<span data-ttu-id="190fc-171">O código de exemplo em ambos os casos exige um arquivo **App.config** com as seguintes entradas:</span><span class="sxs-lookup"><span data-stu-id="190fc-171">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

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

## <a name="see-also"></a><span data-ttu-id="190fc-172">Confira também</span><span class="sxs-lookup"><span data-stu-id="190fc-172">See also</span></span>

- [<span data-ttu-id="190fc-173">Autenticação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="190fc-173">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
