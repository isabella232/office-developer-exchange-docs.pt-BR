---
title: Status (serviço Web da UM-SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: O elemento status define o valor a ser usado em uma solicitação de operação do SetOofStatus (serviço Web da UM).
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459977"
---
# <a name="status-um-web-service---setoofstatus"></a>Status (serviço Web da UM-SetOofStatus)

O elemento **status** define o valor a ser usado em uma solicitação de [operação do SetOofStatus (serviço Web da um)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (serviço Web da UM)](setoofstatus-um-web-service.md)
  
[Status (serviço Web da UM-SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (serviço Web da UM)](setoofstatus-um-web-service.md) <br/> |Define uma solicitação para definir o status de ausência temporária da Unificação de mensagens do Office (OOF) para o usuário que faz a solicitação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor booliano é necessário. Veja a seguir os valores possíveis:
  
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



[Operação SetOofStatus (serviço Web da UM)](setoofstatus-operation-um-web-service.md)

