---
title: PlayOnPhoneGreeting (serviço Web da UM)
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
description: O elemento PlayOnPhoneGreeting define uma solicitação para reproduzir uma saudação de Unificação de mensagens em um telefone.
ms.openlocfilehash: 197e4ba671e1711b73b1e7c239339db589357581
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529921"
---
# <a name="playonphonegreeting-um-web-service"></a>PlayOnPhoneGreeting (serviço Web da UM)

O elemento **PlayOnPhoneGreeting** define uma solicitação para reproduzir uma saudação de Unificação de mensagens em um telefone. 
  
[PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-um-web-service.md)
  
```xml
<PlayOnPhoneGreeting>
  <GreetingType/>
  <DialString/>
</PlayOnPhoneGreeting>
```

 **complexType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Greetingtype (serviço Web da UM)](greetingtype-um-web-service.md) <br/> |Define o tipo de saudação a ser usado em uma solicitação de [operação do PlayOnPhoneGreeting (serviço Web da um)](playonphonegreeting-operation-um-web-service.md) .  <br/> |
|[dialstring (serviço Web da UM)](dialstring-um-web-service.md) <br/> |Contém o valor do número de telefone a ser discado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md)

