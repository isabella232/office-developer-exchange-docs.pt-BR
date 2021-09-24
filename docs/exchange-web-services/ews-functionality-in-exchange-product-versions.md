---
title: Funcionalidade EWS em versões de produtos do Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: O EWS implementa novas funcionalidades em novas versões do produto. Use as informações neste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos aos quais você precisa acessar.
ms.openlocfilehash: bccd0e84fc28f8a7366f0463e555cceec71aa181
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512279"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Funcionalidade EWS em versões de produtos do Exchange

O EWS implementa novas funcionalidades em novas versões do produto. Use as informações neste artigo para determinar se a versão do Exchange que você está direcionando inclui suporte para os dados ou recursos aos quais você precisa acessar. 
  
A tabela a seguir lista as versões Exchange que incluem o EWS e os principais recursos que foram introduzidos em cada versão.
  
## <a name="ews-features-by-product-version"></a>Recursos do EWS por versão do produto

|**Versão do produto**|**Recursos**|
|:-----|:-----|
|Office 365 e Exchange Online |Inclui todos os recursos na versão atual do Exchange além de todos os novos recursos adicionados para clientes online.  |
|Exchange 2013 SP1 | Inclui todos os recursos introduzidos no Exchange 2013. Os seguintes recursos foram introduzidos no Exchange 2013 SP1:<ul><li>Os recibos de leitura agora podem ser suspensos para atualizações e exclusões.</li><li>Você pode obter [informações de aprovação de transporte](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) moderadas.</li><li>As respostas de votação podem ser exibidas.</li><li>O [método SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) e a [operação SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) aceitam todos os parâmetros em um único objeto.</li><li>As pesquisas de Descoberta Eletrônico podem especificar um idioma para consultas de pesquisa e um formato específico de cultura para intervalos de datas.</li><li>O [objeto StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) agora pode acessar os [objetos StreamingSubscription.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx)</li><li>As conversas têm uma configuração para indicar se elas contêm mensagens de email protegidas pelo IRM.</li><li>Os participantes da reunião podem propor novos horários de início e término para reuniões e incluí-los em sua resposta à reunião.</li><li>O método Soap Autodiscover [GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) agora retorna a configuração [GroupingInformation](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) usada para manter afinidade para uma assinatura de evento de várias caixas de correio.</li></ul> |
|Exchange 2013  | Inclui todos os recursos introduzidos no Exchange 2010 SP2. Os seguintes recursos foram introduzidos no Exchange 2013:  <ul><li>  Arquivamento</li><li>Descoberta eletrônica</li><li>Personas</li><li>Políticas de retenção</li><li>Armazenamento de Contato Unificado</li><li>Fotos do usuário</li></ul> |
|Exchange 2010 SP3  | Inclui todos os recursos introduzidos no Exchange 2010 SP1. Os seguintes recursos foram introduzidos no Exchange 2010 SP2:  <ul><li>  Obter Expiração de Senha</li><li>Precisão datetime</li><li>Identificadores de propriedade atualizados para contatos</li><li>Novos cenários de representação</li></ul> |
|Exchange 2010 SP1  | Inclui todos os recursos introduzidos no Exchange 2010. Os seguintes recursos foram introduzidos no Exchange 2010 SP1:  <ul><li>  Criar, recuperar e modificar regras de Caixa de Entrada</li><li>Acesso programático à Caixa de Correio de Arquivo Morto</li><li>Ações de conversas</li><li>Notificações de atravessamento de firewall</li><li>Recursos de administração aprimorados</li><li>Suporte a versão misturada aprimorado</li><li>Suporte à proteção de reação de 2007</li><li>Controle do acesso do aplicativo ao EWS</li><li>Suporte à autenticação de certificado do cliente</li></ul> |
|Exchange 2010  | Inclui todos os recursos introduzidos no Exchange 2007 SP1. Os seguintes recursos foram introduzidos na versão inicial do Exchange 2010: <ul> <li>  Lista de distribuição privada completa</li><li>Objetos de configuração do usuário</li><li>Itens associados à pasta</li><li>Controle de mensagens</li><li>Unificação de Mensagens</li><li>Descoberta Automática SOAP  </li><li>Suporte a fuso horário aprimorado</li><li>Informações de disponibilidade de recursos de sala</li><li>Pesquisa indexada</li><li>Acesso de lixeira</li><li>Informações de Dicas de Email</li></ul> |
|Exchange 2007 SP1  | Inclui todos os recursos introduzidos no Exchange 2007. Os seguintes recursos foram introduzidos no Exchange 2007 SP1:  <ul><li>  Gerenciamento de representantes</li><li>Permissões de pastas</li><li>Pastas públicas</li><li>Postar itens</li><li>Conversão de ID</li></ul> |
|Exchange 2007  | Os seguintes recursos foram introduzidos na versão inicial do Exchange 2007:  <ul><li>  Acesso total a itens, pastas e anexos (Criar, Obter, Atualizar, Excluir)</li><li>Disponibilidade</li><li>Fora do Office configurações</li><li>Notificações</li><li>Sincronização</li><li>Resolução do nome</li><li>Expansão da lista de distribuição (DL)</li><li>Pesquisar</li></ul> |
   
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
- [Migrar para as tecnologias do Exchange ](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Explorar os recursos da API gerenciada por EWS, EWS e Serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

