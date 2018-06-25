---
title: Autenticação e EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Encontre informações para ajudá-lo a escolher o padrão de autenticação correto para seu aplicativo do EWS que tem como destino o Exchange.
ms.openlocfilehash: c81b29cbe9aa3c658a8f776876366fd0875b2669
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750646"
---
# <a name="authentication-and-ews-in-exchange"></a>Autenticação e EWS no Exchange

Encontre informações para ajudá-lo a escolher o padrão de autenticação correto para seu aplicativo do EWS que tem como destino o Exchange.
  
A autenticação é parte essencial do seu aplicativo de serviços Web do Exchange (EWS). O Exchange Online, Exchange Online como parte do Office 365 e a versões locais do Exchange, começando com o Exchange Server 2013 suporta os protocolos de autenticação padrão da web para ajudar a proteger a comunicação entre seu aplicativo e o Exchange server.
  
Se você está direcionando Exchange Online, o método de autenticação que você escolher deve usar HTTPS para criptografar as solicitações e respostas que envia seu aplicativo. Embora você possa usar HTTP com servidores locais do Exchange, é recomendável que você use HTTPS para qualquer solicitação que o seu aplicativo envia para um ponto de extremidade do EWS para ajudar a comunicação segura entre seu aplicativo e um servidor Exchange.
  
Exchange oferece as seguintes opções de autenticação para sua escolha: 
  
- OAuth 2.0 (somente no Exchange Online)
    
- NTLM (Exchange local somente)
    
- Basic (não recomendado)
    
O método de autenticação que você escolher depende de requisitos de segurança de sua organização, se você estiver usando o Exchange Online ou Exchange local e se você tem acesso a um provedor de terceiros que pode emitir tokens OAuth. Este artigo fornece informações que ajudarão você a selecionar o padrão de autenticação que é ideal para seu aplicativo.
  
## <a name="oauth-authentication"></a>Autenticação OAuth

Recomendamos que todos os novos aplicativos usam o padrão de OAuth para conectar aos serviços do Exchange Online. A vantagem de segurança sobre a autenticação básica vale o trabalho adicional necessário para implementar o OAuth em seu aplicativo. Para o registro, no entanto, há também algumas desvantagens que você deve estar ciente.
  
**Tabela 1. Vantagens e desvantagens de usar OAuth**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| OAuth é um protocolo de autenticação padrão do setor.<br/><br/>Autenticação é gerenciada por um provedor de terceiros. Não tem seu aplicativo coletar e armazenar as credenciais do Exchange.<br/><br/>Menos preocupações para você, como seu aplicativo só recebe um token de opaco do provedor de autenticação; Portanto, uma violação de segurança em seu aplicativo só pode expor o token, não as credenciais do usuário Exchange.  <br/> | OAuth depende de um provedor de autenticação de terceiros. Isso pode impor custo adicional em sua organização ou seus clientes.<br/><br/>O padrão de OAuth é mais difícil de implementar do que a autenticação básica.<br/><br/>Para implementar o OAuth, você precisa integrar seu aplicativo com o provedor de autenticação e o servidor Exchange.  <br/> |
   
Para ajudar a minimizar as desvantagens, você pode usar a [Biblioteca de autenticação do Microsoft Azure AD](http://msdn.microsoft.com/library/a03f39fa-7ba4-4182-a98e-55562a64b8f3%28Office.15%29.aspx) (ADAL) para autenticar usuários aos serviços de domínio Active Directory (AD DS) na nuvem ou no local e, em seguida, obter tokens de acesso para proteger as chamadas para um Servidor do Exchange. O Exchange Online requer tokens emitidos pelo serviço do Windows Azure Active Directory, que é compatível com o ADAL; No entanto, você pode usar qualquer biblioteca de terceiros. 
  
Para saber mais sobre como usar a autenticação OAuth no seu aplicativo do EWS, consulte os seguintes recursos:
  
- [Avaliação do office 365](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx?CR_CC=200061904&amp;WT.srch=1&amp;WT.mc_ID=PS_bing_O365Comm_office%20365%20trial_Text), para configurar um servidor Exchange para usar para testar seu aplicativo cliente.
    
- [Biblioteca de Autenticação do Azure AD para .NET](http://msdn.microsoft.com/library/a03f39fa-7ba4-4182-a98e-55562a64b8f3%28Office.15%29.aspx)
    
- [Configurar o Azure Active Directory](http://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx), para habilitar o aplicativo para usar os tokens OAuth para autenticação.
    
- Revise o código de exemplo em [um aplicativo do EWS usando OAuth de autenticar](how-to-authenticate-an-ews-application-by-using-oauth.md) por exemplo código que podem ser analisados. 
    
## <a name="ntlm-authentication"></a>Autenticação NTLM

Autenticação NTLM só está disponível para os servidores do Exchange local. Para aplicativos que são executados dentro do firewall corporativo, a integração entre a autenticação NTLM e o .NET Framework fornece que uma interna significa para autenticar seu aplicativo. 
  
**Tabela 2. Vantagens e desvantagens de usar a autenticação NTLM**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Works "fora da caixa" com seu servidor do Exchange. Você pode configurar o acesso aos serviços do Exchange usando um [cmdlet do Shell de gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Usa o objeto do .NET Framework [CredentialCache](http://msdn2.microsoft.com/EN-US/library/615e0wsd) obter automaticamente as credenciais do usuário.<br/><br/>[Exemplos de código estão disponíveis](http://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) que usam o conectado em credenciais do usuário para autenticação a um servidor do Exchange local.  <br/> | Os usuários devem estar conectados a um domínio para usar a autenticação NTLM.<br/><br/>Pode ser difícil acessar as contas de email que não estão associadas a conta de domínio do usuário.<br/><br/>Aplicativos de serviço devem ter uma conta de domínio para aproveitar as vantagens da autenticação NTLM.  <br/> |
   
## <a name="basic-authentication"></a>Autenticação básica

Oferece autenticação básica r, bem, nível básico de segurança para o aplicativo cliente. Recomendamos que todos os novos aplicativos usam NTLM ou o protocolo OAuth para autenticação; No entanto, a autenticação básica pode ser a opção correta para seu aplicativo em algumas circunstâncias.
  
**Tabela 3. Vantagens e desvantagens de usar a autenticação básica**

|**Vantagens**|**Desvantagens**|
|:-----|:-----|
| Works "fora da caixa" com seu servidor do Exchange. Você pode configurar o acesso aos serviços do Exchange usando um [cmdlet do Shell de gerenciamento do Exchange](how-to-control-access-to-ews-in-exchange.md).<br/><br/>Aplicativos do Windows podem usar credenciais de padrão do usuário conectado.<br/><br/>Muitos [exemplos de código estão disponíveis](http://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c) que mostram como chamar EWS usando a autenticação básica.  <br/> | Exige o seu aplicativo para coletar e armazenar as credenciais do usuário.<br/><br/>Você precisa desativar a autenticação NTLM para todos os usuários usem a autenticação básica.<br/><br/>Se ocorrer uma violação de segurança em seu aplicativo, ele poderá expor o endereço de email do usuário e senha para o invasor.  <br/> |
   
Você precisará decidir se a autenticação básica atende os requisitos de segurança da sua organização e os clientes. A autenticação básica pode ser a melhor opção se você deseja evitar tarefas de instalação extensiva, por exemplo, para teste simples ou aplicativos de demonstração.
  
## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)   
- [Adicionando Sign-On para seu aplicativo Web usando o Microsoft Azure AD.](http://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Controlar o acesso a EWS no Exchange](how-to-control-access-to-ews-in-exchange.md)    
- [Controlando o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md)    
- [Token com suporte e tipos de declaração](http://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
    

