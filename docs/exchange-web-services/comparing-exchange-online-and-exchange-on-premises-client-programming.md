---
title: Comparar a programação de cliente do Exchange Online e do Exchange local
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Saiba mais sobre as considerações de design para a criação de uma API Gerenciada EWS ou um aplicativo cliente EWS que funciona em relação Exchange Online e Exchange local.
ms.openlocfilehash: 438965656e31eca586d06a5e0b6794c0eda87621
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512285"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Comparar a programação de cliente do Exchange Online e do Exchange local

Saiba mais sobre as considerações de design para a criação de uma API Gerenciada EWS ou um aplicativo cliente EWS que funciona em relação Exchange Online e Exchange local.
  
Na maioria das vezes, os clientes e os serviços Web no Exchange que eles direcionam funcionarão da mesma maneira, independentemente de o destino ser um Exchange Online, Exchange Online como parte do Office 365 ou Exchange servidor local. Há, no entanto, algumas exceções, e você vai querer garantir que seu aplicativo possa lidar com elas. Use as informações deste artigo para ajudá-lo a projetar seu cliente para direcionar Exchange Online e Exchange local.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Considerações sobre programação do cliente de descoberta automática

[A Descoberta Automática fornece](autodiscover-for-exchange.md) informações de configuração para Exchange clientes. Um aplicativo cliente pode descobrir suas informações de configuração de uma das três maneiras, dependendo se o cliente está direcionando Exchange Online ou Exchange local. 
  
**Tabela 1. Tipos de serviço de descoberta automática e Exchange aplicabilidade**

|**Tipo de serviço de Descoberta Automática**|**Aplica-se a**|
|:-----|:-----|
|[Descoberta Automática SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online e versões do Exchange local a partir do Exchange 2010  <br/> |
|[Descoberta Automática POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online e versões do Exchange local a partir do Exchange 2007  <br/> |
|[Procurar ponto de conexão de serviço (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Versões do Exchange local a partir do Exchange 2007  <br/> |
   
Além das informações de configuração do cliente, essa Descoberta Automática soap e POX também retornam a versão do serviço Exchange e indicam se o serviço está hospedado por Exchange Online. Essas informações são retornadas em elementos diferentes, dependendo do tipo de Descoberta Automática que você usa.
  
**Tabela 2. Elementos de descoberta automática que retornam a versão do serviço e Exchange Online informações de hospedagem**

|**Tipo de serviço de Descoberta Automática**|**Elemento XML que contém a versão de serviço**|**Elemento XML que indica se o usuário tem uma Exchange Online de usuário**|
|:-----|:-----|:-----|
|Descoberta Automática SOAP  <br/> |[Elemento Setting (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o **valor de texto CasVersion.**  <br/> |[Elemento Setting (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) com o valor de texto **UserMSOnline.**  <br/> |
|Descoberta Automática do POX  <br/> |[ServerVersion (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Certifique-se de que seu cliente capture [](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) essas informações para que ele possa direcionar o conjunto de recursos que está disponível no Exchange servidor. Isso pode ser útil para determinar se seu cliente pode esperar comportamentos diferentes com base em se a caixa de correio do usuário está localizada em uma organização Exchange Online ou Exchange local. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Testes e arquivos de log em aplicativos destinados Exchange Online

Exchange Online fornece acesso aos arquivos de log de protocolo EWS, contadores de desempenho EWS e eventos de serviço relacionados ao EWS que estão disponíveis em servidores Exchange locais. No entanto, o acesso a eles é útil ao descobrir como seu aplicativo se executa quando interage com o EWS. Certifique-se de testar seu aplicativo em um servidor Exchange local para que você possa otimizar seu desempenho. Se possível, você pode alterar as configurações de [throttling](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) em seu servidor de teste para corresponder às configurações de Exchange Online, para que você possa avaliar como seu aplicativo se comportará quando ele se conectar ao Exchange Online. 
  
> [!TIP]
> Você pode usar a [ferramenta EWSRelentless](https://ewsrelentless.codeplex.com/) para executar um teste de carga EWS. Você pode usar essa ferramenta com um servidor de teste, logs de protocolo EWS, contadores de desempenho do EWS, eventos de serviço e as configurações de throttling do EWS para entender melhor como o EWS funciona sob carga. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Configurações e Exchange Online

Os valores padrão para as configurações de [throttling do EWS](ews-throttling-in-exchange.md) são diferentes para Exchange Online do que são para Exchange local. Além disso, você não pode alterar Exchange Online configurações de reação. Você pode usar Exchange cmdlets do Shell de Gerenciamento para descobrir as configurações de Exchange local; no entanto, esses cmdlets não estão habilitados para Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Exchange Cmdlets do Shell de Gerenciamento e configurações

Vários cmdlets podem afetar direta ou indiretamente as APIs do serviço Web no Exchange Online e Exchange local. Os cmdlets não estão disponíveis para o seguinte Exchange Online:
  
- Configurações de throttling 
    
- Configurações de diretório virtual 
    
- Configurações de autenticação
    
Para obter detalhes sobre os cmdlets disponíveis para Exchange Online, consulte [cmdlets](http://help.outlook.com/140/dd575549.aspx)do PowerShell em Exchange Online . Para obter mais informações sobre cmdlets que estão disponíveis para Exchange local, consulte [Exchange cmdlets 2013](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Afinidade do cliente e balanceadores de carga de rede
<a name="affinity"> </a>

A maioria das comunicações do EWS não exige que o cliente participe da manutenção da afinidade com Exchange. As assinaturas de eventos de caixa de correio exigem que o cliente forneça cookies e outras informações para manter a afinidade com o servidor Exchange que mantém a fila de eventos de caixa de correio para um usuário. Exchange Server 2010 usa o exchangecookie para manter a afinidade do cliente nos balanceadores de carga de rede. Exchange Online e versões do Exchange local a partir do Exchange 2013 usam o [header X-AnchorMailbox, o header X-PreferServerAffinity e o cookie X-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) para manter a afinidade para notificações de caixa de correio. 
  
## <a name="authentication"></a>Autenticação
<a name="auth"> </a>

Os clientes podem autenticar com Exchange Online usando Basic ou OAuth. As versões Exchange locais a partir do Exchange 2013 usam o NTLM por padrão; no entanto, é possível configurar Exchange local para usar a autenticação básica também. 
  
## <a name="client-latency-diagnostics"></a>Diagnóstico de latência do cliente
<a name="diag"> </a>

Exchange Online coleta diagnósticos de latência do cliente se eles são relatados. Isso ajuda a Microsoft a solucionar problemas de conectividade com Exchange Online. Exchange local não coleta diagnósticos de latência do cliente. Se o seu cliente Exchange no local, o cliente não poderá relatar diagnósticos de latência ao servidor.
  
## <a name="functionality-in-the-ews-managed-api"></a>Funcionalidade na API Gerenciada do EWS
<a name="ewsma"> </a>

A API Gerenciada do EWS expõe algumas funcionalidades específicas do Exchange local, como pesquisa de conexão de ponto de serviço e algumas funcionalidades específicas do Exchange Online, como o relatório de latência do cliente. Observe que é possível que algumas funcionalidades sejam implementadas no Exchange Online antes de ser implementada na API Gerenciada do EWS. 
  
A seguinte funcionalidade de API Gerenciada do EWS só é aplicável a Exchange Online:
  
- Relatório de latência do cliente
    
- Pré-autenticação básica
    
- A capacidade de solicitar que o RequestId seja retornado em respostas
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Recursos de API em Exchange Online planos e Exchange Server edições
<a name="exo"> </a>

Diferentes conjuntos de recursos podem estar disponíveis em diferentes planos Office 365 e Exchange Online, ou nas versões padrão e corporativa do Exchange Server. Esteja ciente de que algumas funcionalidades da API podem não estar disponíveis para seu aplicativo cliente, dependendo do plano Exchange Online ou da edição Exchange Server que hospeda a caixa de correio de um usuário. 
   
Como a disponibilidade de recursos pode mudar, recomendamos que você verifique os planos Exchange Online e Exchange Server edições para avaliar como a disponibilidade de recursos pode afetar seu cliente. Você também pode projetar seu cliente para verificar a disponibilidade de recursos usando a [operação GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) ou enviando solicitações de teste para as operações que implementam os recursos. Se o recurso não estiver disponível, a resposta do servidor indicará como tal. 
  
## <a name="other-considerations"></a>Outras considerações
<a name="other"> </a>

Você pode fazer o seguinte ao direcionar Exchange local, mas não Exchange Online:
  
- Crie um cliente instalado no servidor Exchange. 
    
- Instale [agentes de transporte personalizados](../transport-agents/transport-agents-in-exchange-2013.md) que podem afetar a entrega e o conteúdo das mensagens que você cria e envia com o EWS e outros clientes. 
    
## <a name="see-also"></a>Confira também

- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
- [Comparando Exchange Online e Exchange Server 2013](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Comparar todas as Office 365 para planos de negócios](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - Ferramenta de geração de carga EWS](https://ewsrelentless.codeplex.com/)
- [Disponibilidade de recursos da API de serviço Web no Exchange e na API Gerenciada do EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)
    

