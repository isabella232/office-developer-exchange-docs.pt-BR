---
title: Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth
description: Saiba como usar a autenticação OAuth com seus aplicativos IMAP, POP e SMTP.
author: svpsiva
ms.date: 07/08/2021
ms.audience: Developer
ms.openlocfilehash: 4a307a6e329d5320b2b304d17a78a61db6d111bd
ms.sourcegitcommit: 357b882a02e37b380a23b8a45b15f9c006a40b02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58764585"
---
# <a name="authenticate-an-imap-pop-or-smtp-connection-using-oauth"></a>Autenticar uma conexão IMAP, POP ou SMTP usando o OAuth

Saiba como usar a autenticação OAuth para se conectar com protocolos IMAP, POP ou SMTP e acessar dados de email para Office 365 usuários.

> O suporte ao OAuth2 para protocolos IMAP, POP, SMTP conforme descrito abaixo é suportado para usuários Microsoft 365 (que inclui Office na Web) e Outlook.com.

Se você não estiver familiarizado com o protocolo OAuth 2.0, comece lendo o protocolo [OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols)em plataforma de identidade da Microsoft visão geral. Para saber mais sobre o Microsoft Authentication Libariers (MSAL), que implementa o protocolo OAuth 2.0 para autenticar usuários e acessar APIs seguras, leia a visão geral [do MSAL](/azure/active-directory/develop/msal-overview).

Você pode usar o serviço de autenticação OAuth fornecido pelo Azure Active Directory para permitir que seu aplicativo se conecte aos protocolos IMAP, POP ou SMTP para acessar Exchange Online no Office 365. Para usar o OAuth com seu aplicativo, você precisa:

1. [Registrar o aplicativo](#register-your-application) com o Azure Active Directory.
1. [Configure seu aplicativo](#configure-your-application) em Azure Active Directory.
1. [Obter um token de acesso](#get-an-access-token) de um servidor de tokens.
1. [Autenticar solicitações de conexão](#authenticate-connection-requests) com um token de acesso.

## <a name="register-your-application"></a>Registre seu aplicativo

Para usar o OAuth, um aplicativo deve ser registrado com Azure Active Directory.

Siga as instruções listadas em [Registrar um aplicativo com o plataforma de identidade da Microsoft](/azure/active-directory/develop/quickstart-register-app) para criar um novo aplicativo.

## <a name="get-an-access-token"></a>Obter um token de acesso

Você pode usar uma de nossas bibliotecas de clientes [MSAL](/azure/active-directory/develop/msal-overview) para buscar um token de acesso do seu aplicativo cliente.

Como alternativa, você pode selecionar um fluxo apropriado na lista a seguir e seguir as etapas correspondentes para chamar as APIs REST da plataforma de identidade subjacente e recuperar um token de acesso.

1. [Fluxo de código de autorização OAuth2](/azure/active-directory/develop/v2-oauth2-auth-code-flow)
1. [Fluxo de concessão de autorização do dispositivo OAuth2](/azure/active-directory/develop/v2-oauth2-device-code)

Não há suporte para o acesso OAuth aos protocolos AUTH IMAP, POP e SMTP por meio de credenciais de cliente OAuth2. Se seu aplicativo precisar de acesso persistente a todas as caixas de correio em uma organização Microsoft 365, recomendamos que você use as APIs do Microsoft Graph que permitem o acesso sem um usuário, habilitam permissões granulares e permitem que os administradores acessem esse acesso a um conjunto específico de caixas de correio.

Certifique-se de especificar os escopos completos, incluindo Outlook URLs de recursos, ao autorizar seu aplicativo e solicitar um token de acesso.

| Protocolo  | Cadeia de caracteres de escopo de permissão |
|-----------|-------------------------|
| IMAP      | `https://outlook.office.com/IMAP.AccessAsUser.All` |
| POP       | `https://outlook.office.com/POP.AccessAsUser.All`  |
| SMTP AUTH | `https://outlook.office.com/SMTP.Send`             |

Além disso, você pode solicitar [offline_access](/azure/active-directory/develop/v2-permissions-and-consent#offline_access) escopo. Quando um usuário aprova o escopo offline_access, seu aplicativo pode receber tokens de atualização do ponto de extremidade plataforma de identidade da Microsoft token. Os tokens de atualização são de longa duração. Seu aplicativo pode obter novos tokens de acesso à medida que os mais antigos expiram.

## <a name="authenticate-connection-requests"></a>Autenticar solicitações de conexão

Você pode iniciar uma conexão com Office 365 de email usando as [configurações de email IMAP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)e POP para Office 365 .

### <a name="sasl-xoauth2"></a>SASL XOAUTH2

A integração com o OAuth requer que seu aplicativo use o formato SASL XOAUTH2 para codificar e transmitir o token de acesso. O SASL XOAUTH2 codifica o nome de usuário e o token de acesso no seguinte formato:

```text
base64("user=" + userName + "^Aauth=Bearer " + accessToken + "^A^A")
```

`^A`representa um **Controle**  +  **A** ( `%x01` ).

Por exemplo, o formato SASL XOAUTH2 para acessar `test@contoso.onmicrosoft.com` com token de acesso `EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA` é:

```text
base64("user=test@contoso.onmicrosoft.com^Aauth=Bearer EwBAAl3BAAUFFpUAo7J3Ve0bjLBWZWCclRC3EoAA^A^A")
```

Após a codificação base64, isso se traduz na sequência de caracteres a seguir. Observe que as quebras de linha são inseridas para capacidade de leitura.

```text
dXNlcj10ZXN0QGNvbnRvc28ub25taWNyb3NvZnQuY29tAWF1dGg9QmVhcmVy
IEV3QkFBbDNCQUFVRkZwVUFvN0ozVmUwYmpMQldaV0NjbFJDM0VvQUEBAQ==
```

### <a name="sasl-xoauth2-authentication-for-shared-mailboxes-in-office-365"></a>Autenticação SASL XOAUTH2 para caixas de correio compartilhadas no Office 365

Em caso de acesso de caixa de correio compartilhada usando o OAuth, o aplicativo precisa obter o token de acesso em nome de um usuário, mas substituir o campo userName na cadeia de caracteres codificada do SASL XOAUTH2 pelo endereço de email da caixa de correio compartilhada. 

### <a name="imap-protocol-exchange"></a>Protocolo IMAP Exchange

Para autenticar uma conexão de servidor IMAP, o cliente terá que responder com um `AUTHENTICATE` comando no seguinte formato:

```text
AUTHENTICATE XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemplo de troca de mensagens cliente-servidor que resulta em um sucesso de autenticação:

```text
[connection begins]
C: C01 CAPABILITY
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 OK AUTHENTICATE completed.
```

Exemplo de troca de mensagens cliente-servidor que resulta em uma falha de autenticação:

```text
[connection begins]
S: * CAPABILITY … AUTH=XOAUTH2
S: C01 OK Completed
C: A01 AUTHENTICATE XOAUTH2 dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlYXJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMjl0Q2cBAQ==
S: A01 NO AUTHENTICATE failed.
```

### <a name="pop-protocol-exchange"></a>Protocolo POP Exchange

Para autenticar uma conexão de servidor POP, o cliente terá que responder com um comando dividido em duas `AUTH` linhas no seguinte formato:    

```text 
AUTH XOAUTH2 
<base64 string in XOAUTH2 format>   
``` 

Exemplo de troca de mensagens cliente-servidor que resulta em um sucesso de autenticação:    

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

Exemplo de troca de mensagens cliente-servidor que resulta em uma falha de autenticação:    

```text 
[connection begins] 
C: AUTH XOAUTH2     
S: +    
C: dXNlcj1zb21ldXNlckBleGFtcGxlLmNvbQFhdXRoPUJlY    
XJlciB5YTI5LnZGOWRmdDRxbVRjMk52YjNSbGNrQmhkSFJoZG1semRHRXVZMj   
l0Q2cBAQ=   
S: -ERR Authentication failure: unknown user name or bad password.  
```

### <a name="smtp-protocol-exchange"></a>Protocolo SMTP Exchange

Para autenticar uma conexão de servidor SMTP, o cliente terá que responder com um `AUTH` comando no seguinte formato:

```text
AUTH XOAUTH2 <base64 string in XOAUTH2 format>
```

Exemplo de troca de mensagens cliente-servidor que resulta em um sucesso de autenticação:

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

Exemplo de troca de mensagens cliente-servidor que resulta em uma falha de autenticação:

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
- [Configurações IMAP, Conexão POP](https://support.office.com/article/pop-and-imap-email-settings-for-outlook-8361e398-8af4-4e97-b147-6c6c4ac95353)
- [Protocolo de Acesso a Mensagens da Internet](https://tools.ietf.org/html/rfc3501)
- [Protocolo Post Office](https://tools.ietf.org/html/rfc1081)
- [Extensão de serviço SMTP para autenticação](https://tools.ietf.org/html/rfc4954)
