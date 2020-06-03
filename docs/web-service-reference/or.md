---
title: Ou
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: O elemento or representa uma expressão de pesquisa que executa uma expressão lógica OR na pesquisa que ela contém. Ou retornará true se qualquer um dos seus filhos retornar true. Ou deve ter dois ou mais filhos.
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462476"
---
# <a name="or"></a>Ou

O elemento **or** representa uma expressão de pesquisa que executa uma expressão lógica **or** na pesquisa que ela contém. **Ou** retornará **true** se qualquer um dos seus filhos retornar **true**. **Ou** deve ter dois ou mais filhos. 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 **OrType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Pesquisa](searchexpression.md) <br/> | Representa a classe base para expressões dentro de uma restrição. <br/><br/>Um dos seguintes elementos deve ser substituído pelo elemento **searché** : <br/> <br/>- [Houver](exists.md) <br/>- [Exclui](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Contém](contains.md) <br/>- [Sido](not.md) <br/>- [E](and.md) <br/>- **Ou** <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar um Boolean **e** uma operação entre duas ou mais expressões de pesquisa. O resultado da operação **and** será **true** se todas as expressões de pesquisa contidas no elemento **e** forem **true**.  <br/> |
|**Or** <br/> |Representa uma expressão de pesquisa que executa uma operação lógica **ou** na expressão de pesquisa que ela contém. **Ou** retornará **true** se qualquer um dos seus filhos retornar **true**. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

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

