---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: O elemento And representa uma expressão de pesquisa que permite executar uma operação Boolean AND entre duas ou mais expressões de pesquisa. O resultado da operação AND será true se todas as expressões de pesquisa contidas no elemento And são verdadeiras.
ms.openlocfilehash: b6cf8ffbb19ea3aff917493e6ae4e324025c6ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541529"
---
# <a name="and"></a>And

O **elemento And** representa uma expressão de pesquisa que permite executar uma operação Boolean **AND** entre duas ou mais expressões de pesquisa. O resultado da operação **AND** será **true** se todas as expressões de pesquisa contidas no **elemento And** são **verdadeiras**.
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 **AndType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Representa a classe base para expressões dentro de uma restrição. Deve haver duas ou mais expressões de pesquisa em uma operação And.<br/><br/>  Um dos seguintes elementos deve ser substituído pelo **elemento SearchExpression:**<ul><li> [Existe](exists.md)</li><li>[Exclui](excludes.md)</li><li>[IsEqualTo](isequalto.md)</li><li>[IsNotEqualTo](isnotequalto.md)</li><li>[IsGreaterThan](isgreaterthan.md)</li><li>[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</li><li>[IsLessThan](islessthan.md)</li><li>[IsLessThanOrEqualTo](islessthanorequalto.md)</li><li>[Contém](contains.md)</li><li>[Not](not.md)</li><li>**And**</li><li>[Or](or.md) </li></ul> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|[Not](not.md) <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.  <br/> |
|**And** <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean **AND** entre duas ou mais expressões de pesquisa. O resultado da operação **AND** será **true** se todas as expressões de pesquisa contidas no **elemento And** são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR lógica** na expressão de pesquisa que ela contém. **Ou** retornará **true** se qualquer um de seus filhos retornar **true**. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

