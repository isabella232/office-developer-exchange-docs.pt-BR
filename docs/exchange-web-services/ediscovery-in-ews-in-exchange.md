---
title: Descoberta eletrônica no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Saiba mais sobre a descoberta eletrônica no EWS no Exchange.
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456091"
---
# <a name="ediscovery-in-ews-in-exchange"></a>Descoberta eletrônica no EWS no Exchange

Saiba mais sobre a descoberta eletrônica no EWS no Exchange.
  
a descoberta eletrônica é um serviço Web de consulta federada que permite que aplicativos externos realizem consultas de dados do Exchange.
  
A descoberta consiste em várias fases, incluindo a identificação e preservação de dados importantes, a remoção e a revisão dos dados e a produção de dados no tribunal. as consultas de descoberta eletrônica facilitam o processo de descoberta fornecendo um único fluxo de trabalho de descoberta no Exchange e no SharePoint.
  
## <a name="ediscovery-operations"></a>operações de descoberta eletrônica

A funcionalidade de descoberta eletrônica exposta pelo EWS está disponível por meio de operações introduzidas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013. 
  
**Tabela 1. Novas operações para descoberta eletrônica**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Obtém informações de configuração para bloqueios in-loco, pesquisas salvas de descoberta e caixas de correio habilitadas para pesquisa de descoberta.  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Obtém o status de um bloqueio baseado em consulta, que é definido usando a [operação SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Recupera os detalhes sobre os itens que não podem ser indexados. Isso inclui, mas não está limitado a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa é feita para indexar o item e informações adicionais sobre o arquivo.  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Recupera a contagem de itens que não podem ser indexados em uma caixa de correio.  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Obtém uma lista de caixas de correio nas quais o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Procura itens em caixas de correio específicas que correspondam a palavras-chave de consulta.  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Define um bloqueio baseado em consulta nos itens.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)
    

