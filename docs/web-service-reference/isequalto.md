---
title: IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: O elemento IsEqualTo representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retornará true se eles forem iguais.
ms.openlocfilehash: a7a7deed79c271be74bb2ff16dd86605d468721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824013"
---
# <a name="isequalto"></a>IsEqualTo

O elemento **IsEqualTo** representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retornará true se eles forem iguais. 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

 **IsEqualToType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades frequentemente referenciadas pelo URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica a membros individuais de um dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades MAPI.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.  <br/> |
|[Não](not.md) <br/> |Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.  <br/> |
|[E](and.md) <br/> |Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa. O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.  <br/> |
|[Ou](or.md) <br/> |Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém. [Ou](or.md) retornará true se qualquer um dos seus filhos retornam true. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

Para executar comparações de sequência de caracteres, considere o uso do elemento [contém](contains.md) , como ele fornece opções para os parâmetros correspondentes, como caso e espaços em branco. Use o elemento [não](not.md) em conjunto com o elemento [contém](contains.md) para negar o resultado. 
  
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

