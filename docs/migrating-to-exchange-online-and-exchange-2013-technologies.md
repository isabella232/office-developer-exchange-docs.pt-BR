---
title: 'Migrar para as tecnologias do Exchange '
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Se você estiver migrando de uma versão anterior do Exchange, use as informações deste artigo para descobrir quais tecnologias de desenvolvimento são compatíveis com as versões atuais do produto e em qual tecnologia migrar.
ms.openlocfilehash: d82f1b305fd1cc30e48cddbf9bf2981d3d829a5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459150"
---
# <a name="migrating-to-exchange-technologies"></a>Migrar para as tecnologias do Exchange 

Se você estiver migrando de uma versão anterior do Exchange, use as informações deste artigo para descobrir quais tecnologias de desenvolvimento são compatíveis com as versões atuais do produto e em qual tecnologia migrar.
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>Determinar se sua tecnologia está disponível nas versões atuais

Use a tabela a seguir para determinar se uma tecnologia de desenvolvimento é compatível com o Exchange Online ou o Exchange 2019. Se não houver suporte para a tecnologia, confira [escolher uma tecnologia de desenvolvimento para migrar para](#bk_choose)o.

<br/> 

**Tecnologias de desenvolvimento do Exchange e versões do produto**

|Tecnologia|Office 365 e Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Visão geral da plataforma de APIs do Office 365](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X ²  <br/> |X ¹ ²  <br/> ||
|[API gerenciada do EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Serviços Web do Exchange (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Aplicativos de email para Outlook](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[OOM (modelo de objeto do Outlook)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Backup and restore](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Interface de serviços do Active Directory (ADSI)  <br/> ||||||X  <br/> |
|Objetos de dados de colaboração para Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Objetos de dados de colaboração para o Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Provedor OLE DB do Exchange (EXOLEDB)  <br/> ||||||X  <br/> |
|Coletores de eventos do repositório do Exchange  <br/> ||||||X  <br/> |
|Sincronização de alteração incremental (ICS)  <br/> ||||||X  <br/> |
|Protocolo LDAP  <br/> ||||||X  <br/> |
|[API de mensagens (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Personalização do Outlook Web App  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|WebDAV (criação e versão distribuídas na Web)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

API REST do ¹ e API do Graph exigem a atualização cumulativa 3 para o Exchange 2016.

² somente clientes híbridos podem tirar proveito das APIs REST para o Office 365 e caixas de correio locais.

## <a name="choose-a-development-technology-to-migrate-to"></a>Escolha uma tecnologia de desenvolvimento para migrar para o

Se a tecnologia que seu aplicativo usa não é suportada ou não foi enfatizada no Exchange Online ou no Exchange 2013, use a tabela a seguir para decidir de qual tecnologia migrar.
  
**Caminhos recomendados de migração de tecnologia**

|**Tecnologia**|**Com suporte no Office 365, Exchange Online e Exchange 2019?**|**Migrar para**|**Mais informações**|
|:-----|:-----|:-----|:-----|
|EDITOR  <br/> |Sim, mas não enfatizado <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |Nenhum  <br/> |
|CDOEX  <br/> |Não  <br/> |[API gerenciada do EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API gerenciada do EWS e o EWS podem acessar o mesmo repositório do Exchange que o CDOEX fornece. Diferentemente dos aplicativos cliente criados com o uso de CDOEX, você pode executar aplicativos EWS em um computador local ou remoto.  <br/> |
|CDOEXM  <br/> |Não <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Os comandos do Shell de gerenciamento do Exchange controlam os servidores do Exchange, grupos de armazenamento, bancos de dados e usuários mais simples do que as APIs do CDOEXM correspondentes. Além disso, você pode migrar facilmente seus aplicativos do CDOEXM para os comandos do Shell de gerenciamento do Exchange.  <br/> |
|CDOSYS<br/> |Não<br/> |[Agentes de transporte](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Use agentes de transporte para aplicativos baseados em notificação que funcionam com versões do Exchange a partir do Exchange 2010.<br/><br/> O CDOSYS está incluído nas versões atuais do Windows. A funcionalidade no CDOSYS está disponível no .NET Framework.  <br/> |
|CDPWF  <br/> |Não  <br/> |[Windows Workflow Foundation (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |Você pode usar o WWF para criar aplicativos avançados de fluxo de trabalho que funcionam com o Exchange 2007.   <br/> |
|ExOLEDB  <br/> |Não  <br/> |[API gerenciada do EWS ou EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |A API gerenciada do EWS e o EWS fornecem o mesmo acesso ao repositório do Exchange que o EXOLEDB fornece. Diferentemente dos aplicativos cliente criados com o uso do EXOLEDB, você pode executar aplicativos EWS em um computador local ou remoto.  <br/> |
|PARTILHA  <br/> |Sim, mas não enfatizado  <br/> |API gerenciada do EWS ou EWS<br/> |Você pode usar a API gerenciada do EWS ou o EWS para [inscrever-](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) se nas notificações e [sincronizar os dados da caixa de correio](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).  <br/> |
|LDAP  <br/> |Sim, mas não enfatizado  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Nenhum  <br/> |
|MAPI  <br/> |Sim, mas não enfatizado  <br/> |Visão geral da plataforma de APIs do Office 365, API gerenciada do EWS, EWS <br/> |Embora o MAPI seja atualmente uma tecnologia de desenvolvimento com suporte, você precisará reprojetar seus aplicativos MAPI para usar uma tecnologia mais recente.<br/><br/>Se seu aplicativo MAPI estiver executando operações de leitura, gravação e atualização simples em emails, calendário ou objetos de contato e direcionar o Office 365, Exchange 2019 ² ou Exchange 2016 ¹ ², você poderá usar as [APIs REST do office 365 para emails, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Se você estiver direcionando o Exchange no local e precisar acessar todas as propriedades que o MAPI pode acessar, você poderá usar a API gerenciada do EWS ou o EWS e [as propriedades esquematizado ou estendidas](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).<br/><br/>**Observação**: a classe [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) fornece acesso a MAPI da API gerenciada do EWS, e o elemento [EXTENDEDFIELDURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) fornece acesso a propriedades MAPI do EWS.           |
|Personalização do Outlook Web App  <br/> |Não  <br/> |[Aplicativos de email](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Nenhum  <br/> |
|Coletar coletores de eventos  <br/> |Não  <br/> |API gerenciada do EWS ou EWS <br/> |Você pode usar a API gerenciada do EWS ou o EWS para [inscrever-](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) se nas notificações e [sincronizar os dados da caixa de correio](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).<br/><br/>As notificações no EWS fornecem o mesmo acesso ao repositório do Exchange que o armazenamento de coletores de eventos fornece. Você pode usar as ferramentas do Visual Studio para simplificar o desenvolvimento de aplicativos clientes de reconhecimento de eventos de armazenamento que usam o EWS.  <br/> |
|Backup e restauração de fluxo  <br/> |Não  <br/> |[Gravador VSS (serviço de cópias de sombra de volume)](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |Nenhum  <br/> |
|Version  <br/> |Não  <br/> |Visão geral da plataforma de APIs do Office 365, API gerenciada do EWS ou EWS <br/> |Se seu aplicativo WebDAV estiver executando operações de leitura, gravação e atualização simples nos objetos mail, Calendar ou Contact, e você será direcionado para o Office 365, Exchange 2019 ² ou Exchange 2016 ¹ ², poderá usar as [APIs REST do office 365 para emails, calendários e contatos](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).<br/><br/>Caso contrário, se você estiver direcionando o Exchange no local e precisar de acesso às mesmas propriedades no repositório do Exchange que o WebDAV fornece, use a API gerenciada do EWS ou o EWS.  <br/> |
|Notificações WebDAV  <br/> |Não  <br/> |API gerenciada do EWS ou EWS<br/> |Você pode usar a API gerenciada do EWS ou o EWS para [inscrever-](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)se nas notificações.  <br/> |
|Formulários da Web  <br/> |Não  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |Alterne para o ASP.NET e atualize os aplicativos para acessar as informações de caixa de correio e servidor usando o EWS.  <br/> |
|Provedores WMI  <br/> |Não  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Nenhum  <br/> |
   
API REST do ¹ e API do Graph exigem a atualização cumulativa 3 para o Exchange 2016.

² somente clientes híbridos podem tirar proveito das APIs REST para o Office 365 e caixas de correio locais.

## <a name="see-also"></a>Confira também

- [Escolher uma API ou tecnologia para desenvolver soluções para o Outlook](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [Requisitos de arquitetura local para a API REST](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
