---
title: IsUMEnabled (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: O elemento IsUMEnabled indica se uma caixa de correio está habilitada para a Unificação de Mensagens.
ms.openlocfilehash: 43632c28c5fb0c526dcf2ad936784953b00cc14a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524116"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (serviço Web de Unificação de Mensagens)

O **elemento IsUMEnabled** indica se uma caixa de correio está habilitada para a Unificação de Mensagens. 
  
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

Um valor de texto que representa um valor Boolean é necessário se esse elemento for incluído. Um valor **true** indica que a caixa de correio está habilitada para a Unificação de Mensagens. Um valor falso **significa** que a caixa de correio não está habilitada para a Unificação de Mensagens. 
  
## <a name="remarks"></a>Comentários

Para determinar se uma caixa de correio está habilitada para a Unificação de Mensagens, use a operação [IsUMEnabled (serviço Web da UM)](isumenabled-operation-um-web-service.md).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação IsUMEnabled (serviço Web de Unificação de Mensagens)](isumenabled-operation-um-web-service.md)


[Elementos XML do serviço Web de Unificação de Mensagens para Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

