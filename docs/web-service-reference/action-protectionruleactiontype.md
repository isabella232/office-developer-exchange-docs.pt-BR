---
title: Ação (ProtectionRuleActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: O elemento Action identifica qual ação deve ser executada se a condição da condição da regra corresponder.
ms.openlocfilehash: 220a6fea16abb9ea823ae6239537b8c121702589
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527506"
---
# <a name="action-protectionruleactiontype"></a>Ação (ProtectionRuleActionType)

O elemento **Action** identifica qual ação deve ser executada se a condição da condição da regra corresponder. 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 **ProtectionRuleActionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Nome** <br/> |Identifica o nome da ação.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Argumento](argument.md) <br/> |Especifica argumentos para a ação. Esse elemento não ocorrerá se a ação especificada não exigir que os argumentos sejam especificados. Esse elemento pode ocorrer uma ou mais vezes se uma ação requer um ou mais argumentos. A ação **RightsProtectMessage** conterá um único argumento.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule](rule.md) <br/> |Contém uma única regra de proteção.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

