---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: O elemento Contains representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecida.
ms.openlocfilehash: 6e36ede6a10c64a4aa53e68721d9edf7893c4c05
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547544"
---
# <a name="contains"></a>Contains

O **elemento Contains** representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecida. 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


**ContainsExpressionType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ContainmentMode** <br/> |Identifica os limites de uma pesquisa.  <br/> |
|**ContainmentComparison** <br/> |Determina se a pesquisa ignora casos e espaços.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Valores de atributo ContainmentMode

|**Valor**|**Descrição**|
|:-----|:-----|
|FullString  <br/> |A comparação é entre a cadeia de caracteres completa e a constante. O valor da propriedade e a constante fornecida são precisamente os mesmos.  <br/> |
|Prefixado  <br/> |A comparação é entre o prefixo de cadeia de caracteres e a constante.  <br/> |
|SUBSTRING  <br/> |A comparação é entre um subdstring da cadeia de caracteres e a constante.  <br/> |
|PrefixOnWords  <br/> |A comparação é entre um prefixo em palavras individuais na cadeia de caracteres e a constante.  <br/> |
|ExactPhrase  <br/> |A comparação é entre uma frase exata na cadeia de caracteres e a constante.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Valores do atributo ContainmentComparison

|**Valor**|**Descrição**|
|:-----|:-----|
|Exact  <br/> |A comparação deve ser exata.  <br/> |
|IgnoreCase  <br/> |A comparação ignora o invólucro.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |A comparação ignora caracteres que não são espaçamento.  <br/> |
|Afastado  <br/> |Para ser removido.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |A comparação ignora caracteres de invólucro e não espaçamento.  <br/> |
|LooseAndIgnoreCase  <br/> |Para ser removido.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |Para ser removido.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |Para ser removido.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI.  <br/> |
|[Constante](constant.md) <br/> |Identifica um valor constante em uma restrição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean And entre duas ou mais expressões de pesquisa. O resultado da operação And será **true** se todas as expressões de pesquisa contidas em And são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa um OR lógico na expressão de pesquisa que contém. O [elemento Or](or.md) retornará **true** se qualquer um de seus filhos retornar **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

Os atributos são usados para determinar como os elementos são matched.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

