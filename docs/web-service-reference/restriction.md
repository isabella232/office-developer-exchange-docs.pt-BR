---
title: Restriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: O elemento Restriction representa a restrição ou consulta usada para filtrar itens ou pastas em FindItem/FindFolder e operações de pasta de pesquisa.
ms.openlocfilehash: 378c2d0ce7911638e5e58346de46759e7fdd87f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540563"
---
# <a name="restriction"></a>Restriction

O **elemento Restriction** representa a restrição ou consulta usada para filtrar itens ou pastas em FindItem/FindFolder e operações de pasta de pesquisa. 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 **RestrictionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean **AND** entre duas ou mais expressões de pesquisa.  <br/> |
|[Contém](contains.md) <br/> |Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecida.  <br/> |
|[Exclui](excludes.md) <br/> |Executa uma máscara de bit das propriedades.  <br/> |
|[Existe](exists.md) <br/> |Representa uma expressão de pesquisa que retorna **true** se a propriedade fornecida existir em um item.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e é avaliada como **true** se for igual.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for maior que o valor ou a propriedade.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for maior ou igual ao valor ou propriedade.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor que o valor ou a propriedade.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor ou igual ao valor ou propriedade.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se os valores não são os mesmos.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que contém.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR lógica** na expressão de pesquisa que contém. O **elemento Or** retornará **true** se qualquer um de seus filhos retornar **true**.  <br/> |
|[SearchExpression](searchexpression.md) <br/> |Representa o elemento substituído dentro de uma restrição. Esse elemento não é usado em um documento de instância XML.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.  <br/> |
|[SearchParameters](searchparameters.md) <br/> |Representa os parâmetros que definem uma pasta de pesquisa.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

