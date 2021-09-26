---
title: Status (serviço Web de Unificação de Mensagens – SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: O elemento Status define o valor a ser usado em uma solicitação de operação SetOofStatus (serviço Web de UM).
ms.openlocfilehash: fc4806e4978ae51ec6113ff8fd45da7db223a071
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546935"
---
# <a name="status-um-web-service---setoofstatus"></a>Status (serviço Web de Unificação de Mensagens – SetOofStatus)

O **elemento Status** define o valor a ser usado em uma solicitação de operação [SetOofStatus (serviço Web de UM).](setoofstatus-operation-um-web-service.md) 
  
[SetOofStatus (serviço Web de Unificação de Mensagens)](setoofstatus-um-web-service.md)
  
[Status (serviço Web de Unificação de Mensagens – SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
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
|[SetOofStatus (serviço Web de Unificação de Mensagens)](setoofstatus-um-web-service.md) <br/> |Define uma solicitação para definir o status de Unificação de Mensagens Office (OOF) para o usuário que faz a solicitação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor Boolean é necessário. Veja a seguir os valores possíveis:
  
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



[Operação SetOofStatus (serviço Web de Unificação de Mensagens)](setoofstatus-operation-um-web-service.md)

