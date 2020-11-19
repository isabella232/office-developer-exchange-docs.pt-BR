---
title: Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth
description: Saiba como usar a autenticação OAuth com seus aplicativos IMAP, POP e SMTP.
author: svpsiva
ms.date: 02/19/2020
ms.audience: Developer
ms.openlocfilehash: 4662aa904ed162edcced6c096eac8cf636180f6a
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348812"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth

Saiba como usar a autenticação OAuth para se conectar com protocolos IMAP, POP ou SMTP e acessar dados de email para usuários do Office 365.

> O suporte do OAuth2 para protocolos IMAP, POP, SMTP, conforme descrito abaixo, é suportado para o Microsoft 365 (que inclui o Office na Web) e os usuários do Outlook.com.

Se você não estiver familiarizado com o protocolo OAuth 2,0, comece lendo o [protocolo oauth 2,0 na visão geral da plataforma de identidade da Microsoft](/azure/active-directory/develop/active-directory-v2-protocols). Para saber mais sobre o Microsoft Authentication Libariers (MSAL), que implementa o protocolo OAuth 2,0 para autenticar usuários e acessar APIs seguras, leia a [visão geral do MSAL](/azure/active-directory/develop/msal-overview).

Você pode usar o serviço de autenticação OAuth fornecido pelo Azure Active Directory para permitir que seu aplicativo se conecte com protocolos IMAP, POP ou SMTP para acessar o Exchange Online no Office 365. Para usar o OAuth com seu aplicativo, você precisa:

1. [Registrar o aplicativo](#register-your-application) com o Azure Active Directory.
1. [Configure seu aplicativo](#configure-your-application) no Azure Active Directory.
1. [Obter um token de acesso](#get-an-access-token) de um servidor de token.
1. [Autenticar solicitações de conexão](#authenticate-connection-requests) com um token de acesso.

## <a name="register-your-application"></a>Registre seu aplicativo

Para usar o OAuth, um aplicativo deve ser registrado no Azure Active Directory.

Siga as instruções listadas em [registrar um aplicativo com a plataforma de identidade da Microsoft](/azure/active-directory/develop/quickstart-register-app) para criar um novo aplicativo.

## <a name="configure-your-application"></a>Configurar seu aplicativo

Siga as instruções listadas em [configurar um aplicativo cliente para acessar as APIs da Web](/azure/active-directory/develop/quickstart-configure-app-access-web-apis)

Certifique-se de adicionar um ou mais dos seguintes escopos de permissão que correspondem aos protocolos que você gostaria de integrar. No assistente **Adicionar uma permissão** , selecione **Microsoft Graph** e, em seguida, **permissões delegadas** para localizar os seguintes escopos de permissão listados.

| Protocolo  | Escopo de permissão        |
|-----------|-------------------------|
| IMAP      | `IMAP.AccessAsUser.All` |
| POP       | `POP.AccessAsUser.All`  |
| AUTENTICAÇÃO SMTP | `SMTP.Send`             |

## <a name="get-an-access-token"></a>Obter um token de acesso

Você pode usar uma de nossas [bibliotecas de cliente do MSAL](/azure/active-directory/develop/msal-overview) para buscar um token de acesso do aplicativo cliente.

Como alternativa, você pode selecionar um fluxo apropriado da lista a seguir e seguir as etapas correspondentes para chamar as APIs REST da plataforma de identidade subjacente e recuperar um token de acesso.

1. [Fluxo de código de autorização OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Fluxo de concessão de autorização de dispositivo OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

Não há suporte para o acesso OAuth a IMAP, POP, protocolos de autenticação SMTP por meio do fluxo de concessão de credenciais do cliente OAuth2. Se seu aplicativo precisar de acesso persistente a todas as caixas de correio em uma organização do Microsoft 365, recomendamos que você use as APIs do Microsoft Graph que permitem o acesso sem um usuário, habilite permissões granulares e permita que o escopo de administradores desse acesso a um conjunto específico de caixas de correio.

Certifique-se de especificar os escopos completos, incluindo URLs de recursos do Outlook, ao autorizar seu aplicativo e solicitar um token de acesso.

| Protocolo  | Cadeia de caracteres de escopo de permissão |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| AUTENTICAÇÃO SMTP | `https://outlook.office.com/SMTP.Send`             |

Além disso, você pode solicitar [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) escopo. Quando um usuário aprova o escopo de offline_access, seu aplicativo pode receber tokens de atualização do ponto de extremidade de token da plataforma de identidade da Microsoft. Os tokens de atualização são de longa duração. Seu aplicativo pode obter novos tokens de acesso com a expiração dos mais antigos.

## <a name="authenticate-connection-requests"></a>Autenticar solicitações de conexão

Você pode iniciar uma conexão com os servidores de email do Office 365 usando as [configurações de email IMAP e pop para o Office 365](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353).

### <a name="sasl-xoauth2"></a>XOAUTH2 SASL

A integração OAuth com exige que seu aplicativo use o formato SASL XOAUTH2 para codificar e transmitir o token de acesso. O SASL XOAUTH2 codifica o nome de usuário, o token de acesso em conjunto no seguinte formato:

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`representa um **controle**  +  **a** ( `%x01` ).

Por exemplo, o formato SASL XOAUTH2 para acessar `test@contoso.onmicrosoft.com` com o token de acesso `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` é:

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

Após a codificação Base64, isso é convertido para a cadeia de caracteres a seguir. Observe que as quebras de linha são inseridas para facilitar a leitura.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Autenticação de XOAUTH2 do SASL para caixas de correio compartilhadas no Office 365

No caso de acesso compartilhado de caixa de correio usando o OAuth, o aplicativo precisa obter o token de acesso em nome de um usuário, mas substituir o campo userName na cadeia de caracteres codificada XOAUTH2 do SASL pelo endereço de email da caixa de correio compartilhada. 

### <a name="imap-protocol-exchange"></a>Intercâmbio de protocolo IMAP

Para autenticar uma conexão de servidor IMAP, o cliente terá que responder com um `AUTHENTICATE` comando no seguinte formato:

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Troca de protocolo POP

Para autenticar uma conexão de servidor POP, o cliente terá que responder com um `AUTH` comando dividido em duas linhas no seguinte formato:    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:    

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

Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Troca de protocolo SMTP

Para autenticar uma conexão de servidor SMTP, o cliente terá que responder com um `AUTH` comando no seguinte formato:

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemplo de troca de mensagens do cliente-servidor que resulta em um êxito de autenticação:

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

Exemplo de troca de mensagens do cliente-servidor que resulta em uma falha de autenticação:

```text
[connection begins]
C: auth xoauth2
S: 334
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj
l0Q2cBAQ==
S: 535 5.7.3 Authentication unsuccessful [SN2PR00CA0018.namprd00.prod.outlook.com]
```

## <a name="see-also"></a>Confira também

- [Autenticação e EWS no Exchange](../exchange-web-services/authentication-and-ews-in-exchange.md)
- [Configurações de conexão POP e IMAP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Internet Message Access Protocol](https://tools.ietf.org/html/rfc3501)
- [Protocolo Post Office](https://tools.ietf.org/html/rfc1081)
- [Extensão de serviço SMTP para autenticação](https://tools.ietf.org/html/rfc4954)
