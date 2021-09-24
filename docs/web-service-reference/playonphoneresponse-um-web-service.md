---
title: PlayOnPhoneResponse (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: O elemento PlayOnPhoneResponse define uma resposta a uma solicitação de operação do PlayOnPhone (serviço Web de UM).
ms.openlocfilehash: 9c2893837a1bc9c4836dc3cab6fb14e0d1fd611b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516521"
---
# <a name="playonphoneresponse-um-web-service"></a>PlayOnPhoneResponse (serviço Web de Unificação de Mensagens)

O **elemento PlayOnPhoneResponse** define uma resposta a uma solicitação de operação [do PlayOnPhone (serviço Web de UM).](playonphone-operation-um-web-service.md) 
  
[PlayOnPhoneResponse (serviço Web de Unificação de Mensagens)](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor de texto é o identificador de chamada a ser usado para o valor de [CallId (serviço Web](callid-um-web-service.md) de UM) em uma solicitação de operação [GetCallInfo (serviço Web](getcallinfo-operation-um-web-service.md) de UM) ou uma solicitação de operação de desconexão (serviço Web de [UM).](disconnect-operation-um-web-service.md) 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-operation-um-web-service.md)

