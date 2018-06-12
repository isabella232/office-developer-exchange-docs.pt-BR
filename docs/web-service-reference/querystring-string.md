---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: O elemento QueryString Especifica um conjunto de valores a serem retornadas que correspondam a cadeia de caracteres de consulta em uma solicitação de operação FindPeople. Uma pesquisa com nenhum QueryString especificado retorna todos os itens da pasta especificada.
ms.openlocfilehash: 9c5c733adcec1496e36986fd720b56b0a0274593
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824935"
---
# <a name="querystring-string"></a>QueryString (String)

O elemento **QueryString** Especifica um conjunto de valores a serem retornadas que correspondam a cadeia de caracteres de consulta em uma solicitação de [operação FindPeople](findpeople-operation.md) . Uma pesquisa com nenhum **QueryString** especificado retorna todos os itens da pasta especificada. 
  
```XML
<QueryString/> 
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Contém os argumentos para uma pesquisa de [operação FindPeople](findpeople-operation.md) .  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto **QueryString** representa uma consulta de caixa de correio que foram feita por meio de um subconjunto da [Sintaxe de consulta avançada (AQS)](http://msdn.microsoft.com/en-us/library/aa965711%28VS.85%29.aspx). Para obter informações sobre a sintaxe para esse elemento, consulte [QueryString (QueryStringType)](querystring-querystringtype.md).
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindPeople](findpeople-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

