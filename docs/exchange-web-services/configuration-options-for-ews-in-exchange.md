---
title: Opções de configuração para o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Encontre informações sobre as definições de configuração que pode ser acessados por seu cliente do EWS e as configurações do Exchange configuráveis que podem afetar o seu cliente do EWS.
ms.openlocfilehash: d6c2866abf3dc16c77d84355afb9d86b0a9934c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750650"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Opções de configuração para o EWS no Exchange

Encontre informações sobre as definições de configuração que pode ser acessados por seu cliente do EWS e as configurações do Exchange configuráveis que podem afetar o seu cliente do EWS. 
  
Várias definições de configuração podem afetar o que pode fazer o seu aplicativo de cliente do EWS. Essas definições de configuração estão: 
  
- Somente leitura ou leitura gravável do cliente.
    
- Acessada no servidor do Exchange que hospeda seu serviço do EWS.
    
Um cliente pode acessar as configurações no Exchange Online, Exchange Online como parte do Office 365 e um servidor do Exchange no local. Todas as configurações de servidor do Exchange no local estão disponíveis para administradores do Exchange; No entanto, não todas essas configurações estão disponíveis para administradores Inquilinos do Exchange Online. Este artigo descreve quais clientes de definições de configuração, os administradores do Exchange Server e locatário do Exchange Online, os administradores podem acessar.
  
## <a name="configuration-settings-that-clients-can-access"></a>Definições de configuração que os clientes podem acessar

O aplicativo cliente pode obter e definir várias opções de configuração do servidor Exchange. Definições de configuração que precisam de todos os aplicativos do EWS são fornecidas pelo serviço de descoberta automática. Outras definições de configuração são usadas para cenários de aplicativo específico. 
  
**Tabela 1. Recursos do serviço Web que fornecem as opções de configuração para clientes EWS**

|**Recurso**|**Descrição**|
|:-----|:-----|
|Serviço de descoberta automática  <br/> |O [serviço de descoberta automática](autodiscover-for-exchange.md) fornece seu cliente de aplicativos com informações de configuração para que seu cliente pode se configurar automaticamente para se comunicar com o EWS.  <br/> |
|Informações de configuração personalizadas armazenadas em uma caixa de correio  <br/> |Você pode usar uma das várias opções para [armazenar informações de configuração personalizada](persistent-application-settings-in-ews-in-exchange.md) na caixa de correio: objetos de configuração do usuário, itens personalizados ou propriedades estendidas.  <br/> |
|Gerenciamento de representante  <br/> | EWS fornece operações CRUD para gerenciar o acesso de representante para uma caixa de correio. Os representantes são usuários que tiverem permissão para acessar a caixa de correio de outro usuário.<br/><br/>  Você pode usar as [operações de gerenciamento do representante](http://msdn.microsoft.com/en-us/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) para habilitar o gerenciamento de representantes usando o EWS ou, se você estiver usando o EWS Managed API, você pode usar os seguintes métodos:<br/><br/>- [ExchangeService.AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|configuração de pesquisa de descoberta eletrônica  <br/> |aplicativos cliente do eDiscovery podem obter [informações de configuração de pesquisa](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) que inclui uma consulta de pesquisa de descoberta eletrônica, uma lista de caixas de correio pesquisáveis, e contém o identificador da caixa de correio no local.  <br/> |
|Permissões de pasta  <br/> |Permissões da pasta limitam o que um usuário pode fazer em uma pasta pública e no caso de acesso de representante, o que um representante pode fazer na pasta de outro usuário. Você pode usar o método [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou a [operação GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para acessar o conjunto de permissões de cada pasta, incluindo as pastas públicas, pastas particulares compartilhadas ou pastas para o qual os usuários têm acesso delegado.  <br/> |
|Dicas de email, Unificação de mensagens ou regras de proteção  <br/> |A [operação GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) fornece [informações de configuração do serviço](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) de somente leitura para dicas de email, Unificação de mensagens e regras de proteção.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Definições de configuração que os administradores podem acessar no Exchange server

A maioria dos cenários de aplicativos cliente não requerem alterações às definições de configuração do servidor; No entanto, alguns cenários fazer. Por exemplo, para habilitar um aplicativo de camada intermediária agir como um usuário, você precisará definir representação do Exchange no servidor. Observe que algumas configurações só podem ser acessadas em servidores do Exchange no local. Se você está direcionando Exchange Online, o aplicativo cliente talvez seja necessário trabalhar com as configurações padrão.
  
**Tabela 2. Opções de configuração de servidor do Exchange que afetam os clientes EWS**

|**Recurso**|**Acessível do Exchange Online?**|**Para obter mais informações, consulte …**|
|:-----|:-----|:-----|
|Configurações do diretório virtual (incluindo autenticação)  <br/> |Não  <br/> |[Get-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Descoberta Automática  <br/> |Não  <br/> |[Get-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Conformidade  <br/> |Sim  <br/> |[Arquivamento](http://technet.microsoft.com/en-us/library/dd979800%28v=exchg.150%29.aspx) <br/> [descoberta eletrônica](http://technet.microsoft.com/en-us/library/dd298021%28v=exchg.150%29.aspx) <br/> [Retenção](http://technet.microsoft.com/en-us/library/dd335168%28v=exchg.150%29.aspx) <br/> [Prevenção de perda de dados](http://technet.microsoft.com/en-us/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Gerenciamento de representante  <br/> |Sim  <br/> |[Gerenciar permissões para destinatários](http://technet.microsoft.com/en-us/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Representação do Exchange  <br/> |Sim  <br/> |[Configurar a representação do Exchange](http://msdn.microsoft.com/en-us/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Dicas de email, Unificação de mensagens ou regras de proteção  <br/> |Sim  <br/> |[Dicas de email](http://technet.microsoft.com/en-us/library/jj649091%28v=exchg.150%29.aspx) <br/> [Unified Messaging Cmdlets](http://technet.microsoft.com/en-us/library/aa997665%28v=exchg.150%29.aspx) <br/> [Regras de proteção do Outlook](http://technet.microsoft.com/en-us/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Limitação  <br/> |Não  <br/> |[As configurações de limitação](ews-throttling-in-exchange.md) <br/> |
|Filtragem de agente do usuário  <br/> |Sim  <br/> |[Filtragem de agente do usuário](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>Confira também

- [Obter informações de configuração de serviço usando o EWS no Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)   
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

