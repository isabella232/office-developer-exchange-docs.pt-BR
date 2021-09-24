---
title: 'Migrar para as tecnologias do Exchange '
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Se você estiver migrando de uma versão anterior do Exchange, use as informações deste artigo para descobrir quais tecnologias de desenvolvimento são suportadas nas versões atuais do produto e para qual tecnologia migrar.
ms.openlocfilehash: 3885d6789cedf5de028b64a0658b336bd021b9ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526998"
---
# <a name="migrating-to-exchange-technologies"></a>Migrar para as tecnologias do Exchange 

Se você estiver migrando de uma versão anterior do Exchange, use as informações deste artigo para descobrir quais tecnologias de desenvolvimento são suportadas nas versões atuais do produto e para qual tecnologia migrar.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Determinar se sua tecnologia está disponível nas versões atuais

Use a tabela a seguir para determinar se uma tecnologia de desenvolvimento tem suporte no Exchange Online ou Exchange 2019. Se a tecnologia não for suportada, consulte [Choose a development technology to migrate to](#bk_choose).

<br/> 

**Exchange de desenvolvimento e versões do produto**

|Tecnologia|Office 365 e Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Visão geral da plataforma de APIs do Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X²  <br/> |X ²  <br/> ||
|[API Gerenciada do EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Serviços Web do Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Aplicativos de email para Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Outlook Modelo de Objeto (OOM)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Backup and restore](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Interface de Serviços do Active Directory (ADSI)  <br/> ||||||X  <br/> |
|Objetos de dados colaborativos para Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Objetos de dados colaborativos Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Exchange Provedor OLE DB (EXOLEDB)  <br/> ||||||X  <br/> |
|Exchange Pias de Eventos da Loja  <br/> ||||||X  <br/> |
|Sincronização de Alterações Incrementais (ICS)  <br/> ||||||X  <br/> |
|Protocolo LDAP  <br/> ||||||X  <br/> |
|[API de Mensagens (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Outlook Web App personalização  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

A API ¹REST e Graph api exigem a Atualização Cumulativa 3 para Exchange 2016.

²Only os clientes híbridos são capazes de tirar proveito das APIs REST para caixas de correio Office 365 e locais.

## <a name="choose-a-development-technology-to-migrate-to"></a>Escolha uma tecnologia de desenvolvimento para a qual migrar

Se a tecnologia usada pelo aplicativo não for suportada ou desemphasized no Exchange Online ou Exchange 2013, use a tabela a seguir para decidir para qual tecnologia migrar.
  
**Caminhos de migração de tecnologia recomendados**

|**Tecnologia**|**Com suporte em Office 365, Exchange Online e Exchange 2019?**|**Migrar para**|**Informações adicionais**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |Sim, mas desemphasized <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |Nenhum.  <br/> |
|CDOEX  <br/> |Não  <br/> |[EWS Managed API ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API Gerenciada EWS e o EWS podem acessar o mesmo Exchange que o CDOEX fornece. Ao contrário dos aplicativos cliente construídos usando CDOEX, você pode executar aplicativos EWS em um computador local ou remoto.  <br/> |
|CDOEXM  <br/> |Não <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Exchange Comandos do Shell de Gerenciamento controlam Exchange servidores, grupos de armazenamento, bancos de dados e usuários mais simples do que as APIs CDOEXM correspondentes. Além disso, você pode migrar facilmente seus aplicativos CDOEXM para Exchange comandos do Shell de Gerenciamento.  <br/> |
|CDOSYS<br/> |Não<br/> |[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Use agentes de transporte para aplicativos baseados em notificação que funcionam com versões de Exchange começando com Exchange 2010.<br/><br/> O CDOSYS está incluído nas versões atuais do Windows. A funcionalidade no CDOSYS está disponível no .NET Framework.  <br/> |
|CDOWF  <br/> |Não  <br/> |[Windows Workflow Foundation (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Você pode usar o WWF para criar aplicativos de fluxo de trabalho avançados que funcionam com Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Não  <br/> |[EWS Managed API ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API Gerenciada EWS e o EWS fornecem o mesmo acesso ao Exchange que o ExOLEDB fornece. Ao contrário dos aplicativos cliente criado usando o ExOLEDB, você pode executar aplicativos EWS em um computador local ou remoto.  <br/> |
|ICS  <br/> |Sim, mas desemphasized  <br/> |EWS Managed API ou EWS<br/> |Você pode usar a API Gerenciada do EWS ou o EWS para [assinar](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) notificações e [sincronizar dados de caixa de correio.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)  <br/> |
|LDAP  <br/> |Sim, mas desemphasized  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Nenhum.  <br/> |
|MAPI  <br/> |Sim, mas desemphasized  <br/> |Office 365 Visão geral da plataforma APIs, API Gerenciada do EWS, EWS <br/> |Embora a MAPI seja atualmente uma tecnologia de desenvolvimento com suporte, você eventualmente terá que redesenhar seus aplicativos MAPI para usar uma tecnologia mais nova.<br/><br/>Se seu aplicativo MAPI estiver executando operações simples de leitura, gravação e atualização em objetos de email, calendário ou contato e destinos do Office 365, Exchange 2019² ou Exchange 2016 ², você poderá usar as APIs REST do Office 365 para [email, calendários](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)e contatos.<br/><br/>Se você estiver direcionando Exchange local e precisar acessar todas as propriedades que MAPI pode acessar, você pode usar a API Gerenciada EWS ou EWS e propriedades [eschematizadas](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)ou propriedades estendidas.<br/><br/>**OBSERVAÇÃO**: A [classe ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fornece acesso ao MAPI da API Gerenciada do EWS e o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) fornece acesso às propriedades MAPI do EWS.           |
|Outlook Web App personalização  <br/> |Não  <br/> |[Aplicativos de email](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Nenhum.  <br/> |
|Pias de eventos da Loja  <br/> |Não  <br/> |EWS Managed API ou EWS <br/> |Você pode usar a API Gerenciada do EWS ou o EWS para [assinar](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) notificações e [sincronizar dados de caixa de correio.](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)<br/><br/>As notificações no EWS fornecem o mesmo acesso ao Exchange que os pias de eventos da loja fornecem. Você pode usar Visual Studio ferramentas para simplificar o desenvolvimento de aplicativos cliente cientes de eventos da loja que usam o EWS.  <br/> |
|Backup e restauração de streaming  <br/> |Não  <br/> |[Escritor do Serviço de Cópia de Sombra de Volume (VSS)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Nenhum.  <br/> |
|WebDAV  <br/> |Não  <br/> |Office 365 Visão geral da plataforma APIs, API Gerenciada do EWS ou EWS <br/> |Se seu aplicativo WebDAV estiver executando operações simples de leitura, gravação e atualização em objetos de email, calendário ou contato, e você estará direcionando o Office 365, o Exchange 2019² ou o Exchange 2016 ², você pode usar as APIs REST Office 365 para [email, calendários](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)e contatos.<br/><br/>Caso contrário, se você estiver direcionando Exchange local e precisar acessar as mesmas propriedades no armazenamento Exchange que o WebDAV fornece, use a API Gerenciada do EWS ou o EWS.  <br/> |
|Notificações do WebDAV  <br/> |Não  <br/> |EWS Managed API ou EWS<br/> |Você pode usar a API Gerenciada do EWS ou o EWS para [assinar as notificações](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md).  <br/> |
|Formulários Web  <br/> |Não  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Alternar para ASP.NET e atualizar aplicativos para acessar informações de caixa de correio e servidor usando o EWS.  <br/> |
|Provedores WMI  <br/> |Não  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Nenhum.  <br/> |
   
A API ¹REST e Graph api exigem a Atualização Cumulativa 3 para Exchange 2016.

²Only os clientes híbridos são capazes de tirar proveito das APIs REST para caixas de correio Office 365 e locais.

## <a name="see-also"></a>Confira também

- [Escolher uma API ou tecnologia para desenvolver soluções para o Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Requisitos de arquitetura local para a API REST](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
