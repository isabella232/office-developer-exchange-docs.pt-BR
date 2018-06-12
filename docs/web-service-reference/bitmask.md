---
title: Máscara de bits
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
description: O elemento de Bitmask representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de exclusões.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751285"
---
# <a name="bitmask"></a>Máscara de bits

O elemento de **Bitmask** representa uma máscara hexadecimal ou decimal a ser usado durante uma operação de restrição de [exclusões](excludes.md) . 
  
```xml
<Bitmask Value="" />
```

**ExcludesValueType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Valor** | Representa uma bitmask decimal ou hexadecimal. O valor é representado pela expressão regular a seguir:<br/>' ((0x|0x)[0-9a-FA-f]*)|([0-9] *)'.<br/><br/>A seguir estão exemplos de valores hexadecimais para este atributo:<br/>-0x12AF<br/>-0X334AE<br/><br/>A seguir estão exemplos de decimais valores para este atributo:<br/>-10<br/>-255<br/>-4562 |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Exclui](excludes.md) <br/> |Executa uma máscara de bit a bit das propriedades.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Valores hexadecimais devem ter um prefixo de 0x ou 0x. Se esse prefixo não existir, o valor é considerado um número decimal.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

