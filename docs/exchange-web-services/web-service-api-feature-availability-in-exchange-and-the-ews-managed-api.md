---
title: Disponibilidade de recursos da API de serviço Web no Exchange e na API Gerenciada do EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Saiba mais sobre quais recursos de API de serviço Web e EWS estão disponíveis em cada versão do Exchange e da API Gerenciada do EWS.
ms.openlocfilehash: 6fc0c40410be543b149885c7b0785a2c6c8828af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544469"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilidade de recursos da API de serviço Web no Exchange e na API Gerenciada do EWS

Saiba mais sobre quais recursos de API de serviço Web e EWS estão disponíveis em cada versão do Exchange e da API Gerenciada do EWS.
  
Exchange aplicativos cliente geralmente direcionam muitas versões de Exchange. Por esse motivo, talvez você queira projetar seu aplicativo para que você possa ativar e desativar os recursos do cliente [EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) com base na versão do Exchange que hospeda a caixa de correio dos usuários. Este artigo fornece informações sobre quais recursos de API de serviço estão disponíveis em diferentes versões do Exchange e da API Gerenciada do EWS. Use essas informações para projetar seu aplicativo para aplicar amplamente aos clientes que executam várias versões de Exchange. 
  
Para obter informações detalhadas sobre as diferenças entre as versões Exchange, revise os arquivos de esquema EWS e a documentação de [referência associada.](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)
  
## <a name="api-features-by-exchange-version"></a>Recursos da API por Exchange versão
<a name="bk_apifeatures"> </a>

As Exchange de serviço Web, incluindo EWS e Descoberta Automática, são desenvolvidas com compatibilidade de várias versões em mente. Portanto, um aplicativo destinado ao Exchange 2007 também funciona em versões do Exchange a partir do Exchange 2013, incluindo Exchange Online e Exchange Online como parte do Office 365. 
  
A tabela a seguir indica quais recursos de API estão disponíveis em cada versão do Exchange e versões da API Gerenciada do EWS a partir da versão 2.0. Como seu aplicativo pode direcionar várias versões do Exchange, será útil para você saber quais versões suportam os recursos que seu cliente implementa. Você pode usar o serviço descoberta automática para descobrir qual versão do Exchange um cliente direciona para um usuário para que você possa ativar e desativar os recursos, dependendo se eles estão disponíveis para seus usuários.
  
**Tabela 1. Disponibilidade de recursos do serviço Web em versões do Exchange e da API Gerenciada do EWS**

|Recurso API|Exchange Online (Office 365)|API Gerenciada do EWS|Exchange 2013|Exchange 2010 SP3|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Resolução de nome ambíguo  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Aplicativos para Outlook gerenciamento  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Acesso à caixa de correio de arquivo morto](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Descoberta Automática (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Descoberta Automática (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Respostas automáticas (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilidade  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilidade (Salas)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Transferência em massa  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Grupos de contatos  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Gerenciamento de conversas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Precisão datetime  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Gerenciamento de representantes  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Expansão da lista de distribuição  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Acesso de lixeira](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Descoberta Eletrônica](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Fusos horário aprimorados  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Permissões de pastas  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Conversão de identificador](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Gerenciamento da caixa de entrada](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Acesso a itens e pastas](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (puxar e empurrar)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (streaming)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Dicas de email  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Expiração da senha  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personas](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Postar itens  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Acesso a pastas públicas](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Políticas de retenção  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Pesquisa (indexada)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Pesquisa (loja)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Sincronização](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Repositório de Contatos Unificado](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Serviço Web de Unificação de Mensagens](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Unificação de Mensagens (baseada em EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Objetos de configuração do usuário](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Fotos do usuário](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Você pode encontrar mais informações sobre os recursos de serviço Web disponíveis em diferentes versões do Exchange lendo sobre as operações [do EWS,](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)o serviço [de Descoberta](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)Automática e os métodos [ExchangeService.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx)
  
## <a name="to-learn-more"></a>Para saber mais
<a name="bk_apifeatures"> </a>

Se você quiser ir mais fundo para entender as diferenças específicas entre Exchange versões, faça o seguinte:
  
- Explore o [esquema EWS](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) para investigar as diferenças entre cada versão do EWS com mais detalhes. 
    
- Baixe [EWSEditor](http://ewseditor.codeplex.com/). Você pode usar o EWSEditor para especificar diferentes versões de esquema de destino e enviar consultas com base na versão de esquema de destino.
    
## <a name="see-also"></a>Confira também

- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)   
- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Novidades no EWS e em outros serviços Web no Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

