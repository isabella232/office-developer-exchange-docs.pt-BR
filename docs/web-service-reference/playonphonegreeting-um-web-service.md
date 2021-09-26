---
title: PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 43eda596-3609-4e1b-8502-1db2636535cf
description: O elemento PlayOnPhoneGreeting define uma solicitação para reproduzir uma saudação de Unificação de Mensagens em um telefone.
ms.openlocfilehash: e3b6a7720be6d046a379af460adbcc88725c0ea3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543118"
---
# <a name="playonphonegreeting-um-web-service"></a>PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)

O **elemento PlayOnPhoneGreeting** define uma solicitação para reproduzir uma saudação de Unificação de Mensagens em um telefone. 
  
[PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-um-web-service.md)
  
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
|[GreetingType (serviço Web de Unificação de Mensagens)](greetingtype-um-web-service.md) <br/> |Define o tipo de saudação a ser usado em uma solicitação de operação [PlayOnPhoneGreeting (serviço Web de UM).](playonphonegreeting-operation-um-web-service.md)  <br/> |
|[dialString (serviço Web de Unificação de Mensagens)](dialstring-um-web-service.md) <br/> |Contém o valor para o número de telefone discar.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-operation-um-web-service.md)

