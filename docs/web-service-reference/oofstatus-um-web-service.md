---
title: OofStatus (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: O elemento OofStatus contém um valor que indicaties o status de Unificação de mensagens de ausência temporária para o usuário que está fazendo uma solicitação do GetUMProperties operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824650"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (serviço web de Unificação de mensagens)

O elemento **OofStatus** contém um valor que indicaties o status de Unificação de mensagens de ausência temporária para o usuário que está fazendo uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (serviço web de Unificação de mensagens)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (serviço web de Unificação de mensagens)](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUMPropertiesResponse (serviço web de Unificação de mensagens)](getumpropertiesresponse-um-web-service.md) <br/> |Define uma resposta a uma solicitação de [operação GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Text value

Um valor booleano de texto é necessário. Veja a seguir os valores possíveis:
  
- True
    
- False
    
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (serviço web de Unificação de mensagens)](getumpropertiesresponse-um-web-service.md)

