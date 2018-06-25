---
title: Restrição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: O elemento de restrição representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.
ms.openlocfilehash: 6b5702696db29910ae476a370bf362fe6a036ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825213"
---
# <a name="restriction"></a>Restrição

O elemento de **restrição** representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa. 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[E](and.md) <br/> |Representa uma expressão de pesquisa que permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.  <br/> |
|[Contém](contains.md) <br/> |Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.  <br/> |
|[Exclui](excludes.md) <br/> |Executa uma máscara de bit a bit das propriedades.  <br/> |
|[Existe](exists.md) <br/> |Representa uma expressão de pesquisa que retornará **true** se a propriedade fornecida existir em um item.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e será avaliada como **true** , se eles forem iguais.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for maior que o valor ou a propriedade.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a propriedade primeira for maior que ou igual ao valor ou propriedade.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor que o valor ou a propriedade.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor ou igual ao valor ou propriedade.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se os valores não são iguais.  <br/> |
|[Não](not.md) <br/> |Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.  <br/> |
|[Ou](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém. O elemento **ou** retornará **true** se qualquer um dos seus filhos retornam **true**.  <br/> |
|[SearchExpression](searchexpression.md) <br/> |Representa o elemento substituído dentro de uma restrição. Este elemento não é usado em um documento de instância XML.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para localizar itens em uma caixa de correio.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Representa os parâmetros que definem a uma pasta de pesquisa.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

