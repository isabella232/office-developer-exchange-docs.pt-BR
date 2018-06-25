---
title: Migrando para tecnologias do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Se você estiver migrando de uma versão anterior do Exchange, use as informações neste artigo para descobrir quais tecnologias de desenvolvimento são suportadas nas versões de produto atual e migrar para o qual tecnologia.
ms.openlocfilehash: 82362b7bcdb79d6ca43603335d51a8bd8c1df239
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750994"
---
# <a name="migrating-to-exchange-technologies"></a>Migrando para tecnologias do Exchange

Se você estiver migrando de uma versão anterior do Exchange, use as informações neste artigo para descobrir quais tecnologias de desenvolvimento são suportadas nas versões de produto atual e migrar para o qual tecnologia.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Determinar se a sua tecnologia está disponível em versões atuais

Use a tabela a seguir para determinar se uma tecnologia de desenvolvimento é suportada no Exchange Online ou Exchange 2013. Se não há suporte para a tecnologia, consulte [Escolher uma tecnologia de desenvolvimento para migrar para o](#bk_choose).

<br/> 

**Versões de produtos e tecnologias de desenvolvimento do Exchange**

|Tecnologia|Office 365 e o Exchange Online|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|
|[Visão geral da plataforma APIs do Office 365](http://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> ||||
|[API gerenciada do EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Serviços Web do Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Aplicativos de email para Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |||
|[Modelo de objeto do Outlook (memória Insuficiente)](http://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Backup e restauração](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |
|[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |
|Interface de serviços do Active Directory (ADSI)  <br/> ||||X  <br/> |
|Objetos de dados de colaboração para Exchange (CDOEX)  <br/> ||||X  <br/> |
|Objetos de dados de colaboração para Windows 2000 (CDOSYS)  <br/> ||||X  <br/> |
|Provedor Exchange OLE DB (EXOLEDB)  <br/> ||||X  <br/> |
|Receptores de evento de armazenamento do Exchange  <br/> ||||X  <br/> |
|Sincronização de alteração incremental (ICS)  <br/> ||||X  <br/> |
|Lightweight Directory Access Protocol (LDAP)  <br/> ||||X  <br/> |
|[API de mensagem (MAPI)](http://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Personalização do Outlook Web App  <br/> |||X  <br/> ||
|Web distribuída Authoring and Versioning (WebDAV)  <br/> ||||X  <br/> |

<a name="bk_choose"> </a>

## <a name="choose-a-development-technology-to-migrate-to"></a>Escolha uma tecnologia de desenvolvimento para migrar para o

Se o seu aplicativo usa a tecnologia não é suportada ou deemphasized no Exchange Online ou Exchange 2013, use a tabela a seguir para decidir qual tecnologia para migrar para o.
  
**Caminhos de migração de tecnologia recomendada**

|**Tecnologia**|**Suportados no Office 365, Exchange Online e Exchange 2013?**|**Migrar para o**|**Mais informações**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |Sim, mas deemphasized <br/>|[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md)<br/> |Nenhum.  <br/> |
|CDOEX  <br/> |Não  <br/> |[API ou EWS gerenciada de EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API gerenciada de EWS e EWS podem acessar o mesmo armazenamento do Exchange que fornece CDOEX. Diferentemente dos aplicativos cliente criados usando o CDOEX, você pode executar aplicativos de EWS em um computador local ou remoto.  <br/> |
|CDOEXM  <br/> |Não <br/> |[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) <br/> |Comandos do Shell de gerenciamento do Exchange controle servidores Exchange, grupos de armazenamento, bancos de dados e os usuários mais simples que as APIs de CDOEXM correspondente. Além disso, você pode facilmente migrar seus aplicativos CDOEXM aos comandos do Shell de gerenciamento do Exchange.  <br/> |
|CDOSYS<br/> |Não<br/> |[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Use os agentes de transporte para aplicativos baseados em notificação que trabalham com as versões do Exchange, começando com o Exchange 2010.<br/><br/> CDOSYS está incluído em versões atuais do Windows. A funcionalidade do CDOSYS está disponível no .NET Framework.  <br/> |
|CDPWF  <br/> |Não  <br/> |[O Windows Workflow Foundation (WWF)](http://msdn.microsoft.com/en-us/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Você pode usar o WWF para criar aplicativos de fluxo de trabalho avançada que funcionam com o Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Não  <br/> |[API ou EWS gerenciada de EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API gerenciada de EWS e EWS fornecem o mesmo acesso ao armazenamento do Exchange que fornece ExOLEDB. Diferentemente dos aplicativos cliente criados usando o ExOLEDB, você pode executar aplicativos de EWS em um computador local ou remoto.  <br/> |
|ICS  <br/> |Sim, mas deemphasized  <br/> |API ou EWS gerenciada de EWS<br/> |Você pode usar a API gerenciada de EWS ou o EWS para [assinar notificações](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) e [sincronizar os dados de caixa de correio](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).  <br/> |
|LDAP  <br/> |Sim, mas deemphasized  <br/> |[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) <br/> |Nenhum.  <br/> |
|MAPI  <br/> |Sim, mas deemphasized  <br/> |O Office 365 APIs visão geral da plataforma, EWS Managed API, EWS <br/> |Embora o MAPI estiver atualmente uma tecnologia de desenvolvimento com suporte, você terá eventualmente reconstruir seus aplicativos MAPI para usar uma tecnologia mais recente.<br/><br/>Se seu aplicativo MAPI está executando simple leitura, gravação e operações de atualização no email, calendário, ou objetos de contato e destinos de Office 365, você pode usar as [APIs do Office 365 REST para emails, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Se você está direcionando Exchange local e você precisa acessar todas as propriedades que pode ser acessados por MAPI, você pode usar a API gerenciada de EWS ou EWS e ambos [esquematizado propriedades ou propriedades estendidas](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Observação**: A classe [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fornece acesso à MAPI da API gerenciada do EWS e o elemento [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) fornece acesso às propriedades MAPI do EWS.           |
|Personalização do Outlook Web App  <br/> |Não  <br/> |[Aplicativos de email](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Nenhum.  <br/> |
|Receptores de evento do repositório  <br/> |Não  <br/> |API ou EWS gerenciada de EWS <br/> |Você pode usar a API gerenciada de EWS ou o EWS para [assinar notificações](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) e [sincronizar os dados de caixa de correio](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).<br/><br/>As notificações de EWS fornecem o mesmo acesso ao armazenamento do Exchange que fornecem de receptores de evento do repositório. Você pode usar as ferramentas do Visual Studio para simplificar o desenvolvimento de aplicativos de reconhecimento de evento do cliente do repositório que usam o EWS.  <br/> |
|Streaming de backup e restauração  <br/> |Não  <br/> |[Gravador de serviço de cópia de sombra (VSS) de volume](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Nenhum.  <br/> |
|WebDAV  <br/> |Não  <br/> |O Office 365 APIs visão geral da plataforma, API gerenciada de EWS ou EWS <br/> |Se seu aplicativo WebDAV está executando as operações de atualização em email, calendário ou objetos de contato, gravação e leitura simple e você terá como destino Office 365, use as [APIs do Office 365 REST para emails, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Caso contrário, se você está direcionando Exchange local e você precisa acessar as mesmas propriedades no armazenamento do Exchange que WebDAV fornece, use a API gerenciada de EWS ou EWS.  <br/> |
|Notificações de WebDAV  <br/> |Não  <br/> |API ou EWS gerenciada de EWS<br/> |Você pode usar a API gerenciada de EWS ou o EWS para [assinar notificações](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md).  <br/> |
|Formulários da Web  <br/> |Não  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Alterne para o ASP.NET e atualizar os aplicativos para acessar informações de caixa de correio e de servidor usando o EWS.  <br/> |
|Provedores WMI  <br/> |Não  <br/> |[Shell de Gerenciamento do Exchange](management/exchange-management-shell.md) <br/> |Nenhum.  <br/> |
   
## <a name="see-also"></a>Ver também

- [Selecionando uma API ou tecnologia para desenvolver soluções para o Outlook](http://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
    

