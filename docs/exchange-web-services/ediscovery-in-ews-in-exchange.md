---
title: Descoberta eDiscovery no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Saiba mais sobre a Descoberta EWS no Exchange.
ms.openlocfilehash: 0b4f211e7f8a6ec085fd03ada1cc5a35187106e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512307"
---
# <a name="ediscovery-in-ews-in-exchange"></a>Descoberta eDiscovery no EWS no Exchange

Saiba mais sobre a Descoberta EWS no Exchange.
  
EDiscovery é um serviço Web de consulta federada que permite que aplicativos externos executem consultas de Exchange dados.
  
A descoberta consiste em várias fases, incluindo a identificação e preservação de dados principais, a coleta e revisão dos dados e a produção de dados no tribunal. As consultas de Descoberta Eletrônico facilitam o processo de descoberta fornecendo um único fluxo de trabalho de descoberta entre Exchange e SharePoint.
  
## <a name="ediscovery-operations"></a>Operações de Descoberta e

A funcionalidade de Descoberta Digital exposta pelo EWS está disponível por meio de operações introduzidas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2013. 
  
**Tabela 1. Novas operações para Descoberta Desdiscovery**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Obtém informações de configuração para retém in-locar, pesquisas de descoberta salvas e as caixas de correio habilitadas para pesquisa de descoberta.  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Obtém o status de uma isenção baseada em consulta, que é definida usando a [operação SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Recupera detalhes sobre itens que não podem ser indexados. Isso inclui, mas não se limita a, o identificador de item, um código de erro, uma descrição de erro, quando uma tentativa foi feita para indexar o item e informações adicionais sobre o arquivo.  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Recupera a contagem de itens que não podem ser indexados em uma caixa de correio.  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Obtém uma lista de caixas de correio em que o cliente tem permissão para pesquisar ou executar a Descoberta Eletrônico.  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Pesquisa itens em caixas de correio específicas que corresponderem a palavras-chave de consulta.  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Define uma espera baseada em consulta em itens.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)
    
- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)
    

