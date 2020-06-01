---
title: IsUMEnabled (serviço Web da UM)
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
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458226"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (serviço Web da UM)

O elemento **IsUMEnabled** indica se uma caixa de correio está habilitada para Unificação de mensagens. 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor booliano é necessário se esse elemento for incluído. Um valor **true** indica que a caixa de correio está habilitada para Unificação de mensagens. Um valor **false** significa que a caixa de correio não está habilitada para Unificação de mensagens. 
  
## <a name="remarks"></a>Comentários

Para determinar se uma caixa de correio está habilitada para Unificação de mensagens, use a [operação IsUMEnabled (serviço da um da Web)](isumenabled-operation-um-web-service.md).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação IsUMEnabled (serviço Web da UM)](isumenabled-operation-um-web-service.md)


[Elementos XML do serviço Web de Unificação de mensagens para o Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

