---
title: SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: O elemento SetPlayOnPhoneDialString define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações de operação do PlayOnPhone (serviço Web de UM) e PlayOnPhoneGreeting (serviço Web da UM).
ms.openlocfilehash: e485fd092da29a3f54b1acc2b7e50167084e13fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540500"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)

O **elemento SetPlayOnPhoneDialString** define uma solicitação para definir a cadeia de caracteres de discagem padrão para as solicitações de operação do [PlayOnPhone (serviço Web de UM)](playonphone-operation-um-web-service.md) e [PlayOnPhoneGreeting (serviço Web](playonphonegreeting-operation-um-web-service.md) da UM). 
  
[SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)](setplayonphonedialstring-um-web-service.md)
  
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
|[dialString (serviço Web de Unificação de Mensagens)](dialstring-um-web-service.md) <br/> |O número de telefone a ser definido como a cadeia de caracteres de discagem padrão.  <br/> |
   
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



[Operação SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)](setplayonphonedialstring-operation-um-web-service.md)

