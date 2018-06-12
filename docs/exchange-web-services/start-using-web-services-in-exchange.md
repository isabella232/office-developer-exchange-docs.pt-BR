---
title: Começar a usar os serviços web no Exchange
manager: sethgros
ms.date: 2/27/2017
ms.audience: Developer
localization_priority: Normal
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Encontre informações para ajudá-lo a começar a usar EWS e outros serviços web do Exchange.
ms.openlocfilehash: 2f203c5634c29105feb39220c3ebdd9624bb49ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750953"
---
# <a name="start-using-web-services-in-exchange"></a>Começar a usar os serviços web no Exchange

Encontre informações para ajudá-lo a começar a usar EWS e outros serviços web do Exchange.
  
O [web services no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)fornecem acesso aos dados de caixa de correio armazenada no Exchange Online, Exchange Online como parte do Office 365 e a versões locais do Exchange, começando com o Exchange Server 2007 e permitem a criação de aplicativos personalizados que você pode usar Use para gerenciar essas informações de acordo com os requisitos da sua organização. Enquanto o intervalo de aplicativos de serviço do EWS e web que você pode criar é praticamente infinito, aplicam o determinados conceitos fundamentais para qualquer tipo de aplicativo. Esta seção fornece informações sobre os conceitos fundamentais que você precisa estar familiarizado com para começar a usar o EWS e outros serviços web do Exchange. 
  
## <a name="build-your-knowledge"></a>Criar seus conhecimentos
<a name="bk_Knowledge"> </a>

Se você usar o .NET Framework ou outra plataforma para desenvolver seu aplicativo de serviço web, convém entender alguns conceitos importantes antes de começar seu projeto de desenvolvimento. 
  
**Tabela 1. Conceitos de serviços da Web**

|**Conceito**|**Resumo**|
|:-----|:-----|
|[Arquitetura](ews-applications-and-the-exchange-architecture.md) <br/> |Saiba mais sobre o funcionamento do EWS dentro da arquitetura do Exchange e os protocolos que ela usa.  <br/> |
|[Tipos de aplicativos do EWS](ews-application-types.md) <br/> |Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.  <br/> |
|[Acesso EWS](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Os administradores do Exchange podem limitar o acesso aos EWS globalmente para toda a organização, para usuários individuais e a aplicativos individuais. Descobrir qual nível de acesso é o certo para você.  <br/> |
|[Setup](setting-up-your-ews-application.md) <br/> |Encontre informações sobre as tarefas que você precisa concluir para criar aplicativos que usam a API gerenciada de EWS ou o EWS para se comunicar com o Exchange.  <br/> |
|[Autenticação](authentication-and-ews-in-exchange.md) <br/> |Saiba mais sobre as opções de autenticação para se conectar ao Exchange Online e do Exchange local.  <br/> |
|[Descoberta automática](autodiscover-for-exchange.md) <br/> |Saiba mais sobre o conjunto de serviços que você pode usar para descobrir o ponto de extremidade de URL em que uma conta de usuário pode acessar informações via EWS.  <br/> |
|[Servidor de caixa de correio](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx) <br/> |Saiba mais sobre o repositório principal de informações disponibilizados para um cliente do EWS. EWS tem acesso a um limitado a conjunto das informações armazenadas nos serviços de domínio Active Directory (AD DS).  <br/> |
|[Aplicativos de email para o Outlook e o EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Encontre informações sobre aplicativos de email para o Outlook e como eles funcionam com o EWS no Exchange.  <br/> |
|[APIs de restante do Office 365 para emails, calendários e contatos](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Saiba mais sobre as APIs do Office 365 que você pode usar para acessar email, calendários e contatos no Exchange Online como parte do Office 365.  <br/> |
|[A API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md) <br/> |Encontre informações sobre a API do cliente preferencial para desenvolvedores do .NET Framework.  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |Encontre informações sobre como criar seu primeiro aplicativo usando o EWS XML solicitações e respostas.  <br/> |
|[Funcionalidade do EWS nas versões de produto do Exchange](ews-functionality-in-exchange-product-versions.md) <br/> |Descobrir qual funcionalidade EWS está disponível na versão do Exchange.  <br/> |
|[Rastrear e solucionar problemas](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Descubra como EWS solicitações e respostas para solucionar erros no seu aplicativo do EWS Managed API de rastreamento.  <br/> |
   
## <a name="create-your-first-application"></a>Crie seu primeiro aplicativo
<a name="create"> </a>

Se você estiver pronto para ir para a empresa de criar seu primeiro .NET Framework ou um aplicativo cliente do EWS, consulte [Introdução ao aplicativos cliente do EWS Managed API](get-started-with-ews-managed-api-client-applications.md) ou [começar com os aplicativos de cliente do EWS](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Obter exemplos de código
<a name="samples"> </a>

Para obter exemplos de códigos e exemplos que mostram como trabalhar com outros serviços da web e de EWS no Exchange, consulte os seguintes recursos:
  
- [Amostras de código do Exchange](http://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Documentação da API do Exchange](develop-web-service-clients-for-exchange.md)
    
- [Fórum de desenvolvimento do Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)
    
Muitos outros exemplos estão disponíveis em blogs, fóruns e sites de demonstração do código. Também recomendamos que você baixe o [EWSEditor](http://ewseditor.codeplex.com/). Esse projeto implementa a maioria das funcionalidades EWS; Você pode encontrar exemplos de todos os a funcionalidade básica do EWS aqui.
  
Se você não for um desenvolvedor do .NET Framework, você pode encontrar muitas bibliotecas de cliente por aí para desenvolvimento do EWS que usam o Java, Python, PHP e outros idiomas. 
  
## <a name="ask-questions-and-solve-problems"></a>Faça perguntas e resolver problemas
<a name="questions"> </a>

Precisa de ajuda para obter suas tarefas e você não estiver encontrando respostas? Você pode pesquisar o [Fórum de desenvolvimento do Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) para descobrir a outra pessoa tiver encontrado e resolvido o mesmo problema. Uma comunidade de colaboradores atendeu centenas de perguntas sobre o desenvolvimento do Exchange. Você também pode encontrar sites de terceiros, fóruns e blogs que abrangem o desenvolvimento do Exchange e podem ter a solução que você está procurando. 
  
Contate o [suporte da Microsoft](https://support.microsoft.com/) se precisar de assistência adicional. A equipe de suporte do desenvolvedor do Exchange é formada por profissionais experientes que podem ajudar a responder às suas perguntas sobre o desenvolvimento do Exchange. 
  
## <a name="see-also"></a>Confira também

- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md) 
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md) 
- [Referência de serviços Web do Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

