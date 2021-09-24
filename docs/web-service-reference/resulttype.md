---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: O elemento ResultType contém o tipo de pesquisa a ser executar. O tipo de pesquisa pode ser somente estatísticas ou visualização.
ms.openlocfilehash: 65227a8f79a7abd597653b646a7c3985c3e38ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509452"
---
# <a name="resulttype"></a>ResultType

O **elemento ResultType** contém o tipo de pesquisa a ser executar. O tipo de pesquisa pode ser somente estatísticas ou visualização. 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxesResult](searchmailboxesresult.md)  |  [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento ResultType** é o tipo de resultado retornado para uma pesquisa de descoberta. Um valor de texto **de StatisticsOnly** retornará as estatísticas de pesquisa. Um valor de texto **de PreviewOnly** retornará informações de visualização de item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

