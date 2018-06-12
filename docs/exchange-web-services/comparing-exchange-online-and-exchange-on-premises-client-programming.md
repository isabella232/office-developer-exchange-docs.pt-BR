---
title: Comparando o Exchange Online e programação do cliente do Exchange local
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Saiba mais sobre as considerações de design para a criação de uma API gerenciada de EWS ou aplicativos de cliente do EWS que funciona em relação o Exchange Online e do Exchange local.
ms.openlocfilehash: 87c6ee476e06b50c339901bf61020b0fc98f8486
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750673"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparando o Exchange Online e programação do cliente do Exchange local

Saiba mais sobre as considerações de design para a criação de uma API gerenciada de EWS ou aplicativos de cliente do EWS que funciona em relação o Exchange Online e do Exchange local.
  
A maior parte, os clientes e web services no Exchange direcionar por eles funcionam da mesma forma, independentemente se o destino é um Exchange Online, Exchange Online como parte do Office 365, ou Exchange server local. No entanto, há algumas exceções, e você vai querer certificar-se de que seu aplicativo pode lidar com elas. Use as informações neste artigo para ajudá-lo a projetar seu cliente visando ambas Exchange Online e Exchange local.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considerações sobre programação de cliente de descoberta automática

[Descoberta automática](autodiscover-for-exchange.md) fornece informações de configuração para clientes do Exchange. Um aplicativo cliente pode descobrir suas informações de configuração de três maneiras, dependendo se o cliente está direcionando Exchange Online ou Exchange local. 
  
**Tabela 1. Tipos de serviço de descoberta automática e a capacidade de aplicação do Exchange**

|**Tipo de serviço de descoberta automática**|**Aplica-se a**|
|:-----|:-----|
|[Descoberta Automática SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |O Exchange Online e versões do Exchange local começando com o Exchange 2010  <br/> |
|[Descoberta Automática POX](autodiscover-for-exchange.md#bk_Options) <br/> |O Exchange Online e versões do Exchange local começando com o Exchange 2007  <br/> |
|[Pesquisa de (SCP) do ponto de conexão de serviço](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versões do Exchange local começando com o Exchange 2007  <br/> |
   
Além das informações da configuração de cliente, que SOAP e descoberta automática de POX também retornam a versão de serviço do Exchange e indicam se o serviço é hospedado pelo Exchange Online. Essas informações são retornadas nos elementos diferentes, dependendo do tipo de descoberta automática é usar.
  
**Tabela 2. Elementos de descoberta automática que retornam a versão do service e o Exchange Online informações de hospedagem**

|**Tipo de serviço de descoberta automática**|**Elemento XML que contém a versão do serviço**|**Elemento XML que indica se o usuário tem uma conta do Exchange Online**|
|:-----|:-----|:-----|
|Descoberta Automática SOAP  <br/> |Elemento de [Configuração (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o valor de texto **CasVersion** .  <br/> |Elemento de [Configuração (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o valor de texto **UserMSOnline** .  <br/> |
|Descoberta Automática do POX  <br/> |[ServerVersion (POX)](http://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Certifique-se de que seu cliente de captura essas informações para que ele pode direcionar o [conjunto de recursos](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) que está disponível no Exchange server. Isso pode ser útil para determinar se o seu cliente pode esperar comportamento diferente com base em se a caixa de correio do usuário está localizada em um Exchange Online ou Exchange organização local. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Arquivos de log e teste em aplicativos que visam o Exchange Online

O Exchange Online não fornece acesso a arquivos de log de protocolo do EWS, contadores de desempenho do EWS e eventos de serviço relacionado à EWS que estão disponíveis nos servidores do Exchange local. Acesso a esses é útil, no entanto, em descobrir como seu aplicativo executa quando ele interage com o EWS. Certifique-se de que você teste seu aplicativo contra um servidor do Exchange no local de teste para que você possa otimizar seu desempenho. Se possível, você pode [alterar as configurações de limitação](http://technet.microsoft.com/en-us/library/bb232205%28v=exchg.150%29.aspx#Policies) no seu servidor de teste para corresponder as configurações de limitação para o Exchange Online, para que você possa avaliar o comportamento de seu aplicativo ao se conectar ao Exchange Online. 
  
> [!TIP]
> Você pode usar a ferramenta [EWSRelentless](https://ewsrelentless.codeplex.com/) para realizar um teste de carga do EWS. Você pode usar essa ferramenta com um servidor de teste, os logs de protocolo do EWS, contadores de desempenho do EWS, eventos de serviço e o EWS as configurações de limitação para compreender melhor como o EWS executa sob carga. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Configurações de limitação e o Exchange Online

Os valores padrão para as [configurações de limitação EWS](ews-throttling-in-exchange.md) são diferentes para o Exchange Online, que eles são para Exchange local. Além disso, você não pode alterar o Exchange Online as configurações de limitação. Você pode usar os cmdlets do Shell de gerenciamento do Exchange para descobrir as configurações de limitação para o Exchange local; No entanto, esses cmdlets não estão habilitados para o Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Configurações de cmdlets e configuração do Shell de gerenciamento do Exchange

Um número de cmdlets pode direta ou indiretamente afetam as APIs de serviço web no Exchange Online e local do Exchange. Cmdlets não estão disponíveis para o seguinte no Exchange Online:
  
- As configurações de limitação 
    
- Configurações do diretório virtual 
    
- Configurações de autenticação
    
Para obter detalhes sobre os cmdlets que estão disponíveis para o Exchange Online, consulte [cmdlets do PowerShell no Exchange Online](http://help.outlook.com/en-us/140/dd575549.aspx). Para obter mais informações sobre os cmdlets que estão disponíveis para o Exchange local, consulte [Exchange 2013 cmdlets](http://technet.microsoft.com/en-us/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Balanceadores de carga de rede e a afinidade do cliente
<a name="affinity"> </a>

A maioria das comunicações do EWS não exigem que o cliente participar da manutenção afinidade com o Exchange. As assinaturas de eventos de caixa de correio exigem que o cliente forneça cookies e outras informações para manter a afinidade com o Exchange server que mantém a fila de eventos de caixa de correio de um usuário. Exchange Server 2010 usa o exchangecookie para manter a afinidade do cliente entre os balanceadores de carga de rede. O Exchange Online e versões do Exchange local começando com o Exchange 2013 usam o [cabeçalho X-AnchorMailbox, o cabeçalho X-PreferServerAffinity e o cookie X-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) para manter afinidade para notificações de caixa de correio. 
  
## <a name="authentication"></a>Autenticação
<a name="auth"> </a>

Clientes podem autenticar com o Exchange Online usando OAuth ou Basic. Versões do Exchange começando com o Exchange 2013 ao local usam NTLM por padrão. No entanto, é possível configurar o Exchange local para usar a autenticação básica. 
  
## <a name="client-latency-diagnostics"></a>Diagnóstico de latência do cliente
<a name="diag"> </a>

Exchange Online coleta diagnóstico de latência do cliente, se eles forem relatados. Isso ajuda o suporte da Microsoft a resolver problemas de conectividade com o Exchange Online. Exchange local não coleta diagnóstico de latência do cliente. Se seu cliente é destinada Exchange local, o cliente não pode relatar diagnósticos de latência no servidor.
  
## <a name="functionality-in-the-ews-managed-api"></a>API gerenciada de funcionalidade no EWS
<a name="ewsma"> </a>

A API gerenciada de EWS expõe algumas funcionalidades específicas para o Exchange no local, como pesquisa de conexão do ponto de serviço e algumas funcionalidades que são específica ao Exchange Online, como o relatório de latência do cliente. Observe que é possível que algumas funcionalidades a serem implementadas no Exchange Online antes que ela é implementada na API gerenciada do EWS. 
  
A seguinte funcionalidade do EWS Managed API só é aplicável para o Exchange Online:
  
- Relatório de latência de cliente
    
- Pré-autenticação básica
    
- A capacidade de solicitar que o RequestId retornado nas respostas
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Recursos de API nos planos do Exchange Online e edições do Exchange Server
<a name="exo"> </a>

Conjuntos de recursos diferentes podem estar disponíveis em diferentes planos do Office 365 e o Exchange Online ou nas versões standard e enterprise do Exchange Server. Lembre-se de que algumas funcionalidades de API podem não estar disponíveis para o aplicativo cliente, dependendo do plano Online do Exchange ou a edição do Exchange Server que hospeda a caixa de correio do usuário. 
  
**Tabela 3. Variações de recurso de API nos planos e edições**

|**Recurso de API**|**Considerações sobre o plano ou edition**|
|:-----|:-----|
|EWS acesso às contas, exceto por meio de representação do Exchange  <br/> |Não permitida no [Office 365 para empresas — planos de quiosque](http://office.microsoft.com/en-us/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |
|UM (Unificação de Mensagens)  <br/> |Disponível somente com o Office 365 Enterprise (E3) plano, Exchange Online plano 2 e edições Enterprise do Exchange Server 2013.  <br/> |
|Integração com o Active Directory Domain Services (AD DS)  <br/> |Não está disponível com o plano do Office 365 Small Business e o Office 365 Small Business Premium.  <br/> |
|Gerenciamento de direitos de informação, legais e arquivamento retém  <br/> |Disponível somente com os planos do Office 365 Enterprise (E3 e E4).  <br/> |
|Proteção de perda de dados  <br/> |Disponível somente com os planos do Office 365 Enterprise, o Exchange Online plano 2 e edições Enterprise do Exchange Server 2013.  <br/> |
   
Porque a disponibilidade de recursos pode ser alterados, recomendamos que você verifique os planos do Exchange Online e edições do Exchange Server para avaliar como a disponibilidade de recursos pode afetar seu cliente. Você também pode projetar seu cliente para verificar a disponibilidade de recurso usando a [operação GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou enviando solicitações de teste para as operações que implementam os recursos. Se o recurso não estiver disponível, a resposta do servidor indicará como tal. 
  
## <a name="other-considerations"></a>Outras considerações
<a name="other"> </a>

Você pode fazer o seguinte procedimento quando direcionamento Exchange local, mas não Exchange on-line:
  
- Crie um cliente que está instalado no servidor Exchange. 
    
- Instale os [agentes de transporte personalizado](../transport-agents/transport-agents-in-exchange-2013.md) que podem afetar a entrega e o conteúdo das mensagens que você criar e enviar com EWS e outros clientes. 
    
## <a name="see-also"></a>Confira também

- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
- [Comparando o Exchange Online e Exchange Server 2013](http://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparar todos os Office 365 para planos de negócios](http://office.microsoft.com/en-us/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - ferramenta de geração de carregamento de EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilidade de recursos do Web service API no Exchange e a API gerenciada de EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [EWS limitação no Exchange](ews-throttling-in-exchange.md)
    

