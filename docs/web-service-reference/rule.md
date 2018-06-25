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
description: O elemento de regra contém uma regra de proteção do único.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825263"
---
# <a name="rule"></a>Rule

O elemento de **regra** contém uma regra de proteção do único. 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 **ProtectionRuleType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Name** <br/> |Identifica o nome da regra. Um atributo necessário do tipo cadeia de caracteres com um tamanho mínimo de 1.  <br/> |
|**UserOverridable** <br/> |Especifica se a regra é obrigatória. Se a regra é obrigatória, este valor do atributo deve ser **false**. Um atributo necessário do tipo booleano.  <br/> |
|**Priority** <br/> |Especifica a prioridade da regra. Um atributo necessário do tipo int com um valor mínimo de 1.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condição](condition.md) <br/> |Identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.  <br/> |
|[Ação (ProtectionRuleActionType)](action-protectionruleactiontype.md) <br/> |Identifica a ação que deve ser executada se corresponder a parte de condição da regra.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regras](rules-ex15websvcsotherref.md) <br/> |Contém uma matriz de regras de proteção.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

