---
title: ResultType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 488ee828-343f-4382-a5e8-eed1005f5dbc
description: O elemento ResultType contém o tipo de pesquisa a ser executado. O tipo de pesquisa pode ser apenas estatísticas ou visualizar apenas.
ms.openlocfilehash: 750f53ae05a7ad9f5aefc9396911a23ef32cdfc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825211"
---
# <a name="resulttype"></a>ResultType

O elemento **ResultType** contém o tipo de pesquisa a ser executado. O tipo de pesquisa pode ser apenas estatísticas ou visualizar apenas. 
  
```XML
<ResultType>StatisticsOnly | PreviewOnly</ResultType>
```

 **SearchResultType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxesResult](searchmailboxesresult.md) | [SearchMailboxes](searchmailboxes.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **ResultType** é o tipo de resultado que é retornado para uma pesquisa de descoberta. Um valor de texto de **StatisticsOnly** retornará as estatísticas da pesquisa. Um valor de texto de **PreviewOnly** irá retornar informações de visualização do item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

