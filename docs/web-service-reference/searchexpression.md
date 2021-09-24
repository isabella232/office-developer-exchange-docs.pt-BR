---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: O elemento SearchExpression é um elemento abstrato que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo de base. Esse elemento não é usado em um documento de instância XML.
ms.openlocfilehash: e8047d333b36d77bc6823efd6488a15a6d2501a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517844"
---
# <a name="searchexpression"></a>SearchExpression

O **elemento SearchExpression** é um elemento abstrato que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo de base. Esse elemento não é usado em um documento de instância XML. 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean **AND** entre duas ou mais expressões de pesquisa. O resultado da operação **AND** será **true** se todas as expressões de pesquisa contidas no **elemento And** são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR lógica** na expressão de pesquisa que ela contém. **Ou** retornará **true** se qualquer um de seus filhos retornar **true**. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

Qualquer elemento de filtro que faz parte do grupo de substituição SearchExpression pode aparecer no lugar do elemento SearchExpression.
  
> [!NOTE]
> Esse elemento nunca ocorrerá diretamente em um documento de instância. 
  
Os elementos a seguir são membros do grupo de substituição SearchExpression:
  
- [Existe](exists.md)
    
- [Exclui](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contém](contains.md)
    
- [Not](not.md)
    
- [And](and.md)
    
- [Or](or.md)
    
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

