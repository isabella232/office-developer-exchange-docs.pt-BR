---
title: Callid (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: O elemento callid contém o valor que representa o identificador da chamada em uma solicitação de solicitação ou desconexão (serviço Web da um) do GetCallInfo.
ms.openlocfilehash: 5d5f596d4a98cbfb4b53be04278dae2305fc10c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529452"
---
# <a name="callid-um-web-service"></a>Callid (serviço Web da UM)

O elemento **callid** contém o valor que representa o identificador da chamada em uma solicitação de solicitação ou [desconexão (](disconnect-um-web-service.md) serviço Web da um) do [GetCallInfo](getcallinfo-um-web-service.md) . 
  
[GetCallInfo (serviço Web da UM)](getcallinfo-um-web-service.md)
  
[Callid (serviço Web da UM)](callid-um-web-service.md)
  
[Desconectar (serviço Web da UM)](disconnect-um-web-service.md)
  
[Callid (serviço Web da UM)](callid-um-web-service.md)
  
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
|[GetCallInfo (serviço Web da UM)](getcallinfo-um-web-service.md) <br/> |Define uma solicitação para obter informações sobre uma chamada.  <br/> |
|[Desconectar (serviço Web da UM)](disconnect-um-web-service.md) <br/> |Define uma solicitação para desconectar uma chamada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor de texto representa o identificador de uma chamada.
  
## <a name="remarks"></a>Comentários

Para fazer uma chamada inicial, use a [operação PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) ou a [operação PlayOnPhoneGreeting (serviço Web da um)](playonphonegreeting-operation-um-web-service.md). Use o valor de texto que é retornado nos elementos [PlayOnPhoneResponse (serviço Web da um)](playonphoneresponse-um-web-service.md) ou [PlayOnPhoneGreetingResponse (serviço Web da um)](playonphonegreetingresponse-um-web-service.md) para o valor de texto do elemento **callid** . 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md)
  
[Operação de desconexão (serviço Web da UM)](disconnect-operation-um-web-service.md)
  
[Operação PlayOnPhone (serviço Web da UM)](playonphone-operation-um-web-service.md)
  
[Operação PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md)

