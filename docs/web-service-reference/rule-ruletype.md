---
title: Rule (RuleType)
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
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: O elemento Rule contém uma única regra e representa uma regra na caixa de correio de um usuário.
ms.openlocfilehash: 0e7d7284d561ea374f66106072df0c4f850c590c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527513"
---
# <a name="rule-ruletype"></a>Rule (RuleType)

O **elemento Rule** contém uma única regra e representa uma regra na caixa de correio de um usuário. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RuleId](ruleid.md) <br/> |Especifica o identificador de regra.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Contém o nome de exibição de uma regra.  <br/> |
|[Prioridade](priority.md) <br/> |Indica a ordem na qual uma regra deve ser executado.  <br/> |
|[IsEnabled](isenabled.md) <br/> |Indica se a regra está habilitada.  <br/> |
|[IsNotSupported](isnotsupported.md) <br/> |Indica se a regra não pode ser modificada com as APIs de código gerenciado.  <br/> |
|[IsInError](isinerror.md) <br/> |Indica se a regra está em uma condição de erro.  <br/> |
|[Condições](conditions.md) <br/> |Identifica as condições que, quando cumpridas, dispararão as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Identifica as exceções que representam todas as condições de exceção de regra disponíveis para a regra de caixa de entrada.  <br/> |
|[Actions](actions.md) <br/> |Representa as ações a serem tomadas em uma mensagem quando as condições são atendidas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateRuleOperation](createruleoperation.md) <br/> |Representa uma operação para criar uma nova regra.  <br/> |
|[InboxRules](inboxrules.md) <br/> |Representa uma matriz de regras na caixa de correio do usuário.  <br/> |
|[SetRuleOperation](setruleoperation.md) <br/> |Representa uma operação para atualizar uma regra existente.  <br/> |
   
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
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[UpdateInboxRules](updateinboxrules.md)
  
[SetRuleOperation](setruleoperation.md)
  
[CreateRuleOperation](createruleoperation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

