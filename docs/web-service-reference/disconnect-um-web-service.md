---
title: Disconnect (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: O elemento Disconnect define uma solicitação para desconectar uma chamada.
ms.openlocfilehash: 6aaff910d85a963a926e7c2a74a91963b120392c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538370"
---
# <a name="disconnect-um-web-service"></a>Disconnect (serviço Web de Unificação de Mensagens)

O **elemento Disconnect** define uma solicitação para desconectar uma chamada. 
  
- [Disconnect (serviço Web de Unificação de Mensagens)](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 **complexType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md) <br/> |O identificador da chamada a ser desconectada.  <br/> |
   
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

- [Operação Disconnect (serviço Web de Unificação de mensagens)](disconnect-operation-um-web-service.md)  
- [Operação PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-operation-um-web-service.md) 
- [Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-operation-um-web-service.md)  
- [CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md)

