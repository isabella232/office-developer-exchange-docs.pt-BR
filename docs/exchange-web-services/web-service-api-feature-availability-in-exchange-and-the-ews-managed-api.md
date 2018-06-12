---
title: Disponibilidade de recursos do Web service API no Exchange e a API gerenciada de EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Saiba quais serviços da web e EWS recursos API estão disponíveis em cada versão do Exchange e o EWS Managed API.
ms.openlocfilehash: d19ab062c8d418e373e8268b1ab039e5436e71bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750960"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Disponibilidade de recursos do Web service API no Exchange e a API gerenciada de EWS

Saiba quais serviços da web e EWS recursos API estão disponíveis em cada versão do Exchange e o EWS Managed API.
  
Aplicativos cliente do Exchange com frequência direcionar várias versões do Exchange. Por esse motivo, você talvez queira criar seu aplicativo, de forma que você pode ativar [os recursos de cliente do EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) e desativar com base na versão do Exchange que hospeda a caixa de correio dos usuários. Este artigo fornece informações sobre quais recursos de API do serviço estão disponíveis em versões diferentes do Exchange e o EWS Managed API. Use essas informações para criar o seu aplicativo para aplicar amplamente a clientes que executam várias versões do Exchange. 
  
Para obter informações detalhadas sobre as diferenças entre as versões do Exchange, revise os arquivos de esquema do EWS e a respectiva [documentação de referência](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx).
  
## <a name="api-features-by-exchange-version"></a>Recursos de API por versão do Exchange
<a name="bk_apifeatures"> </a>

O serviço web do Exchange APIs, incluindo o EWS e descoberta automática, são desenvolvidas com várias versões compatibilidade em mente. Portanto, um aplicativo que tem como destino o Exchange 2007 também opera em relação a versões do Exchange, começando com o Exchange 2013, incluindo o Exchange Online e o Exchange Online como parte do Office 365. 
  
A tabela a seguir indica quais recursos de API estão disponíveis em cada versão do Exchange e versões da API gerenciada EWS começando com a versão 2.0. Porque seu aplicativo pode direcionar várias versões do Exchange, será útil saber quais versões suportam os recursos que seu cliente implementa. Você pode usar o serviço Descoberta automática para descobrir qual versão do Exchange destinada a um cliente para um usuário para que você pode ativar e desativar recursos dependendo se eles estão disponíveis para os usuários.
  
**Tabela 1. Disponibilidade de recurso do serviço Web em versões do Exchange e a API gerenciada de EWS**

|Recurso de API|Exchange Online (Office 365)|API Gerenciada do EWS|Exchange 2013|Exchange 2010 SP3|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Resolução de nome ambígua  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Aplicativos para gerenciamento do Outlook  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Acesso de caixa de correio de arquivo morto](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Descoberta automática (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Descoberta automática (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Respostas automáticas (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Availability  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Disponibilidade (salas)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Transferência em massa  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Grupos de contatos  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Gerenciamento de conversa  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Precisão de DateTime  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Gerenciamento de representante  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Expansão de lista de distribuição  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Acesso do Dumpster](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[descoberta eletrônica](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Fusos horários avançados  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Permissões de pasta  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Conversão do identificador](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Gerenciamento de caixa de entrada](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Acesso de item e pasta](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (recepção e push)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Eventos de caixa de correio (streaming)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Dicas de email  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Expiração de senha  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personagens](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Postar itens  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Acesso à pasta pública](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Políticas de retenção  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Pesquisa (indexada)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Pesquisa (loja)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Sincronização](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Repositório unificado de contatos](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Unificação de mensagens do serviço da Web](http://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Unificação de mensagens (baseado em EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Objetos de configuração do usuário](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Fotos dos usuários](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Você pode encontrar mais informações sobre web recursos de serviço que estão disponíveis em versões diferentes do Exchange por ler sobre as [operações do EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), o [serviço de descoberta automática](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)e os [métodos ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Para saber mais
<a name="bk_apifeatures"> </a>

Se desejar se aprofundar entender as diferenças entre as versões do Exchange, você pode fazer o seguinte:
  
- Explore o [esquema do EWS](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) para investigar as diferenças entre cada versão do EWS em mais detalhes. 
    
- Baixe o [EWSEditor](http://ewseditor.codeplex.com/). Você pode usar EWSEditor para especificar versões do esquema de destino diferente e enviar consultas com base na versão do esquema de destino.
    
## <a name="see-also"></a>Confira também

- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)   
- [Introdução aos aplicativos de cliente API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md) 
- [O que há de novo no EWS e outros serviços da web do Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

