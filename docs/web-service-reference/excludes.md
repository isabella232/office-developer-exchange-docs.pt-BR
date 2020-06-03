---
title: Exclui
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: O elemento Excludes executa uma máscara bit a bit da propriedade especificada e um valor fornecido.
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530611"
---
# <a name="excludes"></a>Exclui

O elemento **Excludes** executa uma máscara bit a bit da propriedade especificada e um valor fornecido. 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

**ExcludesType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades com frequência referenciadas por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades MAPI.  <br/> |
|[Mascara](bitmask.md) <br/> |Representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição [Excludes](excludes.md) . Se o bitmask representar um número hexadecimal, ele deve ser prefixado por 0x ou 0X. Caso contrário, ele será considerado um número decimal.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa. O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém. O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

As **exclusões** serão resolvidas como **true** se uma operação and executada no seguinte procedimento resolver para 0: 
  
1. O valor bit a bit da propriedade
    
2. O valor de bitmask para a propriedade
    
**Excludes** só podem ser aplicadas a uma propriedade que tenha um valor inteiro. Se o tipo de propriedade for algo diferente de um inteiro, um código de erro de **ErrorUnsupportedPathForQuery** será retornado na resposta. 
  
Você pode executar a operação reversa chamando não (exclui).
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

