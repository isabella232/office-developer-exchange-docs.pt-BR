---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: O elemento NonIndexableItemStatistics contém uma matriz de estatísticas para itens que não puderam ser indexados.
ms.openlocfilehash: 29551d5f7f9b4cbdd54a1ee26920eff4fcb11f25
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541963"
---
# <a name="nonindexableitemstatistics"></a>NonIndexableItemStatistics

O **elemento NonIndexableItemStatistics** contém uma matriz de estatísticas para itens que não puderam ser indexados. 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 **ArrayOfNonIndexableItemStatisticsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[NonIndexableItemStatistic](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a>Elementos pai

[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

