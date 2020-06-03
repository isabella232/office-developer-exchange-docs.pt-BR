---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: O elemento SenderDepartments especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de valor filho (ProtectionRuleValueType).
ms.openlocfilehash: cf15b974b9c0cfb09767661f17334defc4041e43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530342"
---
# <a name="senderdepartments"></a>SenderDepartments

O elemento **SenderDepartments** especifica que o departamento do remetente corresponde a qualquer um dos departamentos especificados nos elementos de [valor filho (ProtectionRuleValueType)](value-protectionrulevaluetype.md) . 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 **ProtectionRuleSenderDepartmentsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Valor (ProtectionRuleValueType)](value-protectionrulevaluetype.md) <br/> |Identifica um único departamento de remetente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condição](condition.md) <br/> |Identifica a condição que deve ser satisfeita para a parte de ação da regra a ser executada.  <br/> |
|[E (ProtectionRuleAndType)](and-protectionruleandtype.md) <br/> |Especifica que todos os elementos filho devem corresponder para serem avaliados como **true**. Especifica que deve haver mais de uma condição filha de regra de proteção.  <br/> |
   
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

