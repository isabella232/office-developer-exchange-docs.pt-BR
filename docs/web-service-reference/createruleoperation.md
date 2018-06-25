---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: O elemento CreateRuleOperation representa uma operação para criar uma nova regra de caixa de entrada.
ms.openlocfilehash: c531f222ffe886e6ef53a99609cfa27e84fd6107
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751622"
---
# <a name="createruleoperation"></a>CreateRuleOperation

O elemento **CreateRuleOperation** representa uma operação para criar uma nova regra de caixa de entrada. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[Operations](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 **CreateRuleOperationType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Regra (RuleType)](rule-ruletype.md) <br/> |Representa uma regra a ser criado na caixa de correio do usuário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Operations](operations.md) <br/> |Contém as operações que podem ser executadas em uma caixa de entrada.  <br/> |
   
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



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[DeleteRuleOperation](deleteruleoperation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

