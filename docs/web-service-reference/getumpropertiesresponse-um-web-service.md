---
title: GetUMPropertiesResponse (serviço Web da UM)
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
description: O elemento GetUMPropertiesResponse define uma resposta a uma solicitação de operação GetUMProperties (serviço Web da UM).
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459122"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (serviço Web da UM)

O elemento **GetUMPropertiesResponse** define uma resposta a uma solicitação de [operação GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (serviço Web da UM)](getumpropertiesresponse-um-web-service.md)
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MissedCallNotificationEnabled (serviço Web da UM)](missedcallnotificationenabled-um-web-service.md) <br/> |Indica se as notificações de chamadas perdidas estão habilitadas.  <br/> |
|[PlayOnPhoneDialString (serviço Web da UM)](playonphonedialstring-um-web-service.md) <br/> |Contém a cadeia de caracteres de discagem padrão a ser usada para a [operação PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço da um)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (serviço Web da UM)](telephoneaccessnumbers-um-web-service.md) <br/> |Contém a lista de números de telefone que o usuário pode usar para acessar a Unificação de mensagens por telefone.  <br/> |
|[TelephoneAccessFolderEmail (serviço Web da UM)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contém o identificador da pasta de email a partir da qual a Unificação de mensagens lerá as mensagens por telefone.  <br/> |
   
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



[Operação GetUMProperties (serviço Web da UM)](getumproperties-operation-um-web-service.md)

