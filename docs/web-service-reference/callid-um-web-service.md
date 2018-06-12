---
title: CallId (serviço web de Unificação de mensagens)
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
description: O elemento de CallId contém o valor que representa o identificador da chamada em uma solicitação do GetCallInfo (serviço web de Unificação de mensagens) ou Disconnect (serviço web de Unificação de mensagens).
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751372"
---
# <a name="callid-um-web-service"></a>CallId (serviço web de Unificação de mensagens)

O elemento de **CallId** contém o valor que representa o identificador da chamada em uma solicitação de [GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-um-web-service.md) ou [Disconnect (serviço web de Unificação de mensagens)](disconnect-um-web-service.md) . 
  
[GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-um-web-service.md)
  
[CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md)
  
[Desconectar (serviço web de Unificação de mensagens)](disconnect-um-web-service.md)
  
[CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md)
  
```xml
<CallId/>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-um-web-service.md) <br/> |Define uma solicitação para obter mais informações sobre uma chamada.  <br/> |
|[Desconectar (serviço web de Unificação de mensagens)](disconnect-um-web-service.md) <br/> |Define uma solicitação para desconectar chamada.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto representa o identificador para uma chamada.
  
## <a name="remarks"></a>Coment�rios

Para iniciais uma chamada, use a [operação de PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) ou [PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md). Use o valor de texto que é retornado nos elementos [PlayOnPhoneResponse (serviço web de Unificação de mensagens)](playonphoneresponse-um-web-service.md) ou [PlayOnPhoneGreetingResponse (serviço web de Unificação de mensagens)](playonphonegreetingresponse-um-web-service.md) para o valor de texto do elemento **CallId** . 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md)
  
[Desconectar a operação (serviço web de Unificação de mensagens)](disconnect-operation-um-web-service.md)
  
[Operação de PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md)
  
[Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md)

