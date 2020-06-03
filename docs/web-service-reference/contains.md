---
title: Contém
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: O elemento Contains representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecido.
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527114"
---
# <a name="contains"></a>Contém

O elemento **Contains** representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecido. 
  
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
|Fullstring  <br/> |A comparação é entre a cadeia de caracteres completa e a constante. O valor da propriedade e a constante fornecida são exatamente os mesmos.  <br/> |
|Precedidas  <br/> |A comparação é entre o prefixo de cadeia de caracteres e a constante.  <br/> |
|SUBSTRING  <br/> |A comparação é entre uma subcadeia de caracteres e a constante.  <br/> |
|PrefixOnWords  <br/> |A comparação é entre um prefixo em palavras individuais na cadeia de caracteres e a constante.  <br/> |
|ExactPhrase  <br/> |A comparação é entre uma frase exata na cadeia de caracteres e a constante.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Valores de atributo ContainmentComparison

|**Valor**|**Descrição**|
|:-----|:-----|
|Exata  <br/> |A comparação deve ser exata.  <br/> |
|IgnoreCase  <br/> |A comparação ignora a capitalização.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |A comparação ignora os caracteres sem espaçamento.  <br/> |
|Afastado  <br/> |A ser removido.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |A comparação ignora caracteres de capitalização e sem espaçamento.  <br/> |
|LooseAndIgnoreCase  <br/> |A ser removido.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |A ser removido.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |A ser removido.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades com frequência referenciadas por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades MAPI.  <br/> |
|[Constante](constant.md) <br/> |Identifica um valor constante em uma restrição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa. O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém. O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

Os atributos são usados para determinar como os elementos são correspondidos.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

