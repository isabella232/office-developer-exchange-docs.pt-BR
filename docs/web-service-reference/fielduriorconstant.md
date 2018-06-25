---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: O elemento FieldURIOrConstant representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.
ms.openlocfilehash: 5195feec2a314d9ec15dc4a25a7a014aded1696a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752245"
---
# <a name="fielduriorconstant"></a>FieldURIOrConstant

O elemento **FieldURIOrConstant** representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade. 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

 **FieldURIOrConstantType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Constante](constant.md) <br/> |Identifica um valor de constante em uma restrição.  <br/> |
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades MAPI.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retornará true se eles forem iguais.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior que ou igual ao segundo valor ou propriedade.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor que o segundo valor ou a propriedade.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for menor ou igual ao segundo valor ou propriedade.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se os valores não são iguais.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="example"></a>Exemplo

O exemplo XML a seguir mostra o elemento FieldURIOrConstant usado com uma constante e o URI do campo.
  
```
[xml]
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

