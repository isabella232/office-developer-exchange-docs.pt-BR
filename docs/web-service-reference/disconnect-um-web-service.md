---
title: Desconectar (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: O elemento Disconnect define uma solicitação para desconectar uma chamada.
ms.openlocfilehash: a00d957927a7a97d12c0d8c0c662956a18529cde
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458450"
---
# <a name="disconnect-um-web-service"></a>Desconectar (serviço Web da UM)

O elemento **Disconnect** define uma solicitação para desconectar uma chamada. 
  
- [Desconectar (serviço Web da UM)](disconnect-um-web-service.md)
  
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
|[Callid (serviço Web da UM)](callid-um-web-service.md) <br/> |O identificador da chamada a ser desconectada.  <br/> |
   
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

- [Operação de desconexão (serviço Web da UM)](disconnect-operation-um-web-service.md)  
- [Operação PlayOnPhone (serviço Web da UM)](playonphone-operation-um-web-service.md) 
- [Operação PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md)  
- [Callid (serviço Web da UM)](callid-um-web-service.md)

