---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: O elemento Rule contém uma única regra de proteção.
ms.openlocfilehash: 45fb13ae6e1aacb78e7e8520f8678097796e339f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517872"
---
# <a name="rule"></a>Rule

O **elemento Rule** contém uma única regra de proteção. 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Nome** <br/> |Identifica o nome da regra. Um atributo obrigatório da cadeia de caracteres de tipo com um comprimento mínimo de 1.  <br/> |
|**UserOverridable** <br/> |Especifica se a regra é obrigatória. Se a regra for obrigatória, esse valor de atributo deverá ser **false**. Um atributo obrigatório do tipo Boolean.  <br/> |
|**Prioridade** <br/> |Especifica a prioridade da regra. Um atributo obrigatório do tipo int com um valor mínimo de 1.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condition](condition.md) <br/> |Identifica a condição que deve ser atendida para que a parte de ação da regra seja executada.  <br/> |
|[Action (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |Identifica qual ação deve ser executada se a parte da condição da regra corresponde.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regras ](rules-ex15websvcsotherref.md) <br/> |Contém uma matriz de regras de proteção.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

