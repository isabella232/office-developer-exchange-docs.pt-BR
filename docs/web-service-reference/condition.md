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
description: O elemento de condição identifica a condição que deve ser atendida para a parte de ação da regra a ser executada.
ms.openlocfilehash: ed605946f99aa63416337cd0e731c931176a8ed4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751415"
---
# <a name="condition"></a>Condição

O elemento de **condição** identifica a condição que deve ser atendida para a parte de ação da regra a ser executada. 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

 **ProtectionRuleConditionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AllInternal](allinternal.md) <br/> |Avaliado como **verdadeiro** se todos os destinatários de uma mensagem de email são internos para a organização do remetente.  <br/> |
|[E (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Especifica que todos os elementos filho devem corresponder para avaliar como **true**. Especifica se deve haver mais de uma condição de filho de regra de proteção.  <br/> |
|[RecipientIs](recipientis.md) <br/> |Especifica que qualquer destinatário da mensagem de email corresponde a qualquer um dos destinatários especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[SenderDepartments](senderdepartments.md) <br/> |Especifica se o departamento do remetente corresponde a um dos departamentos especificados nos elementos filho [valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .  <br/> |
|[True](true.md) <br/> |Especifica uma condição que corresponda sempre.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Rule](rule.md) <br/> |Contém uma regra de proteção do único.  <br/> |
   
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

