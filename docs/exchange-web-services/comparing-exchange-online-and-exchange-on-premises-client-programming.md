---
title: Comparando a programação de cliente local do Exchange Online e do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Saiba mais sobre as considerações de design para criar uma API gerenciada do EWS ou um aplicativo cliente do EWS que funcione no Exchange Online e no Exchange local.
ms.openlocfilehash: 8b4dbae5cadfed377aa3a7179144a7cea68bc35c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456161"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparando a programação de cliente local do Exchange Online e do Exchange

Saiba mais sobre as considerações de design para criar uma API gerenciada do EWS ou um aplicativo cliente do EWS que funcione no Exchange Online e no Exchange local.
  
Para a maioria dos clientes e os serviços Web no Exchange, eles funcionam da mesma forma, independentemente de o destino ser um Exchange Online, o Exchange Online como parte do Office 365 ou do servidor local do Exchange. No entanto, há algumas exceções, e você deve certificar-se de que seu aplicativo possa tratá-los. Use as informações deste artigo para ajudá-lo a projetar seu cliente para direcionar o Exchange Online e o Exchange no local.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considerações de programação de cliente de descoberta automática

A [descoberta automática](autodiscover-for-exchange.md) fornece informações de configuração para clientes do Exchange. Um aplicativo cliente pode descobrir suas informações de configuração de uma das três maneiras, dependendo se o cliente está direcionando o Exchange Online ou o Exchange no local. 
  
**Tabela 1. Tipos de serviço de descoberta automática e aplicabilidade do Exchange**

|**Tipo de serviço de descoberta automática**|**Aplica-se a**|
|:-----|:-----|
|[Descoberta Automática SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online e versões do Exchange no local, começando com o Exchange 2010  <br/> |
|[Descoberta Automática POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online e versões do Exchange no local, começando com o Exchange 2007  <br/> |
|[Pesquisa de ponto de conexão de serviço (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versões do Exchange no local, começando com o Exchange 2007  <br/> |
   
Além das informações de configuração do cliente, a descoberta automática de SOAP e POX também retorna a versão do serviço do Exchange e indica se o serviço está hospedado pelo Exchange Online. Essas informações são retornadas em diferentes elementos, dependendo do tipo de descoberta automática que você usa.
  
**Tabela 2. Elementos de descoberta automática que retornam informações de hospedagem e versão de serviço do Exchange Online**

|**Tipo de serviço de descoberta automática**|**Elemento XML que contém a versão do serviço**|**Elemento XML que indica se o usuário tem uma conta do Exchange Online**|
|:-----|:-----|:-----|
|Descoberta Automática SOAP  <br/> |Elemento de [configuração (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o valor de texto **CasVersion** .  <br/> |Elemento de [configuração (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o valor de texto **UserMSOnline** .  <br/> |
|Descoberta Automática do POX  <br/> |[ServerVersion (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Certifique-se de que seu cliente Capture essas informações para que ele possa direcionar o [conjunto de recursos](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) que está disponível no Exchange Server. Isso pode ser útil para determinar se o cliente pode esperar um comportamento diferente com base em se a caixa de correio do usuário está localizada em uma organização local do Exchange Online ou do Exchange. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Testando e registrando arquivos em aplicativos que direcionam o Exchange Online

O Exchange Online não fornece acesso aos arquivos de log de protocolo do EWS, contadores de desempenho do EWS e eventos de serviço relacionados ao EWS que estão disponíveis em servidores locais do Exchange. O acesso a esses é útil, no entanto, na descoberta de como o aplicativo é executado quando ele interage com o EWS. Certifique-se de testar seu aplicativo em um servidor local de teste no Exchange para que você possa otimizar seu desempenho. Se possível, você pode [alterar as configurações de limitação](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) no servidor de teste para corresponder às configurações de limitação do Exchange Online, para que possa avaliar como o aplicativo se comportará quando se conectar ao Exchange Online. 
  
> [!TIP]
> Você pode usar a ferramenta [EWSRelentless](https://ewsrelentless.codeplex.com/) para executar um teste de carga do EWS. Você pode usar essa ferramenta com um servidor de teste, logs de protocolo do EWS, contadores de desempenho do EWS, eventos de serviço e as configurações de limitação do EWS para entender melhor como o EWS realiza sob carga. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Configurações de limitação e Exchange Online

Os valores padrão para as [configurações de limitação de EWS](ews-throttling-in-exchange.md) são diferentes para o Exchange Online do que são para o Exchange local. Além disso, você não pode alterar as configurações de limitação do Exchange Online. Você pode usar os cmdlets do Shell de gerenciamento do Exchange para descobrir as configurações de limitação do Exchange no local; no entanto, esses cmdlets não estão habilitados para o Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Cmdlets e definições de configuração do Shell de gerenciamento do Exchange

Vários cmdlets podem afetar direta ou indiretamente as APIs do serviço Web no Exchange Online e no Exchange local. Os cmdlets não estão disponíveis para o seguinte no Exchange Online:
  
- Configurações de limitação 
    
- Configurações do diretório virtual 
    
- Configurações de autenticação
    
Para obter detalhes sobre os cmdlets disponíveis para o Exchange Online, consulte [cmdlets do PowerShell no Exchange Online](http://help.outlook.com/140/dd575549.aspx). Para saber mais sobre cmdlets disponíveis para o Exchange no local, confira [cmdlets do exchange 2013](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Afinidade de cliente e balanceadores de carga de rede
<a name="affinity"> </a>

A maioria das comunicações do EWS não exige que o cliente participe de manter a afinidade com o Exchange. As assinaturas para eventos de caixa de correio exigem que o cliente forneça cookies e outras informações para manter a afinidade com o servidor Exchange que mantém a fila de eventos de caixa de correio para um usuário. O Exchange Server 2010 usa o exchangecookie para manter a afinidade do cliente nos balanceadores de carga de rede. Exchange Online e versões do Exchange no local a partir do Exchange 2013 usam o [cabeçalho x-AnchorMailbox, o cabeçalho x-PreferServerAffinity e o cookie x-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) para manter a afinidade para notificações de caixa de correio. 
  
## <a name="authentication"></a>Autenticação
<a name="auth"> </a>

Os clientes podem autenticar com o Exchange Online usando o Basic ou o OAuth. As versões do Exchange no local a partir do Exchange 2013 usam NTLM por padrão; no entanto, é possível configurar o Exchange no local para usar a autenticação básica também. 
  
## <a name="client-latency-diagnostics"></a>Diagnóstico de latência do cliente
<a name="diag"> </a>

O Exchange Online coleta diagnósticos de latência do cliente, se forem relatados. Isso ajuda a solucionar problemas de conectividade com o Exchange Online. O Exchange local não coleta diagnósticos de latência do cliente. Se o cliente tiver como alvo o Exchange local, o cliente não poderá relatar o diagnóstico de latência para o servidor.
  
## <a name="functionality-in-the-ews-managed-api"></a>Funcionalidade na API gerenciada do EWS
<a name="ewsma"> </a>

A API gerenciada do EWS expõe algumas funcionalidades específicas para o Exchange local, como pesquisa de conexão de ponto de serviço e algumas funcionalidades específicas para o Exchange Online, como relatórios de latência do cliente. Observe que é possível que algumas funcionalidades sejam implementadas no Exchange Online antes de serem implementadas na API gerenciada do EWS. 
  
A seguinte funcionalidade de API gerenciada do EWS só é aplicável ao Exchange Online:
  
- Relatórios de latência do cliente
    
- Pré-autenticação básica
    
- A capacidade de solicitar que a RequestId seja retornada em respostas
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Recursos de API nos planos do Exchange Online e nas edições do Exchange Server
<a name="exo"> </a>

Diferentes conjuntos de recursos podem estar disponíveis em diferentes planos do Office 365 e do Exchange Online, ou nas versões standard e Enterprise do Exchange Server. Lembre-se de que algumas funcionalidades da API podem não estar disponíveis para seu aplicativo cliente, dependendo do plano do Exchange Online ou Exchange Server Edition que hospeda a caixa de correio de um usuário. 
  
**Tabela 3. Variações de recursos de API em planos e edições**

|**Recurso de API**|**Considerações de planejamento ou edição**|
|:-----|:-----|

| Acesso do EWS a contas, exceto por representação do Exchange  <br/> | Não é permitido no [Office 365 for Business – planos quiosque](https://office.microsoft.com/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |


| Unificação de mensagens (UM)  <br/> | Disponível apenas com o Office 365 Enterprise (E3) Plan, o Exchange Online Plan 2 e o Exchange Server 2013 Enterprise Editions.  <br/> | | Integração dos serviços de domínio do Active Directory (AD DS)  <br/> | Não está disponível no plano do Office 365 Small Business e do Office 365 Small Business Premium.  <br/> | | Gerenciamento de direitos de informação, arquivamento e bloqueios legais  <br/> | Disponível apenas com os planos do Office 365 Enterprise (E3 e E4).  <br/> | | Proteção contra perda de dados  <br/> | Disponível apenas com o Office 365 Enterprise Plans, Exchange Online Plan 2 e Exchange Server 2013 Enterprise Editions.  <br/> |
   
Como a disponibilidade de recursos pode ser alterada, recomendamos que você verifique os planos do Exchange Online e as edições do Exchange Server para avaliar como a disponibilidade de recursos pode afetar o cliente. Você também pode criar seu cliente para verificar a disponibilidade de recursos usando a [operação GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou enviando solicitações de teste para as operações que implementam os recursos. Se o recurso não estiver disponível, a resposta do servidor indicará como tal. 
  
## <a name="other-considerations"></a>Outras considerações
<a name="other"> </a>

Você pode fazer o seguinte ao direcionar o Exchange no local, mas não o Exchange Online:
  
- Crie um cliente que esteja instalado no Exchange Server. 
    
- Instalar [agentes de transporte personalizados](../transport-agents/transport-agents-in-exchange-2013.md) que podem afetar a entrega e o conteúdo de mensagens que você cria e envia com o EWS e outros clientes. 
    
## <a name="see-also"></a>Também consulte

- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
- [Comparando o Exchange Online e o Exchange Server 2013](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparar todos os planos do Office 365 para empresas](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless-ferramenta de geração de carga do EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilidade de recursos da API do serviço Web no Exchange e na API gerenciada do EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)
    

