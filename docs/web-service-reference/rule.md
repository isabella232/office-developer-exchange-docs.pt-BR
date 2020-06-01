---
title: Rule
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: O elemento Rule contém uma única regra de proteção.
ms.openlocfilehash: 6c18a2bd026893cd333bc7007203abf04a6f0be7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464998"
---
# <a name="rule"></a>Rule

O elemento **Rule** contém uma única regra de proteção. 
  
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
|**Nome** <br/> |Identifica o nome da regra. Um atributo necessário do tipo cadeia de caracteres com um tamanho mínimo de 1.  <br/> |
|**Useroverridable** <br/> |Especifica se a regra é obrigatória. Se a regra for obrigatória, esse valor de atributo deve ser **false**. Um atributo necessário do tipo Boolean.  <br/> |
|**Prioridade** <br/> |Especifica a prioridade da regra. Um atributo necessário do tipo int com um valor mínimo de 1.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condição](condition.md) <br/> |Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.  <br/> |
|[Ação (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |Identifica qual ação deve ser executada se a condição da condição da regra corresponder.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regras](rules-ex15websvcsotherref.md) <br/> |Contém uma matriz de regras de proteção.  <br/> |
   
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

