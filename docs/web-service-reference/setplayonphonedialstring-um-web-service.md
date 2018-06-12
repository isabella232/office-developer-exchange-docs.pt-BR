---
title: SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)
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
description: O elemento SetPlayOnPhoneDialString define uma solicitação para definir a sequência de discagem padrão para a operação de PlayOnPhone (serviço web de Unificação de mensagens) e PlayOnPhoneGreeting solicitações de operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825450"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)

O elemento de **SetPlayOnPhoneDialString** define uma solicitação para definir a sequência de discagem padrão para solicitações de [operação de PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) e [a operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md) . 
  
[SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[dialString (serviço web de Unificação de mensagens)](dialstring-um-web-service.md) <br/> |O número de telefone para definir como a cadeia de caracteres de discagem padrão.  <br/> |
   
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



[Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)](setplayonphonedialstring-operation-um-web-service.md)

