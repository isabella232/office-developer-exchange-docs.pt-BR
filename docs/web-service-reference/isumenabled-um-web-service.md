---
title: IsUMEnabled (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: O elemento IsUMEnabled indica se uma caixa de correio está habilitada para Unificação de mensagens.
ms.openlocfilehash: 5f4d59c5497158e5afbc8bb5db4900bd129df50b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824113"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (serviço web de Unificação de mensagens)

O elemento **IsUMEnabled** indica se uma caixa de correio está habilitada para Unificação de mensagens. 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Um valor de texto que representa um valor booleano é necessário se este elemento é incluído. Um valor **true** indica que a caixa de correio está habilitada para Unificação de mensagens. Um valor **false** significa que a caixa de correio não está habilitada para Unificação de mensagens. 
  
## <a name="remarks"></a>Comentários

Para determinar se uma caixa de correio está habilitada para Unificação de mensagens, use a [operação IsUMEnabled (serviço web de Unificação de mensagens)](isumenabled-operation-um-web-service.md).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de IsUMEnabled (serviço web de Unificação de mensagens)](isumenabled-operation-um-web-service.md)


[Unified Messaging web service os elementos XML para o Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

