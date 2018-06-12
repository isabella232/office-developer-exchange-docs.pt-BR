---
title: Tipos de aplicativos do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.
ms.openlocfilehash: 1ce739f453ba1bc6f1b5d38edae3776daa562ffb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750653"
---
# <a name="ews-application-types"></a>Tipos de aplicativos do EWS

Saiba mais sobre os tipos mais comuns de aplicativos que você pode criar usando o EWS no Exchange.
  
A [arquitetura do EWS e Exchange](ews-applications-and-the-exchange-architecture.md) oferece um modelo de desenvolvimento uniforme que você pode usar para criar os tipos mais comuns de aplicativos de forma consistente, incluindo o seguinte: 
  
- [Aplicativos cliente](#bk_clientapps) — aplicativos autônomos que usam o EWS para acessar dados do Exchange. Outlook e Outlook Web App são exemplos de aplicativos cliente. 
    
- [Aplicativos de portal](#bk_portalapps) — aplicativos que estendem a uma página da web existente, incluindo as informações recuperadas do Exchange, como informações de livre/ocupado ou contatos. Uma web part do SharePoint que recupera os dados do Exchange é um exemplo de um aplicativo de portal. 
    
- [Aplicativos de serviço](#bk_serviceapps) — usados para integrar ou sincronizar os dados do Exchange em um sistema existente de trabalhos em segundo plano. Por exemplo, um aplicativo que sincroniza as informações de contato do Exchange em um aplicativo CRM. 
    
Cada um desses modelos de aplicativo pode usar uma base de código comum para recuperar informações do Exchange -, portanto você não precisa alterar o código do EWS usado para recuperar informações de item entre um cliente, portal ou aplicativo de serviço. O que pode mudar de um aplicativo para o próximo é o mecanismo de autenticação e acesso de caixa de correio. Por exemplo, aplicativos clientes normalmente usam acesso direto do usuário e básica ou autenticação NTLM, enquanto um aplicativo de serviço provavelmente usa a representação para acesso de caixa de correio e a autenticação OAuth.
  
## <a name="client-applications"></a>Aplicativos cliente
<a name="bk_clientapps"> </a>

Um aplicativo cliente do EWS é qualquer aplicativo autônomo que usa o EWS para recuperar as informações de armazenamento do Exchange. Aplicativos cliente do EWS usam acesso para cliente direto ou acesso de representante ao recuperar dados do repositório de caixa de correio. Eis alguns exemplos de aplicativos de cliente que usam o EWS:
  
- Outlook, em recursos, como disponibilidade, dicas de email e usuário status de ausência temporária
    
- OWA para Dispositivos
    
- Outlook para Mac 2011
    
- Lync, para obter informações de disponibilidade
    
Aplicativos clientes frequentemente usam acesso direto e básica ou autenticação NTLM, para que os usuários estão limitados para acessar informações em sua própria caixa de correio com suas próprias credenciais de logon. Também devem oferecer suporte a aplicativos cliente Delegar acesso para usuários que tiverem permissão para acessar a caixa de correio de outro usuário.
  
## <a name="portal-applications"></a>Aplicativos de portal
<a name="bk_portalapps"> </a>

Um aplicativo de portal estende a uma página da web existente ou portal para incluir informações de caixa de correio do Exchange como um componente personalizado da página. Web parts do SharePoint são os aplicativos mais comuns de portal e fornecem aos usuários uma experiência personalizada, fornecendo os modos de exibição em dados de caixa de correio do Exchange, como mensagens não lidas, as mensagens mais recentes e eventos de calendário, junto com seus comumente visualizado Página do portal do SharePoint. Aplicativos de portal do EWS podem usar o acesso de cliente direta, acesso de representante ou representação para recuperar dados do repositório de caixa de correio. Como o Exchange 2013 e SharePoint 2013 suportem o protocolo de autorização do OAuth para autenticação de servidor-para-servidor, o OAuth fornece o método de autenticação mais seguro e sem interrupções.
  
## <a name="service-applications"></a>Aplicativos de serviço
<a name="bk_serviceapps"> </a>

Normalmente, um aplicativo de serviço é um trabalho de plano de fundo incorporado a um aplicativo existente que se estende para o Exchange para correlacionar dados entre o sistema e o armazenamento do Exchange. Aplicativos de serviço geralmente não têm uma interface de usuário e usar representação ou OAuth para autenticação e acesso. Criar uma conta de serviço para representar usuários é comum em aplicativos de serviço do EWS, porque é possível conceder uma permissão única conta para representar um conjunto de usuários e realizar operações de caixa de correio para essas contas. Por exemplo, um aplicativo de serviço do EWS pode sincronizar dados entre marketing listas em uma solução CRM e grupos de distribuição do Exchange, usando uma conta de serviço e a representação.
  
## <a name="see-also"></a>Confira também


- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Aplicativos do EWS e arquitetura do Exchange](ews-applications-and-the-exchange-architecture.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

