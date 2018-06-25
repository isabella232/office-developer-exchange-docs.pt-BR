---
title: Regra (RuleType)
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
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: O elemento de regra contém uma única regra e representa uma regra de caixa de correio do usuário.
ms.openlocfilehash: b1f9f058213543633335db11f03729964baf98ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825259"
---
# <a name="rule-ruletype"></a>Regra (RuleType)

O elemento de **regra** contém uma única regra e representa uma regra de caixa de correio do usuário. 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 **RuleType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |Especifica o identificador da regra.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Contém o nome de exibição de uma regra.  <br/> |
|[Priority](priority.md) <br/> |Indica a ordem na qual uma regra será executada.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Indica se a regra está habilitada.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Indica se a regra não pode ser modificada com os APIs de código gerenciado.  <br/> |
|[IsInError](isinerror.md) <br/> |Indica se a regra está em uma condição de erro.  <br/> |
|[Condições](conditions.md) <br/> |Identifica as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Identifica as exceções que representam todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.  <br/> |
|[Ações](actions.md) <br/> |Representa as ações a serem tomadas em uma mensagem quando as condições são atendidas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Representa uma operação para criar uma nova regra.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Representa uma matriz de regras da caixa de correio do usuário.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Representa uma operação de atualização de uma regra existente.  <br/> |
   
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
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

