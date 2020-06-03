---
title: Disponibilidade de recursos da API do serviço Web no Exchange e na API gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Saiba mais sobre quais recursos da API do serviço da Web e EWS estão disponíveis em cada versão do Exchange e a API gerenciada do EWS.
ms.openlocfilehash: f15cf4784a59c18d1bb9ae20af378baed084acc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529844"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilidade de recursos da API do serviço Web no Exchange e na API gerenciada do EWS

Saiba mais sobre quais recursos da API do serviço da Web e EWS estão disponíveis em cada versão do Exchange e a API gerenciada do EWS.
  
Os aplicativos cliente do Exchange geralmente direcionam muitas versões do Exchange. Por esse motivo, talvez você queira criar seu aplicativo de forma que você possa ativar e desativar os [recursos do cliente EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) com base na versão do Exchange que hospeda a caixa de correio dos usuários. Este artigo fornece informações sobre quais recursos da API de serviço estão disponíveis em diferentes versões do Exchange e a API gerenciada do EWS. Use essas informações para projetar seu aplicativo para ser aplicado amplamente aos clientes que executam várias versões do Exchange. 
  
Para obter informações detalhadas sobre as diferenças entre as versões do Exchange, revise os arquivos de esquema do EWS e a [documentação de referência](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)associada.
  
## <a name="api-features-by-exchange-version"></a>Recursos da API por versão do Exchange
<a name="bk_apifeatures"> </a>

As APIs do serviço Web do Exchange, incluindo o EWS e a descoberta automática, são desenvolvidas com a compatibilidade com várias versões em mente. Portanto, um aplicativo que tem como alvo o Exchange 2007 também funciona em relação às versões do Exchange a partir do Exchange 2013, incluindo o Exchange Online e o Exchange Online como parte do Office 365. 
  
A tabela a seguir indica quais recursos da API estão disponíveis em cada versão do Exchange e versões da API gerenciada do EWS, começando com a versão 2,0. Como o aplicativo pode ter como alvo várias versões do Exchange, será útil saber quais versões são compatíveis com os recursos implementados pelo cliente. Você pode usar o serviço de descoberta automática para descobrir qual versão do Exchange um cliente se destina a um usuário para que você possa ativar e desativar recursos, dependendo se eles estão disponíveis para os usuários.
  
**Tabela 1. Disponibilidade de recursos do serviço Web em versões do Exchange e a API gerenciada do EWS**

|Recurso de API|Exchange Online (Office 365)|API Gerenciada do EWS|Exchange 2013|Exchange 2010 SP3|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Resolução de nomes ambíguos  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Aplicativos para gerenciamento do Outlook  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Acesso de caixa de correio de arquivo](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Descoberta automática (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Descoberta automática (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Respostas automáticas (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilidade  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilidade (salas)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Transferência em massa  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Grupos de contatos  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Gerenciamento de conversa  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Precisão DateTime  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Gerenciamento de representante  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Expansão de lista de distribuição  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Acesso de dumpster](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Descoberta eletrônica](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Fusos horários aprimorados  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Permissões de pastas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Conversão de identificador](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Gerenciamento de caixa de entrada](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Acesso a itens e pastas](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (pull e push)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (streaming)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Dicas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Expiração da senha  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personas](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Itens post  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Acesso a pastas públicas](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Políticas de retenção  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Pesquisa (indexado)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Pesquisa (repositório)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Sincronização](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Repositório de Contatos Unificado](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Serviço Web de Unificação de mensagens](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Unificação de mensagens (baseada em EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Objetos de configuração do usuário](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Fotos do usuário](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Você pode encontrar mais informações sobre os recursos do serviço Web disponíveis em diferentes versões do Exchange lendo sobre as operações do [EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), o [serviço de descoberta automática](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)e os [métodos ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Para saber mais
<a name="bk_apifeatures"> </a>

Se quiser aprofundar-se para entender as diferenças específicas entre as versões do Exchange, você pode fazer o seguinte:
  
- Explore o [esquema do EWS](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) para investigar as diferenças entre cada versão do EWS com mais detalhes. 
    
- Baixe o [EWSEditor](http://ewseditor.codeplex.com/). Você pode usar o EWSEditor para especificar diferentes versões de esquema de destino e enviar consultas com base na versão de esquema de destino.
    
## <a name="see-also"></a>Confira também

- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)   
- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md) 
- [O que há de novo no EWS e outros serviços Web no Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

