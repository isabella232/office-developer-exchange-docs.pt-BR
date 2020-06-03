---
title: Condição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: O elemento Condition identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.
ms.openlocfilehash: 2aea11197f072a4dbe21292bb47075d6f273d31b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463220"
---
# <a name="condition"></a>Condição

O elemento **Condition** identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada. 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

**ProtectionRuleConditionType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Interno](allinternal.md) <br/> |Avalia como **true** se todos os destinatários de uma mensagem de email são internos à organização do remetente.  <br/> |
|[E (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**. Especifica que deve haver mais de uma condição filha de regra de proteção.  <br/> |
|[Destinatário](recipientis.md) <br/> |Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[Verdadeiro](true.md) <br/> |Especifica uma condição que sempre corresponde.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule](rule.md) <br/> |Contém uma única regra de proteção.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
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

