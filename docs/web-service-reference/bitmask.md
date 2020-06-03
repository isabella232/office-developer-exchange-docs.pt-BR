---
title: Mascara
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: O elemento bitmask representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição Excludes.
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458807"
---
# <a name="bitmask"></a>Mascara

O elemento **bitmask** representa uma máscara hexadecimal ou decimal a ser usada durante uma operação de restrição [Excludes](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Valor** | Representa um bitmask decimal ou hexadecimal. O valor é representado pela seguinte expressão regular:<br/>`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.<br/><br/>Estes são exemplos de valores hexadecimais para este atributo:<br/>- 0x12AF<br/>- 0X334AE<br/><br/>Estes são exemplos de valores decimais para este atributo:<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Exclui](excludes.md) <br/> |Executa uma máscara de bits bit das propriedades.  <br/> |
   
## <a name="remarks"></a>Comentários

Os valores hexadecimais devem ter um prefixo de 0x ou 0X. Se esse prefixo não existir, o valor será considerado um número decimal.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

