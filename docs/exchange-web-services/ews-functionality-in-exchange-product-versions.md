---
title: Funcionalidade do EWS em versões de produtos do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: O EWS implementa nova funcionalidade em novas versões de produto. Use as informações deste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos que você precisa acessar.
ms.openlocfilehash: a8032e16cdd9100289666d8f2ce742fe054ede2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456028"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Funcionalidade do EWS em versões de produtos do Exchange

O EWS implementa nova funcionalidade em novas versões de produto. Use as informações deste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos que você precisa acessar. 
  
A tabela a seguir lista as versões do Exchange que incluem o EWS e os principais recursos que foram introduzidos em cada versão.
  
## <a name="ews-features-by-product-version"></a>Recursos do EWS por versão do produto

|**Versão do produto**|**Recursos**|
|:-----|:-----|
|Office 365 e Exchange Online |Inclui todos os recursos da versão atual do Exchange além de qualquer novo recurso adicionado para clientes online.  |
|Exchange 2013 SP1 | Inclui todos os recursos introduzidos no Exchange 2013. Os seguintes recursos foram introduzidos no Exchange 2013 SP1:<ul><li>As confirmações de leitura agora podem ser suspensas para atualizações e exclusões.</li><li>Você pode obter informações de aprovação de [transporte moderadas](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) .</li><li>As respostas de votação podem ser exibidas.</li><li>O método [SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) e a operação [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) aceitam todos os parâmetros em um único objeto.</li><li>as pesquisas de descoberta eletrônica podem especificar um idioma para consultas de pesquisa e um formato específico de cultura para intervalos de datas.</li><li>Agora, o objeto [StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) pode acessar os objetos [StreamingSubscription](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx) .</li><li>As conversas têm uma configuração para indicar se elas contêm mensagens de email protegidas pelo IRM.</li><li>Os participantes da reunião podem propor novas horas de início e de término para as reuniões e incluí-las na resposta da reunião.</li><li>O método SOAP autodiscover [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) agora retorna a configuração [GroupingInformation](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) usada para manter a afinidade de uma assinatura de evento de várias caixas de correio.</li></ul> |
|Exchange 2013  | Inclui todos os recursos introduzidos no Exchange 2010 SP2. Os seguintes recursos foram introduzidos no Exchange 2013:  <ul><li>  Arquivamento</li><li>Descoberta eletrônica</li><li>Personas</li><li>Políticas de retenção</li><li>Armazenamento de Contato Unificado</li><li>Fotos do usuário</li></ul> |
|Exchange 2010 SP3  | Inclui todos os recursos introduzidos no Exchange 2010 SP1. Os seguintes recursos foram introduzidos no Exchange 2010 SP2:  <ul><li>  Obter expiração de senha</li><li>Precisão DateTime</li><li>Identificadores de propriedade atualizados para contatos</li><li>Novos cenários de representação</li></ul> |
|Exchange 2010 SP1  | Inclui todos os recursos introduzidos no Exchange 2010. Os seguintes recursos foram introduzidos no Exchange 2010 SP1:  <ul><li>  Criar, recuperar e modificar regras de caixa de entrada</li><li>Acesso programático à caixa de correio de arquivo morto</li><li>Ações de conversas</li><li>Notificações de passagem de firewall</li><li>Recursos de administração aprimorados</li><li>Suporte aprimorado à versão mista</li><li>Suporte à proteção contra limitação</li><li>Controle do acesso de aplicativos ao EWS</li><li>Suporte a autenticação de certificado de cliente</li></ul> |
|Exchange 2010  | Inclui todos os recursos introduzidos no Exchange 2007 SP1. Os seguintes recursos foram introduzidos na versão inicial de lançamento do Exchange 2010: <ul> <li>  Lista de distribuição privada completa</li><li>Objetos de configuração do usuário</li><li>Itens associados da pasta</li><li>Controle de mensagens</li><li>Unificação de Mensagens</li><li>Descoberta Automática SOAP  </li><li>Suporte avançado a fuso horário</li><li>Informações de disponibilidade do recurso de sala</li><li>Pesquisa indexada</li><li>Acesso de dumpster</li><li>Informações de dicas de dados</li></ul> |
|Exchange 2007 SP1  | Inclui todos os recursos introduzidos no Exchange 2007. Os seguintes recursos foram introduzidos no Exchange 2007 SP1:  <ul><li>  Gerenciamento de representante</li><li>Permissões de pastas</li><li>Pastas públicas</li><li>Itens post</li><li>Conversão de ID</li></ul> |
|Exchange 2007  | Os seguintes recursos foram introduzidos na versão inicial de lançamento do Exchange 2007:  <ul><li>  Acesso completo a itens, pastas e anexos (criar, obter, atualizar, excluir)</li><li>Disponibilidade</li><li>Configurações de ausência temporária</li><li>Notificações</li><li>Sincronização</li><li>Resolução do nome</li><li>Expansão da lista de distribuição (DL)</li><li>Pesquisar</li></ul> |
   
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Migrar para as tecnologias do Exchange ](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorar os recursos do EWS Managed API, do EWS e dos serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

