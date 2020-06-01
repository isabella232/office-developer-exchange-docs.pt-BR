---
title: OofStatus (serviço Web da UM)
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
description: O elemento OofStatus contém um valor que indicaties o status da Unificação de mensagens do Office para o usuário que está fazendo uma solicitação de GetUMProperties (serviço Web da UM).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460572"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (serviço Web da UM)

O elemento **OofStatus** contém um valor que indicaties o status da Unificação de mensagens do Office para o usuário que está fazendo uma solicitação de [GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) . 
  
[GetUMPropertiesResponse (serviço Web da UM)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (serviço Web da UM)](oofstatus-um-web-service.md)
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetUMPropertiesResponse (serviço Web da UM)](getumpropertiesresponse-um-web-service.md) <br/> |Define uma resposta a uma solicitação de [operação do GetUMProperties (serviço Web da um)](getumproperties-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto booliano é necessário. Veja a seguir os valores possíveis:
  
- Verdadeiro
    
- Falso
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetUMProperties (serviço Web da UM)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (serviço Web da UM)](getumpropertiesresponse-um-web-service.md)

