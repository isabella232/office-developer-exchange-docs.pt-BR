---
title: CallId (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: O elemento CallId contém o valor que representa o identificador da chamada em uma solicitação GetCallInfo (serviço web de UM) ou solicitação Desconectar (serviço Web de UM).
ms.openlocfilehash: c19f1061d81bf7683fd2c84fb1c6968826046be6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522024"
---
# <a name="callid-um-web-service"></a>CallId (serviço Web de Unificação de Mensagens)

O **elemento CallId** contém o valor que representa o identificador da chamada em uma solicitação [GetCallInfo (serviço web de UM)](getcallinfo-um-web-service.md) ou [solicitação Desconectar (serviço Web de UM).](disconnect-um-web-service.md) 
  
[GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-um-web-service.md)
  
[CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md)
  
[Disconnect (serviço Web de Unificação de Mensagens)](disconnect-um-web-service.md)
  
[CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-um-web-service.md) <br/> |Define uma solicitação para obter informações sobre uma chamada.  <br/> |
|[Disconnect (serviço Web de Unificação de Mensagens)](disconnect-um-web-service.md) <br/> |Define uma solicitação para desconectar uma chamada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor de texto representa o identificador de uma chamada.
  
## <a name="remarks"></a>Comentários

Para inicializar uma chamada, use a operação [PlayOnPhone (serviço Web](playonphone-operation-um-web-service.md) da UM) ou a operação [PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md). Use o valor de texto retornado nos elementos [PlayOnPhoneResponse (serviço Web](playonphoneresponse-um-web-service.md) da UM) ou [PlayOnPhoneGreetingResponse (serviço Web da UM)](playonphonegreetingresponse-um-web-service.md) para o valor de texto do elemento **CallId.** 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-operation-um-web-service.md)
  
[Operação Disconnect (serviço Web de Unificação de mensagens)](disconnect-operation-um-web-service.md)
  
[Operação PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-operation-um-web-service.md)
  
[Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-operation-um-web-service.md)

