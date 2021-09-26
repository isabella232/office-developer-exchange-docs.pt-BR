---
title: Not
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: O elemento Not representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.
ms.openlocfilehash: a62a964043d85033ceffc5ca380468e0aeebdfc3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541956"
---
# <a name="not"></a>Not

O **elemento Not** representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém. 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 **NotType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SearchExpression](searchexpression.md) <br/> | Representa a classe base para expressões dentro de uma restrição. <br/><br/>Um dos seguintes elementos deve ser substituído pelo **elemento SearchExpression:** <br/> <br/>- [Existe](exists.md) <br/>- [Exclui](excludes.md) <br/>- [IsEqualTo](isequalto.md) <br/>- [IsNotEqualTo](isnotequalto.md) <br/>- [IsGreaterThan](isgreaterthan.md) <br/>- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/>- [IsLessThan](islessthan.md) <br/>- [IsLessThanOrEqualTo](islessthanorequalto.md) <br/>- [Contém](contains.md) <br/>- **Não** <br/>- [E](and.md) <br/>- [Ou](or.md) <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Representa a restrição ou consulta usada para filtrar itens ou pastas nas operações FindItem/FindFolder e pasta de pesquisa.  <br/> |
|**Not** <br/> |Representa uma expressão de pesquisa que nega o valor Boolean da expressão de pesquisa que ela contém.  <br/> |
|[And](and.md) <br/> |Representa uma expressão de pesquisa que permite executar uma operação Boolean **AND** entre duas ou mais expressões de pesquisa. O resultado da operação **AND** será **true** se todas as expressões de pesquisa contidas no **elemento And** são **verdadeiras**.  <br/> |
|[Or](or.md) <br/> |Representa uma expressão de pesquisa que executa uma operação **OR lógica** na expressão de pesquisa que ela contém. **Ou** retornará **true** se qualquer um de seus filhos retornar **true**. **Ou** deve ter dois ou mais filhos.  <br/> |
   
## <a name="remarks"></a>Comentários

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

