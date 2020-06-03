---
title: SetPlayOnPhoneDialString (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: O elemento SetPlayOnPhoneDialString define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações PlayOnPhone (serviço Web da UM) e PlayOnPhoneGreeting (serviço Web da UM).
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458625"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (serviço Web da UM)

O elemento **SetPlayOnPhoneDialString** define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações [PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e [PLAYONPHONEGREETING (serviço Web da um)](playonphonegreeting-operation-um-web-service.md) . 
  
[SetPlayOnPhoneDialString (serviço Web da UM)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[dialstring (serviço Web da UM)](dialstring-um-web-service.md) <br/> |O número de telefone a ser definido como a cadeia de caracteres de discagem padrão.  <br/> |
   
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



[Operação SetPlayOnPhoneDialString (serviço Web da UM)](setplayonphonedialstring-operation-um-web-service.md)

