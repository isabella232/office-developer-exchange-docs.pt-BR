---
title: QueryString (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: O elemento QueryString especifica um conjunto de valores a serem retornados que corresponderão à cadeia de caracteres de consulta em uma solicitação de operação FindPeople. Uma pesquisa sem QueryString especificada retorna todos os itens da pasta especificada.
ms.openlocfilehash: 6dfd4b5552511e2551baf5ce645f82d4f74e5499
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523731"
---
# <a name="querystring-string"></a>QueryString (String)

O **elemento QueryString** especifica um conjunto de valores a serem retornados que corresponderão à cadeia de caracteres de consulta em uma solicitação de operação [FindPeople.](findpeople-operation.md) Uma pesquisa sem **QueryString** especificada retorna todos os itens da pasta especificada. 
  
```XML
<QueryString/> 
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindPeople](findpeople.md) <br/> |Contém os argumentos de uma pesquisa [de operação FindPeople.](findpeople-operation.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

O **valor de texto QueryString** representa uma consulta de caixa de correio feita usando um subconjunto de Sintaxe de Consulta Avançada [(AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). Para obter informações sobre a sintaxe desse elemento, consulte [QueryString (QueryStringType)](querystring-querystringtype.md).
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindPeople](findpeople-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

