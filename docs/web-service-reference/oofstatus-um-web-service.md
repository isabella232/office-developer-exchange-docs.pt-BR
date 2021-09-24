---
title: OofStatus (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: O elemento OofStatus contém um valor que indica o status de Unificação de Mensagens Office para o usuário que está fazendo uma solicitação de operação GetUMProperties (serviço Web de UM).
ms.openlocfilehash: 4e899317defdb4ac4c27c3fdc17d7b7222dff6a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539266"
---
# <a name="oofstatus-um-web-service"></a>OofStatus (serviço Web de Unificação de Mensagens)

O **elemento OofStatus** contém um valor que indica o status de Unificação de Mensagens Office para o usuário que está fazendo uma solicitação de operação [GetUMProperties (serviço Web](getumproperties-operation-um-web-service.md) de UM). 
  
[GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)](getumpropertiesresponse-um-web-service.md)
  
[OofStatus (serviço Web de Unificação de Mensagens)](oofstatus-um-web-service.md)
  
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
|[GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)](getumpropertiesresponse-um-web-service.md) <br/> |Define uma resposta a uma [solicitação de operação GetUMProperties (serviço Web de UM).](getumproperties-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto booleano é necessário. Veja a seguir os valores possíveis:
  
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



[Operação GetUMProperties (serviço Web de Unificação de Mensagens)](getumproperties-operation-um-web-service.md)
  
[GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)](getumpropertiesresponse-um-web-service.md)

