---
title: eDiscovery do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Saiba mais sobre descoberta eletrônica no EWS no Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750649"
---
# <a name="ediscovery-in-ews-in-exchange"></a>eDiscovery do EWS no Exchange

Saiba mais sobre descoberta eletrônica no EWS no Exchange.
  
descoberta eletrônica é um serviço web de consulta federados que permite que aplicativos externos executar consultas de dados do Exchange.
  
Descoberta consiste em várias fases, incluindo identificando e preservar dados de chave, remoção para baixo e revisar os dados e produzindo dados no tribunal. consultas do eDiscovery facilitam o processo de descoberta, fornecendo um fluxo de trabalho de descoberta único entre Exchange e SharePoint.
  
## <a name="ediscovery-operations"></a>operações de descoberta eletrônica

A funcionalidade de descoberta eletrônica que é exposta por EWS está disponível por meio de operações introduzidas no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2013. 
  
**Tabela 1. Novas operações para a descoberta eletrônica**

|**Nome da operação**|**Descrição**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Obtém informações de configuração de bloqueio in-loco, salvo pesquisas de descoberta e as caixas de correio que estão habilitadas para pesquisa de descoberta.  <br/> |
|[GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Obtém o status de uma isenção baseado em consulta, que é definido usando a [operação SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Recupera os detalhes sobre os itens que não podem ser indexados. Isso inclui, mas não está limitado a, o identificador do item, um código de erro, uma descrição do erro, quando foi feita uma tentativa para indexar o item e informações adicionais sobre o arquivo.  <br/> |
|[GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Recupera a contagem de itens que não podem ser indexados em uma caixa de correio.  <br/> |
|[GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Obtém uma lista de caixas de correio que o cliente tem permissão para pesquisar ou executar a descoberta eletrônica.  <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Procura por itens em caixas de correio específicas que coincidem com palavras-chave de consulta.  <br/> |
|[SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Define uma consulta com base em espera em itens.  <br/> |
   
## <a name="see-also"></a>Confira também

- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)
    

