---
title: Status (UM serviço web - SetOofStatus)
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
description: O elemento de Status define o valor a ser usado em uma solicitação do SetOofStatus operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825583"
---
# <a name="status-um-web-service---setoofstatus"></a>Status (UM serviço web - SetOofStatus)

O elemento de **Status** define o valor a ser usado em uma solicitação de [operação SetOofStatus (serviço web de Unificação de mensagens)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (serviço web de Unificação de mensagens)](setoofstatus-um-web-service.md)
  
[Status (UM serviço web - SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (serviço web de Unificação de mensagens)](setoofstatus-um-web-service.md) <br/> |Define uma solicitação para definir o status de Unificação de mensagens fora do escritório (OOF) para o usuário que faz com que a solicitação.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor booleano. Veja a seguir os valores possíveis:
  
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



[Operação de SetOofStatus (serviço web de Unificação de mensagens)](setoofstatus-operation-um-web-service.md)

