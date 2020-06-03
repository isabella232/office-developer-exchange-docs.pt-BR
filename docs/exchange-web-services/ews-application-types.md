---
title: Tipos de aplicativo do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 02bbe039adaec1054ab33f642f3bf14a7ba22b90
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455426"
---
# <a name="ews-application-types"></a>Tipos de aplicativo do EWS

Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.
  
A [arquitetura EWS e Exchange](ews-applications-and-the-exchange-architecture.md) fornece um modelo de desenvolvimento uniforme que você pode usar para criar os tipos mais comuns de aplicativos de uma maneira consistente, incluindo o seguinte: 
  
- [Aplicativos cliente](#bk_clientapps) — aplicativos autônomos que usam o EWS para acessar dados do Exchange. O Outlook e o Outlook Web App são exemplos de aplicativos cliente. 
    
- [Aplicativos de portal](#bk_portalapps) — aplicativos que estendem uma página da Web existente, incluindo informações recuperadas do Exchange, como informações de disponibilidade ou de contato. Uma Web Part do SharePoint que recupera os dados do Exchange é um exemplo de um aplicativo de Portal. 
    
- [Aplicativos de serviço](#bk_serviceapps) : trabalhos em segundo plano usados para integrar ou sincronizar dados do Exchange em um sistema existente. Por exemplo, um aplicativo que sincroniza informações de contato do Exchange para um aplicativo CRM. 
    
Cada um desses modelos de aplicativos pode usar uma base de código comum para recuperar informações do Exchange-para que você não precise alterar o código EWS usado para recuperar informações de item entre um cliente, portal ou aplicativo de serviço. O que pode ser alterado de um aplicativo para o próximo é o acesso de caixa de correio e o mecanismo de autenticação. Por exemplo, os aplicativos clientes normalmente usam o acesso direto de usuários e a autenticação básica ou NTLM, enquanto um aplicativo de serviço provavelmente usa representação para acesso de caixa de correio e autenticação OAuth.
  
## <a name="client-applications"></a>Aplicativos do cliente
<a name="bk_clientapps"> </a>

Um aplicativo cliente do EWS é qualquer aplicativo autônomo que use EWS para recuperar informações do repositório do Exchange. Os aplicativos clientes do EWS usam acesso direto para cliente ou acesso de representante para recuperar dados do armazenamento de caixa de correio. Veja a seguir alguns exemplos de aplicativos cliente que usam EWS:
  
- Outlook, em recursos como dicas de entrada, disponibilidade e status de ausência temporária do usuário
    
- OWA para dispositivos
    
- Outlook para Mac 2011
    
- Lync, para informações de disponibilidade
    
Os aplicativos clientes normalmente usam o acesso direto e a autenticação básica ou NTLM, de forma que os usuários estejam limitados a acessar informações em suas próprias caixas de correio com suas próprias credenciais de logon. Os aplicativos cliente também devem oferecer suporte ao acesso de representante para usuários que receberam permissão para acessar a caixa de correio de outro usuário.
  
## <a name="portal-applications"></a>Aplicativos de portal
<a name="bk_portalapps"> </a>

Um aplicativo de portal estende uma página da Web existente ou portal para incluir informações de caixa de correio do Exchange como um componente personalizado da página. As Web Parts do SharePoint são os aplicativos de portal mais comuns e fornecem aos usuários uma experiência personalizada ao fornecer modos de exibição aos dados de caixa de correio do Exchange, como mensagens não lidas, mensagens mais recentes e eventos de calendário, juntamente com a página do portal SharePoint comumente vista. Os aplicativos do portal EWS podem usar o acesso para cliente direto, o acesso de representante ou a representação para recuperar dados do armazenamento de caixa de correio. Como o Exchange 2013 e o SharePoint 2013 dão suporte ao protocolo de autorização OAuth para autenticação de servidor para servidor, o OAuth fornece o método de autenticação mais simples e seguro.
  
## <a name="service-applications"></a>Aplicativos de serviço
<a name="bk_serviceapps"> </a>

Um aplicativo de serviço geralmente é um trabalho em segundo plano incorporado a um aplicativo existente que se estende ao Exchange para correlacionar dados entre o sistema e o repositório do Exchange. Os aplicativos de serviço normalmente não têm uma interface de usuário e usam representação ou OAuth para autenticação e acesso. A criação de uma conta de serviço para representar usuários é comum nos aplicativos do serviço EWS, pois você pode conceder a uma única permissão de conta para representar um conjunto de usuários e realizar operações de caixa de correio para essas contas. Por exemplo, um aplicativo de serviço do EWS pode sincronizar dados entre listas de marketing em uma solução CRM e grupos de distribuição do Exchange usando uma conta de serviço e representação.
  
## <a name="see-also"></a>Confira também


- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Aplicativos EWS e a arquitetura do Exchange](ews-applications-and-the-exchange-architecture.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

