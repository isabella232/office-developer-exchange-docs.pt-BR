---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: O elemento Excludes executa uma máscara bit a bit da propriedade especificada e um valor fornecido.
ms.openlocfilehash: 7923c31a4a1fea0270c9a4372072d7b0a3b79c76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510138"
---
# <a name="excludes"></a>Excludes

O **elemento Excludes** executa uma máscara bit a bit da propriedade especificada e um valor fornecido. 
  
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
|[FieldURI](fielduri.md) <br/> |Identifica propriedades referenciadas com frequência por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica propriedades MAPI.  <br/> |
|[Bitmask](bitmask.md) <br/> |Representa uma máscara hexadecimal ou decimal a ser usada durante uma [operação de restrição Excludes.](excludes.md) Se a máscara de bits representar um número hexadecimal, ela deverá ser prefixada por 0x ou 0X. Caso contrário, ele será considerado um número decimal.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean And entre duas ou mais expressões de pesquisa. O resultado da operação And será **true** se todas as expressões de pesquisa contidas em And são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa um OR lógico na expressão de pesquisa que contém. O [elemento Or](or.md) retornará **true** se qualquer um de seus filhos retornar **true**.  <br/> |
   
## <a name="remarks"></a>Comentários

**Excludes** será resolvido como **true se** uma operação AND executada na seguinte solução for 0: 
  
1. O valor bitwise para a propriedade
    
2. O valor de bitmask para a propriedade
    
**Exclui só** pode ser aplicado a uma propriedade que tenha um valor inteiro. Se o tipo de propriedade for diferente de um inteiro, um código de erro **errorUnsupportedPathForQuery** será retornado na resposta. 
  
Você pode executar a operação inversa chamando Not(Excludes).
  
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

