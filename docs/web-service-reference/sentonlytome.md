---
title: SentOnlyToMe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SentOnlyToMe
api_type:
- schema
ms.assetid: b6d4dea5-812d-4b29-917d-071ebd7ddd92
description: O elemento SentOnlyToMe indica se o proprietário da caixa de correio deve ser a única na propriedade ToRecipients de mensagens de entrada para que a condição ou exceção seja aplicada.
ms.openlocfilehash: 3127550b09d6f5ccf5ba87ad34557afd047f8be0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458646"
---
# <a name="sentonlytome"></a>SentOnlyToMe

O elemento **SentOnlyToMe** indica se o proprietário da caixa de correio deve ser a única na propriedade **ToRecipients** de mensagens de entrada para que a condição ou exceção seja aplicada. 
  
```XML
<SentOnlyToMe/>true | false</SentOnlyToMe>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Condições](conditions.md) <br/> |Representa as condições que, ao serem atendidas, acionarão as ações de regra para uma regra.  <br/> |
|[Exceções](exceptions.md) <br/> |Representa todas as condições de exceção de regra disponíveis para uma regra de caixa de entrada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que o proprietário da caixa de correio deve ser o único na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada. Um valor **false** indica que o proprietário da caixa de correio não deve ser o único na propriedade **ToRecipients** das mensagens de entrada para que a condição ou exceção seja aplicada. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

