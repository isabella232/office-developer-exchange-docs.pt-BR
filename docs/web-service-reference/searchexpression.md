---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: O SearchExpression é um elemento abstrato que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo de base. Este elemento não é usado em um documento de instância XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825286"
---
# <a name="searchexpression"></a>SearchExpression

O **SearchExpression** é um elemento abstrato que representa o elemento substituído dentro de uma restrição. Todas as expressões de pesquisa derivam desse tipo de base. Este elemento não é usado em um documento de instância XML. 
  
```xml
<SearchExpression/>
```

 **SearchExpressionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.  <br/> |
|[Não](not.md) <br/> |Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.  <br/> |
|[E](and.md) <br/> |Representa uma expressão de pesquisa que lhe permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa. O resultado da operação **e** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **verdadeiras**.  <br/> |
|[Ou](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém. **Ou** retornará **true** se qualquer um dos seus filhos retornam **true**. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

Qualquer elemento de filtro que faz parte do grupo de substituição SearchExpression pode aparecer no lugar do elemento SearchExpression.
  
> [!NOTE]
> Esse elemento nunca ocorrerá dentro de um documento da instância. 
  
Os seguintes elementos são membros do grupo de substituição SearchExpression:
  
- [Existe](exists.md)
    
- [Exclui](excludes.md)
    
- [IsEqualTo](isequalto.md)
    
- [IsNotEqualTo](isnotequalto.md)
    
- [IsGreaterThan](isgreaterthan.md)
    
- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)
    
- [IsLessThan](islessthan.md)
    
- [IsLessThanOrEqualTo](islessthanorequalto.md)
    
- [Contém](contains.md)
    
- [Não](not.md)
    
- [E](and.md)
    
- [Ou](or.md)
    
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

