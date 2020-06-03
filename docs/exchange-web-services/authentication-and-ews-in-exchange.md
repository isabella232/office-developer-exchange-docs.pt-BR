---
title: Autenticação e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Encontre informações para ajudá-lo a escolher o padrão de autenticação certo para seu aplicativo do EWS que tem como alvo o Exchange.
localization_priority: Priority
ms.openlocfilehash: 69018b6f88fc80e1e18edd96ed0e16d52064572d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528479"
---
# <a name="authentication-and-ews-in-exchange"></a>Autenticação e EWS no Exchange

Encontre informações para ajudá-lo a escolher o padrão de autenticação certo para seu aplicativo do EWS que tem como alvo o Exchange.
  
A autenticação é uma parte fundamental do seu aplicativo de serviços Web do Exchange (EWS). O Exchange Online, o Exchange Online como parte do Office 365 e versões locais do Exchange a partir do Exchange Server 2013 dão suporte a protocolos de autenticação da Web padrão para ajudar a proteger a comunicação entre seu aplicativo e o servidor do Exchange.
  
Se você estiver direcionando para o Exchange Online, o método de autenticação que você escolher deverá usar HTTPS para criptografar as solicitações e respostas enviadas por seu aplicativo. Embora você possa usar HTTP com servidores locais do Exchange, recomendamos que você use HTTPS para qualquer solicitação que seu aplicativo envie para um ponto de extremidade do EWS para ajudar a proteger a comunicação entre seu aplicativo e um servidor Exchange.
  
O Exchange fornece as seguintes opções de autenticação para que você escolha: 
  
- OAuth 2,0 (somente Exchange Online)
    
- NTLM (somente Exchange local)
    
- Básico (não é mais recomendado)
    
O método de autenticação escolhido depende dos requisitos de segurança da sua organização, se você estiver usando o Exchange Online ou o Exchange local, e se você tem acesso a um provedor de terceiros que possa emitir tokens OAuth. Este artigo fornece informações que o ajudarão a selecionar o padrão de autenticação adequado para o seu aplicativo.
  
## <a name="oauth-authentication"></a>Autenticação OAuth

Recomendamos que todos os novos aplicativos usem o padrão OAuth para se conectarem aos serviços do Exchange Online. A vantagem de segurança sobre a autenticação básica vale o trabalho adicional necessário para implementar o OAuth em seu aplicativo. Para o registro, no entanto, há também algumas desvantagens que você deve estar ciente.
  
**Tabela 1. Vantagens e desvantagens de usar o OAuth**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| O OAuth é um protocolo de autenticação padrão da indústria.<br/><br/>A autenticação é gerenciada por um provedor de terceiros. O aplicativo não precisa coletar e armazenar as credenciais do Exchange.<br/><br/>Menos preocupações para você, porque seu aplicativo só recebe um token opaco do provedor de autenticação; Portanto, uma violação de segurança em seu aplicativo só pode expor o token, não as credenciais do Exchange do usuário.  <br/> | O OAuth se baseia em um provedor de autenticação de terceiros. Isso pode impor custos adicionais à sua organização ou seus clientes.<br/><br/>O padrão OAuth é mais difícil de implementar do que a autenticação básica.<br/><br/>Para implementar o OAuth, você precisa integrar seu aplicativo com o provedor de autenticação e o servidor do Exchange.  <br/> |
   
Para ajudar a minimizar as desvantagens, você pode usar a [biblioteca de autenticação do Microsoft Azure ad](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (Adal) para autenticar usuários nos serviços de domínio do Active Directory (AD DS) na nuvem ou no local e, em seguida, obter tokens de acesso para proteger as chamadas a um servidor Exchange. O Exchange Online requer tokens emitidos pelo serviço do Azure Active Directory, que é suportado pela ADAL; no entanto, você pode usar qualquer biblioteca de terceiros. 
  
Para saber mais sobre como usar a autenticação OAuth no seu aplicativo EWS, confira os seguintes recursos:
  
- [Versão de avaliação do Office 365](https://docs.microsoft.com/office/developer-program/office-365-developer-program), para configurar um servidor Exchange a ser usado para testar o aplicativo cliente.
    
- [Biblioteca de Autenticação do Azure AD para .NET](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)
    
- [Configure o Azure Active Directory](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)para permitir que seu aplicativo use tokens OAuth para autenticação.
    
- Revise o código de exemplo em [autenticar um aplicativo EWS usando OAuth](how-to-authenticate-an-ews-application-by-using-oauth.md) como código de exemplo que você pode estudar. 
    
## <a name="ntlm-authentication"></a>Autenticação NTLM

A autenticação NTLM só está disponível para servidores locais do Exchange. Para aplicativos executados dentro do firewall corporativo, a integração entre a autenticação NTLM e o .NET Framework fornece um meio interno para autenticar seu aplicativo. 
  
**Tabela 2. Vantagens e desvantagens de usar a autenticação NTLM**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Funciona "pronto" com o Exchange Server. Você pode configurar o acesso aos serviços do Exchange usando um [cmdlet do Shell de gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Usa o objeto [CredentialCache](https://msdn2.microsoft.com/library/615e0wsd) do .NET Framework para obter automaticamente as credenciais do usuário.<br/><br/>[Exemplos de código estão disponíveis](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) para usar as credenciais do usuário conectado para autenticação em um servidor Exchange local.  <br/> | Os usuários devem estar conectados a um domínio para usar a autenticação NTLM.<br/><br/>Pode ser difícil acessar contas de email que não estão associadas à conta de domínio do usuário.<br/><br/>Os aplicativos de serviço devem ter uma conta de domínio para aproveitar a autenticação NTLM.  <br/> |

   
## <a name="basic-authentication"></a>Autenticação básica

A autenticação básica fornece um nível básico de segurança para o aplicativo cliente. Recomendamos que todos os novos aplicativos usem o NTLM ou o protocolo OAuth para autenticação; no entanto, a autenticação básica pode ser a escolha correta para seu aplicativo em algumas circunstâncias.
  
**Tabela 3. Vantagens e desvantagens de usar a autenticação básica**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Funciona "pronto" com o Exchange Server. Você pode configurar o acesso aos serviços do Exchange usando um [cmdlet do Shell de gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Os aplicativos do Windows podem usar as credenciais padrão do usuário conectado.<br/><br/>[Há vários exemplos de código disponíveis](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) que mostram como chamar o EWS usando a autenticação básica.  <br/> | Requer que seu aplicativo colete e armazene as credenciais do usuário.<br/><br/>Você precisa desativar a autenticação NTLM se quiser forçar todos os usuários a usar a autenticação básica.<br/><br/>Se ocorrer uma violação de segurança em seu aplicativo, ele poderá expor o endereço de email e a senha do usuário ao invasor.  <br/> |
   
Você precisa decidir se a autenticação básica atende aos requisitos de segurança da sua organização e dos clientes. A autenticação básica pode ser a escolha certa se você quiser evitar tarefas abrangentes de configuração, por exemplo, para aplicativos simples de teste ou demonstração.
  
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Adicionando logon ao seu aplicativo Web usando o Microsoft Azure AD](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Controlar o acesso ao EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)    
- [Controlando o acesso do aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)   
- [Tipos de token e declaração com suporte](https://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
 