---
title: NotSentToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotSentToMe
api_type:
- schema
ms.assetid: 7cb63269-622c-4198-9a21-f5a021bf6901
description: O elemento NotSentToMe indica se o proprietário da caixa de correio não deve ser na propriedade ToRecipients das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 917648f811855961877d1aba4924573e95e3962a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824555"
---
# <a name="notsenttome"></a>NotSentToMe

O elemento **NotSentToMe** indica se o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado. 
  
```xml
<NotSentToMe>true | false</NotSentToMe>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, quando atendida, irá disparar as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa as exceções que representam todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** indica que o proprietário da caixa de correio não deve ser na propriedade **ToRecipients** das mensagens recebidas na ordem para a condição ou uma exceção a ser aplicado. Um valor **false** indica que o proprietário da caixa de correio deve estar na propriedade **ToRecipients** das mensagens de entrada na ordem para a condição ou uma exceção a ser aplicado. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

