---
title: Autenticação e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Encontre informações para ajudar na escolha do padrão de autenticação correto para o seu aplicativo EWS que visa o Exchange.
localization_priority: Priority
ms.openlocfilehash: 0b35921f33b935f9a5a490e15d4e76d1a3e3c9dc
ms.sourcegitcommit: 843a2e030a94b12aec70c553ca4e06e39ac02d82
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49603831"
---
# <a name="authentication-and-ews-in-exchange"></a>Autenticação e EWS no Exchange

Encontre informações para ajudar na escolha do padrão de autenticação correto para o seu aplicativo EWS que visa o Exchange.
  
A autenticação é uma parte fundamental do aplicativo EWS (Serviços Web do Exchange). O Exchange Online, o Exchange Online como parte do Office 365, e as versões locais do Exchange, a partir do Exchange Server 2013, oferecem suporte a protocolos de autenticação Web padrão para ajudar a proteger a comunicação entre o aplicativo e o servidor Exchange.
  
Se você estiver usando o Exchange Online, o método de autenticação escolhido deve usar HTTPS para criptografar as solicitações e respostas enviadas pelo aplicativo. Embora seja possível usar HTTP com servidores do Exchange no local, recomendamos o uso de HTTPS para qualquer solicitação que o aplicativo envie a um ponto de extremidade do EWS para ajudar a proteger a comunicação o aplicativo e um servidor Exchange.
  
O Exchange oferece as seguintes opções de autenticação para você escolher: 
  
- OAuth 2.0 (somente Exchange Online)
    
- NTLM (somente Exchange no local)
    
- Básico (não recomendado)
    
O método de autenticação escolhido depende dos requisitos de segurança da organização, se você está usando o Exchange Online ou o Exchange no local, e se você tem acesso a um provedor de terceiros que emite tokens OAuth. Este artigo fornece informações que ajudarão você a escolher o padrão de autenticação ideal para o seu aplicativo.
  
## <a name="oauth-authentication"></a>Autenticação OAuth

É recomendável que todos os novos aplicativos usem o padrão OAuth para se conectar aos serviços do Exchange Online. O trabalho adicional necessário para implementar o OAuth traz a vantagem de ter maior segurança em relação à autenticação básica. No entanto, há também algumas desvantagens que você deve estar ciente.
  
**Tabela 1. Vantagens e desvantagens de usar o OAuth**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| O OAuth é um protocolo de autenticação padrão do setor.<br/><br/>A autenticação é gerenciada por um provedor de terceiros. O aplicativo não precisa coletar e armazenar as credenciais do Exchange.<br/><br/>Menos preocupações para você, pois o aplicativo só recebe um token opaco do provedor de autenticação; portanto, uma violação de segurança no aplicativo só expõe o token, e não as credenciais do Exchange do usuário.  <br/> | O OAuth conta com um provedor de autenticação de terceiros. Isso pode impor custos adicionais à organização ou aos clientes.<br/><br/>O padrão OAuth é mais difícil de implementar do que a autenticação básica.<br/><br/>Para implementar o OAuth, é necessário integrar o aplicativo com o provedor de autenticação e o servidor do Exchange.  <br/> |
   
Para ajudar a minimizar as desvantagens, use a [Biblioteca de Autenticação do Microsoft Azure AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) para autenticar os usuários ao AD DS (Active Directory Domain Services) na nuvem ou no local e, em seguida, obter tokens de acesso para proteger as chamadas a um servidor do Exchange. O Exchange Online requer fichas emitidas pelo serviço do Azure Active Directory que é aceito pelo ADAL; no entanto, é possível usar qualquer biblioteca de terceiros. 
  
Para saber mais sobre como usar a autenticação OAuth no aplicativo EWS, confira os seguintes recursos:
  
- [Avaliação do Office 365](https://docs.microsoft.com/office/developer-program/office-365-developer-program), para configurar um servidor Exchange a ser usado para testar o aplicativo do cliente.
    
- [Biblioteca de Autenticação do Azure AD para .NET](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)
    
- [Configurar o Azure Active Directory](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx) para permitir que o aplicativo use tokens OAuth para autenticação.
    
- Verifique o código de exemplo em [Autenticar um aplicativo EWS usando o OAuth](how-to-authenticate-an-ews-application-by-using-oauth.md), como código de exemplo a ser estudado. 
    
## <a name="ntlm-authentication"></a>Autenticação NTLM

A autenticação NTLM está disponível apenas para servidores do Exchange no local. Para aplicativos executados dentro do firewall corporativo, a integração entre a autenticação NTLM e o .NET Framework fornece um meio integrado para autenticar o aplicativo. 
  
**Tabela 2. Vantagens e desvantagens de usar a autenticação NTLM**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Funciona como pronto para uso com o servidor Exchange. Configure o acesso aos serviços do Exchange usando um [cmdlet do Shell de Gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Usa o objeto [CredentialCache](https://msdn2.microsoft.com/library/615e0wsd) do .NET Framework para obter automaticamente as credenciais do usuário.<br/><br/>[Estão disponíveis exemplos de código](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) que usam as credenciais do usuário conectado para autenticação em um servidor do Exchange no local.  <br/> | Os usuários devem estar conectados a um domínio para usar a autenticação NTLM.<br/><br/>Pode ser difícil acessar as contas de email que não estão associadas à conta de domínio do usuário.<br/><br/>Os aplicativos de serviço devem ter uma conta de domínio para aproveitar a autenticação NTLM.  <br/> |

   
## <a name="basic-authentication"></a>Autenticação básica

A autenticação básica oferece um nível básico de segurança para o aplicativo cliente. É recomendável que todos os novos aplicativos usem NTLM ou o protocolo OAuth para autenticação; no entanto, a autenticação básica pode ser a escolha ideal para o aplicativo em algumas circunstâncias.
  
**Tabela 3. Vantagens e desvantagens de usar a autenticação básica**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Funciona como pronto para uso com o servidor Exchange. Configure o acesso aos serviços do Exchange usando um [cmdlet do Shell de Gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Os aplicativos do Windows podem usar as credenciais padrão do usuário conectado.<br/><br/>Vários [exemplos de código disponíveis](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) que mostram como chamar o EWS usando autenticação básica.  <br/> | Requer que o aplicativo colete ou armazene as credenciais do usuário.<br/><br/>Será necessário desativar a autenticação NTLM se quiser forçar todos os usuários a usar a autenticação básica.<br/><br/>Se ocorrer uma violação de segurança no aplicativo, ela poderá expor o endereço de email e a senha do usuário ao invasor.  <br/> |
   
É necessário decidir se a autenticação básica atende aos requisitos de segurança da sua organização e dos seus clientes. A autenticação básica pode ser a escolha certa se você quiser evitar tarefas de configuração demoradas, por exemplo, para aplicativos simples de teste ou de demonstração.

> [!NOTE]
> Não há mais suporte para a autenticação básica no EWS para conectar-se ao Exchange Online. Use a autenticação OAuth em todos os aplicativos novos ou existentes do EWS para se conectar ao Exchange Online. A autenticação OAuth para o EWS só está disponível no Exchange Online como parte do Microsoft 365. Os aplicativos do EWS que usam o OAuth devem ser registrados com o Azure Active Directory.
  
## <a name="see-also"></a>Confira também
- [Autenticar um aplicativo EWS usando o OAuth](how-to-authenticate-an-ews-application-by-using-oauth.md)
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Adicionar o logon ao aplicativo Web usando o Microsoft Azure AD](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Controlar o acesso ao EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)    
- [Controlar o acesso do aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Tipos de token e de declaração com suporte](https://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
 
