---
title: Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth
description: Saiba como usar a autenticação OAuth com seus aplicativos IMAP, POP e SMTP.
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: f83a932790cde558e741ece1e87403103aff18fd
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012556"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a><span data-ttu-id="4b54e-103">Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth</span><span class="sxs-lookup"><span data-stu-id="4b54e-103">Authenticate an IMAP, POP or SMTP connection using OAuth</span></span>

<span data-ttu-id="4b54e-104">Saiba como usar a autenticação OAuth para se conectar com protocolos IMAP, POP ou SMTP e acessar dados de email para usuários do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4b54e-104">Learn how to use OAuth authentication to connect with IMAP, POP or SMTP protocols and access email data for Office 365 users.</span></span>

> <span data-ttu-id="4b54e-105">O suporte do OAuth2 para protocolos IMAP, POP, SMTP, conforme descrito abaixo, não tem suporte para usuários do Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="4b54e-105">OAuth2 support for IMAP, POP, SMTP protocols as described below is not supported for Outlook.com users.</span></span>

<span data-ttu-id="4b54e-106">Se você não estiver familiarizado com o OAuth 2,0, comece lendo a [visão geral da plataforma de identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="4b54e-106">If you're not familiar with OAuth 2.0, start by reading the [Microsoft identity platform (v2.0) overview](/azure/active-directory/develop/v2-overview).</span></span> <span data-ttu-id="4b54e-107">Esse documento apresenta a você diferentes componentes da plataforma de identidade da Microsoft, incluindo SDKs.</span><span class="sxs-lookup"><span data-stu-id="4b54e-107">That document introduces you to different components of Microsoft identity platform, including SDKs.</span></span>

<span data-ttu-id="4b54e-108">Você pode usar o serviço de autenticação OAuth fornecido pelo Azure Active Directory para permitir que seu aplicativo se conecte com protocolos IMAP, POP ou SMTP para acessar o Exchange Online no Office 365.</span><span class="sxs-lookup"><span data-stu-id="4b54e-108">You can use the OAuth authentication service provided by Azure Active Directory to enable your application to connect with IMAP, POP or SMTP protocols to access Exchange Online in Office 365.</span></span> <span data-ttu-id="4b54e-109">Para usar o OAuth com seu aplicativo, você precisa:</span><span class="sxs-lookup"><span data-stu-id="4b54e-109">To use OAuth with your application you need to:</span></span>

1. <span data-ttu-id="4b54e-110">[Registre seu aplicativo com o](#register-your-application) Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b54e-110">[Register your application](#register-your-application) with Azure Active Directory.</span></span>
1. <span data-ttu-id="4b54e-111">[Configure seu aplicativo](#configure-your-application) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b54e-111">[Configure your application](#configure-your-application) in Azure Active Directory.</span></span>
1. <span data-ttu-id="4b54e-112">[Obter um token de acesso](#get-an-access-token) de um servidor de token.</span><span class="sxs-lookup"><span data-stu-id="4b54e-112">[Get an access token](#get-an-access-token) from a token server.</span></span>
1. <span data-ttu-id="4b54e-113">[Autenticar solicitações de conexão](#authenticate-connection-requests) com um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="4b54e-113">[Authenticate connection requests](#authenticate-connection-requests) with an access token.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="4b54e-114">Registrar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b54e-114">Register your application</span></span>

<span data-ttu-id="4b54e-115">Para usar o OAuth, um aplicativo deve ser registrado no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b54e-115">To use OAuth, an application must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="4b54e-116">Siga as instruções listadas em [registrar um aplicativo com a plataforma de identidade da Microsoft](/azure/active-directory/develop/quickstart-register-app) para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b54e-116">Follow the instructions listed in [Register an application with the Microsoft identity platform](/azure/active-directory/develop/quickstart-register-app) to create a new application.</span></span>

## <a name="configure-your-application"></a><span data-ttu-id="4b54e-117">Configurar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b54e-117">Configure your application</span></span>

<span data-ttu-id="4b54e-118">Siga as instruções listadas em [configurar um aplicativo cliente para acessar as APIs da Web](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span><span class="sxs-lookup"><span data-stu-id="4b54e-118">Follow the instructions listed in [Configure a client application to access web APIs](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)</span></span>

<span data-ttu-id="4b54e-119">Certifique-se de adicionar um ou mais dos seguintes escopos de permissão que correspondem aos protocolos que você gostaria de integrar.</span><span class="sxs-lookup"><span data-stu-id="4b54e-119">Make sure to add one or more of the following permission scopes that correspond to the protocols you would like to integrate with.</span></span> <span data-ttu-id="4b54e-120">No assistente **Adicionar uma permissão** , selecione **Microsoft Graph** e, em seguida, **permissões delegadas** para localizar os seguintes escopos de permissão listados.</span><span class="sxs-lookup"><span data-stu-id="4b54e-120">In the **Add a permission** wizard, select **Microsoft Graph** and then **Delegated permissions** to find the following permission scopes listed.</span></span>

| <span data-ttu-id="4b54e-121">Protocolo</span><span class="sxs-lookup"><span data-stu-id="4b54e-121">Protocol</span></span>  | <span data-ttu-id="4b54e-122">Escopo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b54e-122">Permission scope</span></span>        |
|-----------|-------------------------|
| <span data-ttu-id="4b54e-123">IMAP</span><span class="sxs-lookup"><span data-stu-id="4b54e-123">IMAP</span></span>      | `IMAP.AccessAsUser.All` |
| <span data-ttu-id="4b54e-124">POP</span><span class="sxs-lookup"><span data-stu-id="4b54e-124">POP</span></span>       | `POP.AccessAsUser.All`  |
| <span data-ttu-id="4b54e-125">AUTENTICAÇÃO SMTP</span><span class="sxs-lookup"><span data-stu-id="4b54e-125">SMTP AUTH</span></span> | `SMTP.Send`             |

## <a name="get-an-access-token"></a><span data-ttu-id="4b54e-126">Obter um token de acesso</span><span class="sxs-lookup"><span data-stu-id="4b54e-126">Get an access token</span></span>

<span data-ttu-id="4b54e-127">Você pode usar uma de nossas [bibliotecas de cliente do MSAL](/azure/active-directory/develop/msal-overview) para buscar um token de acesso do aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b54e-127">You can use one of our [MSAL client libraries](/azure/active-directory/develop/msal-overview) to fetch an access token from your client application.</span></span>

<span data-ttu-id="4b54e-128">Como alternativa, você pode selecionar um fluxo apropriado da lista a seguir e seguir as etapas correspondentes para chamar as APIs REST da plataforma de identidade subjacente e recuperar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="4b54e-128">Alternatively, you can select an appropriate flow from the following list and follow the corresponding steps to call the underlying identity platform REST APIs and retrieve an access token.</span></span>

1. [<span data-ttu-id="4b54e-129">Fluxo de código de autorização OAuth2</span><span class="sxs-lookup"><span data-stu-id="4b54e-129">OAuth2 authorization code flow</span></span>](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [<span data-ttu-id="4b54e-130">Fluxo de concessão de autorização de dispositivo OAuth2</span><span class="sxs-lookup"><span data-stu-id="4b54e-130">OAuth2 Device authorization grant flow</span></span>](/azure/active-directory/develop/v2-oauth2-device-code)

<span data-ttu-id="4b54e-131">Não há suporte para o acesso OAuth a IMAP, POP, protocolos de autenticação SMTP por meio do fluxo de concessão de credenciais do cliente OAuth2.</span><span class="sxs-lookup"><span data-stu-id="4b54e-131">OAuth access to IMAP, POP, SMTP AUTH protocols via OAuth2 client credentials grant flow is not supported.</span></span> <span data-ttu-id="4b54e-132">Se seu aplicativo precisar de acesso persistente a todas as caixas de correio em uma organização do Microsoft 365, recomendamos que você use as APIs do Microsoft Graph que permitem o acesso sem um usuário, habilite permissões granulares e permita que o escopo de administradores desse acesso a um conjunto específico de caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="4b54e-132">If your application needs persistent access to all mailboxes in a Microsoft 365 organization, we recommend that you use the Microsoft Graph APIs which allow access without a user, enable granular permissions and let administrators scope such access to a specific set of mailboxes.</span></span>

<span data-ttu-id="4b54e-133">Certifique-se de especificar os escopos completos, incluindo URLs de recursos do Outlook, ao autorizar seu aplicativo e solicitar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="4b54e-133">Make sure to specify the full scopes, including Outlook resource URLs, when authorizing your application and requesting an access token.</span></span>

| <span data-ttu-id="4b54e-134">Protocolo</span><span class="sxs-lookup"><span data-stu-id="4b54e-134">Protocol</span></span>  | <span data-ttu-id="4b54e-135">Cadeia de caracteres de escopo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b54e-135">Permission scope string</span></span> |
|-----------|-------------------------|
| <span data-ttu-id="4b54e-136">IMAP</span><span class="sxs-lookup"><span data-stu-id="4b54e-136">IMAP</span></span>      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| <span data-ttu-id="4b54e-137">POP</span><span class="sxs-lookup"><span data-stu-id="4b54e-137">POP</span></span>       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| <span data-ttu-id="4b54e-138">AUTENTICAÇÃO SMTP</span><span class="sxs-lookup"><span data-stu-id="4b54e-138">SMTP AUTH</span></span> | `https://outlook.office.com/SMTP.Send`             |

<span data-ttu-id="4b54e-139">Além disso, você pode solicitar [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) escopo.</span><span class="sxs-lookup"><span data-stu-id="4b54e-139">In addition, you can request for [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) scope.</span></span> <span data-ttu-id="4b54e-140">Quando um usuário aprova o escopo de offline_access, seu aplicativo pode receber tokens de atualização do ponto de extremidade de token da plataforma de identidade da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4b54e-140">When a user approves the offline_access scope, your app can receive refresh tokens from the Microsoft identity platform token endpoint.</span></span> <span data-ttu-id="4b54e-141">Os tokens de atualização são de longa duração.</span><span class="sxs-lookup"><span data-stu-id="4b54e-141">Refresh tokens are long-lived.</span></span> <span data-ttu-id="4b54e-142">Seu aplicativo pode obter novos tokens de acesso com a expiração dos mais antigos.</span><span class="sxs-lookup"><span data-stu-id="4b54e-142">Your app can get new access tokens as older ones expire.</span></span>

## <a name="authenticate-connection-requests"></a><span data-ttu-id="4b54e-143">Autenticar solicitações de conexão</span><span class="sxs-lookup"><span data-stu-id="4b54e-143">Authenticate connection requests</span></span>

<span data-ttu-id="4b54e-144">Você pode iniciar uma conexão com os servidores de email do Office 365 usando as [configurações de email IMAP e pop para o Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span><span class="sxs-lookup"><span data-stu-id="4b54e-144">You can initiate a connection to Office 365 mail servers using the [IMAP and POP email settings for Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).</span></span>

### <a name="sasl-xoauth2"></a><span data-ttu-id="4b54e-145">XOAUTH2 SASL</span><span class="sxs-lookup"><span data-stu-id="4b54e-145">SASL XOAUTH2</span></span>

<span data-ttu-id="4b54e-146">A integração OAuth com exige que seu aplicativo use o formato SASL XOAUTH2 para codificar e transmitir o token de acesso.</span><span class="sxs-lookup"><span data-stu-id="4b54e-146">OAuth integration with requires your application to use SASL XOAUTH2 format for encoding and transmitting the access token.</span></span> <span data-ttu-id="4b54e-147">O SASL XOAUTH2 codifica o nome de usuário, o token de acesso em conjunto no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="4b54e-147">SASL XOAUTH2 encodes the username, access token together in the following format:</span></span>

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

<span data-ttu-id="4b54e-148">`^A`representa um **controle**  +  **a** ( `%x01` ).</span><span class="sxs-lookup"><span data-stu-id="4b54e-148">`^A` represents a **Control** + **A** (`%x01`).</span></span>

<span data-ttu-id="4b54e-149">Por exemplo, o formato SASL XOAUTH2 para acessar `test@contoso.onmicrosoft.com` com o token de acesso `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` é:</span><span class="sxs-lookup"><span data-stu-id="4b54e-149">For example, the SASL XOAUTH2 format to access `test@contoso.onmicrosoft.com` with access token `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` is:</span></span>

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

<span data-ttu-id="4b54e-150">Após a codificação Base64, isso é convertido para a cadeia de caracteres a seguir.</span><span class="sxs-lookup"><span data-stu-id="4b54e-150">After base64 encoding, this translates to the following string.</span></span> <span data-ttu-id="4b54e-151">Observe que as quebras de linha são inseridas para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="4b54e-151">Note that line breaks are inserted for readability.</span></span>

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a><span data-ttu-id="4b54e-152">Autenticação de XOAUTH2 do SASL para caixas de correio compartilhadas no Office 365</span><span class="sxs-lookup"><span data-stu-id="4b54e-152">SASL XOAUTH2 authentication for shared mailboxes in Office 365</span></span>

<span data-ttu-id="4b54e-153">No caso de acesso compartilhado de caixa de correio usando o OAuth, o aplicativo precisa obter o token de acesso em nome de um usuário, mas substituir o campo userName na cadeia de caracteres codificada XOAUTH2 do SASL pelo endereço de email da caixa de correio compartilhada.</span><span class="sxs-lookup"><span data-stu-id="4b54e-153">In case of shared mailbox access using OAuth, application needs to obtain the access token on behalf of a user but replace the userName field in the SASL XOAUTH2 encoded string with the email address of the shared mailbox.</span></span> 

### <a name="imap-protocol-exchange"></a><span data-ttu-id="4b54e-154">Intercâmbio de protocolo IMAP</span><span class="sxs-lookup"><span data-stu-id="4b54e-154">IMAP Protocol Exchange</span></span>

<span data-ttu-id="4b54e-155">Para autenticar uma conexão de servidor IMAP, o cliente terá que responder com um `AUTHENTICATE` comando no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="4b54e-155">To authenticate a IMAP server connection, the client will have to respond with an `AUTHENTICATE` command in the following format:</span></span>

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="4b54e-156">Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-156">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

<span data-ttu-id="4b54e-157">Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-157">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a><span data-ttu-id="4b54e-158">Troca de protocolo POP</span><span class="sxs-lookup"><span data-stu-id="4b54e-158">POP Protocol Exchange</span></span>

<span data-ttu-id="4b54e-159">Para autenticar uma conexão de servidor POP, o cliente terá que responder com um `AUTH` comando dividido em duas linhas no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="4b54e-159">To authenticate a POP server connection, the client will have to respond with an `AUTH` command split into two lines in the following format:</span></span>    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

<span data-ttu-id="4b54e-160">Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-160">Sample client-server message exchange that results in an authentication success:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYX   
JlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0  
Q2cBAQ==    
S: +OK User successfully authenticated. 
[connection continues...]   
``` 

<span data-ttu-id="4b54e-161">Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-161">Sample client-server message exchange that results in an authentication failure:</span></span>    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a><span data-ttu-id="4b54e-162">Troca de protocolo SMTP</span><span class="sxs-lookup"><span data-stu-id="4b54e-162">SMTP Protocol Exchange</span></span>

<span data-ttu-id="4b54e-163">Para autenticar uma conexão de servidor SMTP, o cliente terá que responder com um `AUTH` comando no seguinte formato:</span><span class="sxs-lookup"><span data-stu-id="4b54e-163">To authenticate a SMTP server connection, the client will have to respond with an `AUTH` command in the following format:</span></span>

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

<span data-ttu-id="4b54e-164">Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-164">Sample client-server message exchange that results in an authentication success:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 235 2.7.0 Authentication successful
[connection continues...]
```

<span data-ttu-id="4b54e-165">Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:</span><span class="sxs-lookup"><span data-stu-id="4b54e-165">Sample client-server message exchange that results in an authentication failure:</span></span>

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a><span data-ttu-id="4b54e-166">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4b54e-166">See also</span></span>

- [<span data-ttu-id="4b54e-167">Autenticação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b54e-167">Authentication and EWS in Exchange</span></span>](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [<span data-ttu-id="4b54e-168">Configurações de conexão POP e IMAP</span><span class="sxs-lookup"><span data-stu-id="4b54e-168">IMAP, POP Connection settings</span></span>](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [<span data-ttu-id="4b54e-169">Internet Message Access Protocol</span><span class="sxs-lookup"><span data-stu-id="4b54e-169">Internet Message Access Protocol</span></span>](https://tools.ietf.org/html/rfc3501)
- [<span data-ttu-id="4b54e-170">Protocolo Post Office</span><span class="sxs-lookup"><span data-stu-id="4b54e-170">Post Office Protocol</span></span>](https://tools.ietf.org/html/rfc1081)
- [<span data-ttu-id="4b54e-171">Extensão de serviço SMTP para autenticação</span><span class="sxs-lookup"><span data-stu-id="4b54e-171">SMTP Service extension for Authentication</span></span>](https://tools.ietf.org/html/rfc4954)
