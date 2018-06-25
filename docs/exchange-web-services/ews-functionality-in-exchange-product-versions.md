---
title: Funcionalidade do EWS nas versões de produto do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS implementa a nova funcionalidade em novas versões do produto. Use as informações neste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos que você precisará ter acesso ao.
ms.openlocfilehash: 6b676781f25eeeb90fd9ab075fbe63198766bd99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750657"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Funcionalidade do EWS nas versões de produto do Exchange

EWS implementa a nova funcionalidade em novas versões do produto. Use as informações neste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos que você precisará ter acesso ao. 
  
A tabela a seguir lista as versões do Exchange que incluem EWS e os principais recursos que foram introduzidos em cada versão.
  
## <a name="ews-features-by-product-version"></a>Recursos do EWS por versão do produto

|**Versão do produto**|**Recursos**|
|:-----|:-----|
|Office 365 e o Exchange Online |Inclui todos os recursos na versão atual do Exchange além de quaisquer recursos novos que são adicionadas aos clientes online.  |
|Exchange 2013 SP1 | Inclui todos os recursos introduzidos no Exchange 2013. Os seguintes recursos foram introduzidos no Exchange 2013 SP1:<ul><li>Agora podem ser suspenso confirmações de leitura para atualizações e exclusões.</li><li>Você pode obter informações de aprovação [moderados transporte](http://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) .</li><li>Respostas da votação podem ser exibidas.</li><li>O método [SetHoldOnMailboxes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) e a operação de [SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) aceitam todos os parâmetros em um único objeto.</li><li>pesquisas de descoberta eletrônica podem especificar um idioma para consultas de pesquisa e um formato específico da cultura para intervalos de data.</li><li>O objeto [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) agora pode acessar os objetos [StreamingSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) .</li><li>Conversas com uma configuração para indicar se eles contêm mensagens de email são protegidas por IRM.</li><li>Os participantes da reunião podem propor novo horários de início e término para reuniões e incluí-las em sua resposta de reunião.</li><li>O método de descoberta automática do SOAP [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) agora retorna [GroupingInformation](http://msdn.microsoft.com/EN-US/library/office/dn529149%28v=exchg.150%29.aspx) configuração é usada manter a afinidade de uma inscrição de evento várias caixas de correio.</li></ul> |
|Exchange 2013  | Inclui todos os recursos introduzidos no Exchange 2010 SP2. Os seguintes recursos foram introduzidos no Exchange 2013:  <ul><li>  Arquivamento</li><li>Descoberta eletrônica</li><li>Personagens</li><li>Políticas de retenção</li><li>Repositório unificado de contatos</li><li>Fotos dos usuários</li></ul> |
|Exchange 2010 SP3  | Inclui todos os recursos introduzidos no Exchange 2010 SP1. Os seguintes recursos foram introduzidos no Exchange 2010 SP2:  <ul><li>  Obtenha a validade da senha</li><li>Precisão de DateTime</li><li>Identificadores de propriedade atualizados para contatos</li><li>Novos cenários de representação</li></ul> |
|Exchange 2010 SP1  | Inclui todos os recursos introduzidos no Exchange 2010. Os seguintes recursos foram introduzidos no Exchange 2010 SP1:  <ul><li>  Criar, recuperar e modificar as regras de caixa de entrada</li><li>Acesso programático à caixa de correio de arquivo morto</li><li>Ações de conversas</li><li>Atravessando notificações de firewall</li><li>Recursos de administração aprimorado</li><li>Versão mista suporte aprimorado</li><li>Suporte à proteção de limitação</li><li>Controle de acesso do aplicativo a EWS</li><li>Suporte à autenticação de certificado de cliente</li></ul> |
|Exchange 2010  | Inclui todos os recursos introduzidos no Exchange 2007 SP1. Os seguintes recursos introduzidos na versão inicial do Exchange 2010: <ul> <li>  Lista completa de distribuição particular</li><li>Objetos de configuração do usuário</li><li>Itens associados de pasta</li><li>Acompanhamento de mensagens</li><li>Unificação de Mensagens</li><li>Descoberta Automática SOAP  </li><li>Suporte aprimorado de fuso horário</li><li>Informações de disponibilidade de recurso de sala</li><li>Pesquisa indexada</li><li>Acesso do Dumpster</li><li>Informações de dicas de email</li></ul> |
|Exchange 2007 SP1  | Inclui todos os recursos introduzidos no Exchange 2007. Os seguintes recursos foram introduzidos no Exchange 2007 SP1:  <ul><li>  Gerenciamento de representante</li><li>Permissões de pasta</li><li>Pastas públicas</li><li>Postar itens</li><li>Conversão de ID</li></ul> |
|Exchange 2007  | Os seguintes recursos introduzidos na versão inicial do Exchange 2007:  <ul><li>  Acesso total a itens, pastas e anexos (criar, obter, atualizar, excluir)</li><li>Availability</li><li>Sem configurações do Office</li><li>Notificações</li><li>Sincronização</li><li>Resolução de nomes</li><li>Expansão de lista (DL) de distribuição</li><li>Pesquisar</li></ul> |
   
## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
- [Migrar para as tecnologias do Exchange ](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

