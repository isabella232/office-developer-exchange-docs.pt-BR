---
title: Opções de configuração do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Encontre informações sobre as definições de configuração que o cliente do EWS pode acessar e as configurações configuráveis do Exchange que podem afetar seu cliente do EWS.
ms.openlocfilehash: 55f927b7b301bdfaa298bcd254b18a00cf1692d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456154"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Opções de configuração do EWS no Exchange

Encontre informações sobre as definições de configuração que o cliente do EWS pode acessar e as configurações configuráveis do Exchange que podem afetar seu cliente do EWS. 
  
Muitas definições de configuração podem afetar o que o aplicativo cliente do EWS pode fazer. Estas definições de configuração são: 
  
- Somente leitura ou leitura gravável do cliente.
    
- Acessado no servidor Exchange que hospeda o serviço EWS.
    
Um cliente pode acessar as configurações do Exchange Online, do Exchange Online como parte do Office 365 e de um servidor local do Exchange. Todas as configurações do Exchange Server local estão disponíveis para administradores do Exchange; no entanto, nem todas essas configurações estão disponíveis para administradores de locatários do Exchange Online. Este artigo descreve quais definições de configuração clientes, administradores do Exchange Server e administradores de locatário do Exchange Online podem acessar.
  
## <a name="configuration-settings-that-clients-can-access"></a>Definições de configuração que os clientes podem acessar

Seu aplicativo cliente pode obter e definir várias opções de configuração do servidor Exchange. Definições de configuração de que todos os aplicativos EWS precisam ser fornecidos pelo serviço de descoberta automática. Outras definições de configuração são usadas para cenários de aplicativos específicos. 
  
**Tabela 1. Recursos do serviço Web que fornecem opções de configuração para clientes do EWS**

|**Recurso**|**Descrição**|
|:-----|:-----|
|Serviço de descoberta automática  <br/> |O [serviço de descoberta automática](autodiscover-for-exchange.md) fornece aos aplicativos cliente informações de configuração para que o cliente possa se configurar automaticamente para se comunicar com o EWS.  <br/> |
|Informações de configuração personalizadas armazenadas em uma caixa de correio  <br/> |Você pode usar uma das várias opções para [armazenar informações de configuração personalizadas](persistent-application-settings-in-ews-in-exchange.md) em sua caixa de correio: objetos de configuração do usuário, itens personalizados ou propriedades estendidas.  <br/> |
|Gerenciamento de representante  <br/> | O EWS fornece operações CRUD para gerenciar o acesso de representante a uma caixa de correio. Delegados são usuários que receberam permissão para acessar a caixa de correio de outro usuário.<br/><br/>  Você pode usar as [operações de gerenciamento de representante](https://msdn.microsoft.com/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) para habilitar o gerenciamento de representante usando EWS ou, se estiver usando a API gerenciada do EWS, é possível usar os seguintes métodos:<br/><br/>- [ExchangeService. adddelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. getdelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. RemoveDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|configuração de pesquisa de descoberta eletrônica  <br/> |os aplicativos cliente de descoberta eletrônica podem obter [informações de configuração de pesquisa](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) que incluem uma consulta de pesquisa de descoberta eletrônica, uma lista de caixas de correio pesquisáveis e o identificador de bloqueio de caixa de correio in-loco.  <br/> |
|Permissões de pastas  <br/> |As permissões de pasta limitam o que um usuário pode fazer em uma pasta pública e, no caso de acesso de representante, o que um representante pode fazer na pasta de outro usuário. Você pode usar o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou a [operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para acessar o conjunto de permissões de cada pasta, incluindo pastas públicas, pastas privadas compartilhadas ou pastas às quais os usuários têm acesso de representante.  <br/> |
|Dicas de email, Unificação de mensagens ou regras de proteção  <br/> |A [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) fornece [informações de configuração de serviço](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) somente leitura para dicas de email, Unificação de mensagens e regras de proteção.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Definições de configuração que os administradores podem acessar no Exchange Server

A maioria dos cenários de aplicativo cliente não exigem alterações nas definições de configuração do servidor; no entanto, alguns cenários fazem. Por exemplo, para permitir que um aplicativo de camada intermediária atue como um usuário, você precisa definir a representação do Exchange no servidor. Observe que algumas configurações só podem ser acessadas em servidores locais do Exchange. Se você estiver direcionando para o Exchange Online, seu aplicativo cliente pode precisar trabalhar com as configurações padrão.
  
**Tabela 2. Opções de configuração do Exchange Server que afetam os clientes do EWS**

|**Recurso**|**Acessível a partir do Exchange Online?**|**Para obter mais informações, consulte...**|
|:-----|:-----|:-----|
|Configurações do diretório virtual (incluindo autenticação)  <br/> |Não  <br/> |[Get-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Descoberta Automática  <br/> |Não  <br/> |[Get-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Conformidade  <br/> |Sim  <br/> |[Arquivamento](https://technet.microsoft.com/library/dd979800%28v=exchg.150%29.aspx) <br/> [Descoberta eletrônica](https://technet.microsoft.com/library/dd298021%28v=exchg.150%29.aspx) <br/> [Retenção](https://technet.microsoft.com/library/dd335168%28v=exchg.150%29.aspx) <br/> [Prevenção contra perda de dados](https://technet.microsoft.com/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Gerenciamento de representante  <br/> |Sim  <br/> |[Manage Permissions for Recipients](https://technet.microsoft.com/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Representação do Exchange  <br/> |Sim  <br/> |[Configurar representação do Exchange](https://msdn.microsoft.com/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Dicas de email, Unificação de mensagens ou regras de proteção  <br/> |Sim  <br/> |[Dicas de Email](https://technet.microsoft.com/library/jj649091%28v=exchg.150%29.aspx) <br/> [Cmdlets de Unificação de mensagens](https://technet.microsoft.com/library/aa997665%28v=exchg.150%29.aspx) <br/> [Regras de Proteção do Outlook](https://technet.microsoft.com/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Limitação  <br/> |Não  <br/> |[Configurações de limitação](ews-throttling-in-exchange.md) <br/> |
|Filtragem de agente do usuário  <br/> |Sim  <br/> |[Filtragem de agente do usuário](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>Também consulte

- [Obter informações de configuração de serviço usando o EWS no Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)   
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

