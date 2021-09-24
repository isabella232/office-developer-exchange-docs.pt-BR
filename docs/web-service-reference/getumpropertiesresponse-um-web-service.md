---
title: GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: O elemento GetUMPropertiesResponse define uma resposta a uma solicitação de operação GetUMProperties (serviço Web da UM).
ms.openlocfilehash: 97c3850d46369d4ab533629a8b24e199db3dd44a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522961"
---
# <a name="getumpropertiesresponse-um-web-service"></a>GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)

O **elemento GetUMPropertiesResponse** define uma resposta a uma solicitação de operação [GetUMProperties (serviço Web](getumproperties-operation-um-web-service.md) da UM). 
  
[GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)](getumpropertiesresponse-um-web-service.md)
  
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
|[MissedCallNotificationEnabled (serviço Web de Unificação de Mensagens)](missedcallnotificationenabled-um-web-service.md) <br/> |Indica se as notificações de chamada perdidas estão habilitadas.  <br/> |
|[PlayOnPhoneDialString (serviço Web de Unificação de Mensagens)](playonphonedialstring-um-web-service.md) <br/> |Contém a cadeia de caracteres de discagem padrão a ser usada para a operação [PlayOnPhone (serviço Web](playonphone-operation-um-web-service.md) de UM) e a operação [PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md).  <br/> |
|[TelephoneAccessNumbers (serviço Web de Unificação de Mensagens)](telephoneaccessnumbers-um-web-service.md) <br/> |Contém a lista de números de telefone que o usuário pode usar para acessar a Unificação de Mensagens por meio de um telefone.  <br/> |
|[TelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](telephoneaccessfolderemail-um-web-service.md) <br/> |Contém o identificador da pasta de email da qual a Unificação de Mensagens lerá mensagens por telefone.  <br/> |
   
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



[Operação GetUMProperties (serviço Web de Unificação de Mensagens)](getumproperties-operation-um-web-service.md)

