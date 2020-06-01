---
title: Registra
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: O elemento timestamp representa o carimbo de data/hora de um evento de caixa de correio.
ms.openlocfilehash: f2280d4eab67b603963c4f0a7468bf35a2b63a88
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459886"
---
# <a name="timestamp"></a>Registra

O elemento **timestamp** representa o carimbo de data/hora de um evento de caixa de correio. 
  
```xml
<TimeStamp/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento em que um item ou pasta é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento em que um item ou pasta é criado.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento em que um item ou pasta é excluído.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento em que um item ou pasta é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento em que um item ou pasta é movido de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Essa propriedade é somente leitura.
  
## <a name="remarks"></a>Comentários

Este elemento está disponível principalmente para uso na determinação do cliente da frequência de eventos. Isso não está presente no [StatusEvent](statusevent.md).
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

