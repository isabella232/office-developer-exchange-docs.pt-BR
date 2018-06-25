---
title: PlayOnPhoneGreeting (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: O elemento de PlayOnPhoneGreeting define uma solicitação para reproduzir um Unificação de mensagens em um telefone de saudação.
ms.openlocfilehash: c30140fc60b9e902517b4cc18deb9b61efa61e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824836"
---
# <a name="playonphonegreeting-um-web-service"></a>PlayOnPhoneGreeting (serviço web de Unificação de mensagens)

O elemento de **PlayOnPhoneGreeting** define uma solicitação para reproduzir um Unificação de mensagens em um telefone de saudação. 
  
[PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GreetingType (serviço web de Unificação de mensagens)](greetingtype-um-web-service.md) <br/> |Define o tipo de saudação a ser usado em uma solicitação de [operação PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md) .  <br/> |
|[dialString (serviço web de Unificação de mensagens)](dialstring-um-web-service.md) <br/> |Contém o valor para o número de telefone discar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md)

