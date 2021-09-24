---
title: Opções de configuração para EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Encontre informações sobre as configurações que seu cliente EWS pode acessar e as configurações configuráveis Exchange que podem afetar seu cliente EWS.
ms.openlocfilehash: ed7667086b36897fd07031526e5a4657a120d505
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522282"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Opções de configuração para EWS no Exchange

Encontre informações sobre as configurações que seu cliente EWS pode acessar e as configurações configuráveis Exchange que podem afetar seu cliente EWS. 
  
Muitas configurações podem afetar o que seu aplicativo cliente EWS pode fazer. Essas configurações são: 
  
- Somente leitura ou leitura-writeable do cliente.
    
- Acessado no servidor Exchange que hospeda seu serviço EWS.
    
Um cliente pode acessar configurações em Exchange Online, Exchange Online como parte do Office 365 e um servidor de Exchange local. Todas as configurações de Exchange do servidor local estão disponíveis para Exchange administradores; no entanto, nem todas essas configurações estão disponíveis para administradores Exchange Online locatários. Este artigo descreve quais configurações clientes, Exchange Server administradores e Exchange Online locatários podem acessar.
  
## <a name="configuration-settings-that-clients-can-access"></a>Configurações que os clientes podem acessar

Seu aplicativo cliente pode obter e definir várias opções de configuração do servidor Exchange cliente. As configurações de que todos os aplicativos EWS precisam são fornecidas pelo serviço descoberta automática. Outras configurações são usadas para cenários de aplicativo específicos. 
  
**Tabela 1. Recursos de serviço Web que fornecem opções de configuração para clientes EWS**

|**Recurso**|**Descrição**|
|:-----|:-----|
|Serviço de descoberta automática  <br/> |O [serviço descoberta automática](autodiscover-for-exchange.md) fornece aos aplicativos cliente informações de configuração para que seu cliente possa se configurar automaticamente para se comunicar com o EWS.  <br/> |
|Informações de configuração personalizadas armazenadas em uma caixa de correio  <br/> |Você pode usar uma das várias opções para armazenar informações [de](persistent-application-settings-in-ews-in-exchange.md) configuração personalizadas em sua caixa de correio: objetos de configuração do usuário, itens personalizados ou propriedades estendidas.  <br/> |
|Gerenciamento de representantes  <br/> | O EWS fornece operações CRUD para gerenciar o acesso de representante a uma caixa de correio. Representantes são usuários que receberam permissão para acessar a caixa de correio de outro usuário.<br/><br/>  Você pode [](https://msdn.microsoft.com/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) usar as operações de gerenciamento de representantes para habilitar o gerenciamento de representantes usando o EWS ou, se estiver usando a API Gerenciada do EWS, você pode usar os seguintes métodos:<br/><br/>- [ExchangeService.AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|Configuração de pesquisa de Descoberta Eletrônica  <br/> |Os aplicativos cliente de [](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) Descoberta Eletrônica podem obter informações de configuração de pesquisa que incluem uma consulta de pesquisa de Descoberta Eletrônica, uma lista de caixas de correio pesquisáveis e o identificador de retém de caixa de correio in-loco.  <br/> |
|Permissões de pastas  <br/> |As permissões de pasta limitam o que um usuário pode fazer em uma pasta pública e, no caso de acesso delegado, o que um representante pode fazer na pasta de outro usuário. Você pode usar o método [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou a operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para acessar o conjunto de permissões de cada pasta, incluindo pastas públicas, pastas privadas compartilhadas ou pastas às quais os usuários têm acesso de representante.  <br/> |
|Dicas de email, Unificação de Mensagens ou regras de proteção  <br/> |A [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) fornece [](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) informações de configuração de serviço somente leitura para dicas de email, Unificação de Mensagens e regras de proteção.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Configurações que os administradores podem acessar no Exchange servidor

A maioria dos cenários de aplicativo cliente não exige alterações nas configurações do servidor; no entanto, alguns cenários fazem. Por exemplo, para habilitar um aplicativo de camada intermediária para atuar como usuário, você precisa definir Exchange Representação no servidor. Observe que algumas configurações só podem ser acessadas em servidores Exchange locais. Se você estiver direcionando Exchange Online, seu aplicativo cliente pode precisar trabalhar com as configurações padrão.
  
**Tabela 2. Exchange de configuração de servidor que afetam clientes EWS**

|**Característica**|**Acessível por Exchange Online?**|**Para obter mais informações, consulte...**|
|:-----|:-----|:-----|
|Configurações de diretório virtual (incluindo autenticação)  <br/> |Não  <br/> |[Get-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Descoberta automática  <br/> |Não  <br/> |[Get-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Conformidade  <br/> |Sim  <br/> |[Arquivamento](https://technet.microsoft.com/library/dd979800%28v=exchg.150%29.aspx) <br/> [Descoberta Eletrônica](https://technet.microsoft.com/library/dd298021%28v=exchg.150%29.aspx) <br/> [Retenção](https://technet.microsoft.com/library/dd335168%28v=exchg.150%29.aspx) <br/> [Prevenção contra perda de dados](https://technet.microsoft.com/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Gerenciamento de representantes  <br/> |Sim  <br/> |[Manage Permissions for Recipients](https://technet.microsoft.com/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Exchange Representação  <br/> |Sim  <br/> |[Configurar Exchange representação](https://msdn.microsoft.com/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Dicas de email, Unificação de Mensagens ou regras de proteção  <br/> |Sim  <br/> |[Dicas de Email](https://technet.microsoft.com/library/jj649091%28v=exchg.150%29.aspx) <br/> [Cmdlets de Unificação de Mensagens](https://technet.microsoft.com/library/aa997665%28v=exchg.150%29.aspx) <br/> [Regras de Proteção do Outlook](https://technet.microsoft.com/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Limitação  <br/> |Não  <br/> |[Configurações de throttling](ews-throttling-in-exchange.md) <br/> |
|Filtragem de agente de usuário  <br/> |Sim  <br/> |[Filtragem de agente de usuário](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>Confira também

- [Obter informações de configuração de serviço usando o EWS no Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)   
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

