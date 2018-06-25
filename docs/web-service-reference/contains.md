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
description: O elemento contém representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751468"
---
# <a name="contains"></a>Contém

O elemento **contém** representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido. 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 **ContainsExpressionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ContainmentMode** <br/> |Identifica os limites de uma pesquisa.  <br/> |
|**ContainmentComparison** <br/> |Determina se a pesquisa ignora casos e espaços.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Valores de atributo ContainmentMode

|**Valor**|**Descrição**|
|:-----|:-----|
|FullString  <br/> |A comparação é entre a cadeia de caracteres completa e a constante. O valor da propriedade e a constante fornecida com precisão são os mesmos.  <br/> |
|O prefixo  <br/> |A comparação é entre o prefixo de cadeia de caracteres e a constante.  <br/> |
|Subcadeia de caracteres  <br/> |A comparação é entre uma subcadeia da cadeia de caracteres e a constante.  <br/> |
|PrefixOnWords  <br/> |A comparação é entre um prefixo de palavras individuais na cadeia de caracteres e a constante.  <br/> |
|ExactPhrase  <br/> |A comparação é entre uma frase exata na cadeia de caracteres e a constante.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Valores de atributo ContainmentComparison

|**Valor**|**Descrição**|
|:-----|:-----|
|Exact  <br/> |A comparação deve ser exata.  <br/> |
|IgnoreCase  <br/> |Comparação ignora maiusculas e minúsculas.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |Comparação ignora caracteres sem espaçamento.  <br/> |
|Afastado  <br/> |A ser removido.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |Comparação ignora a cobertura e sem espaçamento de caracteres.  <br/> |
|LooseAndIgnoreCase  <br/> |A ser removido.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |A ser removido.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |A ser removido.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades MAPI.  <br/> |
|[Constante](constant.md) <br/> |Identifica um valor de constante em uma restrição.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.  <br/> |
|[Não](not.md) <br/> |Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.  <br/> |
|[E](and.md) <br/> |Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa. O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.  <br/> |
|[Ou](or.md) <br/> |Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém. O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

Os atributos são usados para determinar como os elementos são correspondidos.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

