---
title: GetUMPropertiesResponse (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: O elemento de GetUMPropertiesResponse define uma resposta a uma solicitação do GetUMProperties operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823685"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (serviço web de Unificação de mensagens)

O elemento de **GetUMPropertiesResponse** define uma resposta a uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (serviço web de Unificação de mensagens)](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **UMProperties**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MissedCallNotificationEnabled (serviço web de Unificação de mensagens)](missedcallnotificationenabled-um-web-service.md) <br/> |Indica se as notificações de chamadas perdidas estão habilitadas.  <br/> |
|[PlayOnPhoneDialString (serviço web de Unificação de mensagens)](playonphonedialstring-um-web-service.md) <br/> |Contém a cadeia de caracteres de discagem padrão a ser usado para a [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) e a [operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (serviço web de Unificação de mensagens)](telephoneaccessnumbers-um-web-service.md) <br/> |Contém a lista de números de telefone que o usuário pode usar para acessar a Unificação de mensagens por meio de um telefone.  <br/> |
|[TelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contém o identificador para a pasta de email do qual Unificação de mensagens lê as mensagens por telefone.  <br/> |
   
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



[Operação de GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md)

