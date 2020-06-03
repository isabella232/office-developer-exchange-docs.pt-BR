---
title: Introdução ao uso dos serviços Web no Exchange
manager: sethgros
ms.date: 2/26/2019
ms.audience: Developer
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Encontre informações para ajudá-lo a começar a usar o EWS e outros serviços Web no Exchange.
localization_priority: Priority
ms.openlocfilehash: 5980e22599585aa376890a414e0e8e7c7c5c707a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463752"
---
# <a name="start-using-web-services-in-exchange"></a>Introdução ao uso dos serviços Web no Exchange

Encontre informações para ajudá-lo a começar a usar o EWS e outros serviços Web no Exchange.
  
Os [Serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) fornecem acesso a dados de caixa de correio armazenados no Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange a partir do exchange Server 2007 e permitem que você crie aplicativos personalizados que você pode usar para gerenciar essas informações de acordo com os requisitos de sua organização. Embora o intervalo de aplicativos de serviço da Web e do EWS que você pode criar seja praticamente infinito, certos conceitos fundamentais se aplicam a qualquer tipo de aplicativo. Esta seção fornece informações sobre os conceitos fundamentais com os quais você precisa se familiarizar para começar a usar o EWS e outros serviços Web no Exchange. 
  
## <a name="build-your-knowledge"></a>Criar seu conhecimento
<a name="bk_Knowledge"> </a>

Se você usa o .NET Framework ou outra plataforma para desenvolver seu aplicativo de serviço Web, convém entender alguns conceitos importantes antes de começar seu projeto de desenvolvimento. 
  
**Tabela 1. Conceitos de serviços Web**

|**Conceito**|**Resumo**|
|:-----|:-----|
|[Arquitetura](ews-applications-and-the-exchange-architecture.md) <br/> |Saiba mais sobre como o EWS funciona dentro da arquitetura do Exchange e os protocolos que ele usa.  <br/> |
|[Tipos de aplicativo do EWS](ews-application-types.md) <br/> |Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.  <br/> |
|[Acesso ao EWS](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Os administradores do Exchange podem limitar o acesso ao EWS globalmente para toda a organização, para usuários individuais e para aplicativos individuais. Descubra o nível de acesso certo para você.  <br/> |
|[Configurar](setting-up-your-ews-application.md) <br/> |Encontre informações sobre as tarefas que precisam ser concluídas para criar aplicativos que usam a API gerenciada do EWS ou o EWS para se comunicar com o Exchange.  <br/> |
|[Autenticação](authentication-and-ews-in-exchange.md) <br/> |Saiba mais sobre as opções de autenticação para se conectar ao Exchange Online e ao Exchange local.  <br/> |
|[Descoberta Automática](autodiscover-for-exchange.md) <br/> |Saiba mais sobre o conjunto de serviços que você pode usar para descobrir o ponto de extremidade da URL onde a conta de um usuário pode acessar informações por meio do EWS.  <br/> |
|[Servidor de Caixa de Correio](https://technet.microsoft.com/library/jj150491%28v=exchg.150%29.aspx) <br/> |Saiba mais sobre o repositório principal de informações disponibilizadas para um cliente do EWS. O EWS tem acesso a um conjunto limitado de informações armazenadas nos serviços de domínio do Active Directory (AD DS).  <br/> |
|[Aplicativos de email para Outlook e EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Encontre informações sobre aplicativos de email para o Outlook e como eles funcionam com o EWS no Exchange.  <br/> |
|[APIs de restante do Office 365 para emails, calendários e contatos](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Saiba mais sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Exchange Online como parte do Office 365.  <br/> |
|[A API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md) <br/> |Encontre informações sobre a API do cliente preferencial para desenvolvedores do .NET Framework.  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |Encontre informações sobre como criar seu primeiro aplicativo usando solicitações e respostas XML do EWS.  <br/> |
|[Funcionalidade do EWS em versões de produtos do Exchange](ews-functionality-in-exchange-product-versions.md) <br/> |Descubra o que a funcionalidade do EWS está disponível na versão do Exchange.  <br/> |
|[Rastrear e solucionar problemas](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Descubra como rastrear solicitações e respostas do EWS para solucionar erros no seu aplicativo de API gerenciada do EWS.  <br/> |
   
## <a name="create-your-first-application"></a>Criar seu primeiro aplicativo
<a name="create"> </a>

Se você estiver pronto para obter o negócio de escrever seu primeiro aplicativo do .NET Framework ou do EWS, confira [introdução aos aplicativos clientes de API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md) ou [introdução aos aplicativos clientes do EWS](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Obter exemplos de código
<a name="samples"> </a>

Para encontrar exemplos de código e exemplos que mostram como trabalhar com o EWS e outros serviços Web no Exchange, consulte os seguintes recursos:
  
- [Exemplos de código do Exchange](https://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Documentação da API do Exchange](develop-web-service-clients-for-exchange.md)
    
- [Fórum de desenvolvimento do Exchange](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment)
    
Muitos outros exemplos estão disponíveis em Blogs, sites de demonstração de código e fóruns. Também recomendamos que você baixe o [EWSEditor](http://ewseditor.codeplex.com/). Este projeto implementa a maior parte da funcionalidade do EWS; Você pode encontrar exemplos de todas as funcionalidades principais do EWS aqui.
  
Se você não for um desenvolvedor do .NET Framework, poderá encontrar várias bibliotecas de cliente para o desenvolvimento do EWS que usam Java, Python, PHP e outros idiomas. 
  
## <a name="ask-questions-and-solve-problems"></a>Fazer perguntas e resolver problemas
<a name="questions"> </a>

Precisa de ajuda para realizar tarefas e você não está encontrando respostas? Você pode pesquisar no [Fórum de desenvolvimento do Exchange](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) para descobrir se alguém encontrou e solucionou o mesmo problema. Uma comunidade de colaboradores respondeu centenas de perguntas sobre o desenvolvimento do Exchange. Você também pode encontrar sites, fóruns e Blogs de terceiros que cobrem o desenvolvimento do Exchange e que podem ter a solução que você está procurando. 
  
Entre em contato com [o suporte da Microsoft](https://support.microsoft.com/) se precisar de mais ajuda. A equipe de suporte para desenvolvedores do Exchange é responsável por profissionais experientes que podem ajudar a responder suas perguntas sobre o desenvolvimento do Exchange. 
  
## <a name="see-also"></a>Confira também

- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md) 
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md) 
- [Referência de serviço Web do Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

