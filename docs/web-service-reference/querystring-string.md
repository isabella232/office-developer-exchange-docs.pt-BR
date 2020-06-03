---
title: QueryString (cadeia de caracteres)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f81b1b3d-9fe4-4ab3-b517-42e4207fa596
description: O elemento QueryString especifica um conjunto de valores a serem retornados que correspondam à cadeia de caracteres de consulta em uma solicitação de operação FindPeople. Uma pesquisa sem QueryString especificado retorna todos os itens da pasta especificada.
ms.openlocfilehash: ec025f86d3e6fb74810e9c539eba102d05adbb93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465321"
---
# <a name="querystring-string"></a>QueryString (cadeia de caracteres)

O elemento **QueryString** especifica um conjunto de valores a serem retornados que correspondam à cadeia de caracteres de consulta em uma solicitação de [operação FindPeople](findpeople-operation.md) . Uma pesquisa sem **QueryString** especificado retorna todos os itens da pasta especificada. 
  
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
|[FindPeople](findpeople.md) <br/> |Contém os argumentos para uma pesquisa de [operação do FindPeople](findpeople-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto **QueryString** representa uma consulta de caixa de correio feita usando um subconjunto de [sintaxe de consulta avançada (AQS)](https://msdn.microsoft.com/library/aa965711%28VS.85%29.aspx). Para obter informações sobre a sintaxe desse elemento, confira [QueryString (querystringtype)](querystring-querystringtype.md).
  
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

