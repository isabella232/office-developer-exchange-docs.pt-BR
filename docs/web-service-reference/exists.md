---
title: Exists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: O elemento Exists representa uma expressão de pesquisa que retorna true se a propriedade fornecida existir em um item.
ms.openlocfilehash: 992283d42f2060b7408f40289198bdbd22e71ec6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541403"
---
# <a name="exists"></a>Exists

O **elemento Exists** representa uma expressão de pesquisa que retorna **true** se a propriedade fornecida existir em um item. 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 **ExistsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean And entre duas ou mais expressões de pesquisa. O resultado da operação And será **verdadeiro se** todas as expressões de pesquisa contidas em And são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa um OR lógico na expressão de pesquisa que ela contém. [Ou](or.md) retornará **true** se qualquer um de seus filhos retornar **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

