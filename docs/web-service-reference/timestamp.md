---
title: Carimbo de hora
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
description: O elemento de carimbo de hora representa o carimbo de hora de um evento de caixa de correio.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837791"
---
# <a name="timestamp"></a>Carimbo de hora

O elemento de **carimbo de hora** representa o carimbo de hora de um evento de caixa de correio. 
  
```xml
<TimeStamp/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento onde uma pasta ou um item é copiada.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento onde uma pasta ou um item é criada.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento onde uma pasta ou um item é excluída.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento onde um item ou pasta é modificada.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento onde uma pasta ou um item é movida da pasta pai de um para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

Esta propriedade é somente leitura.
  
## <a name="remarks"></a>Comentários

Este elemento está disponível principalmente para uso na determinação do cliente da frequência de evento. Isso não está presente no [StatusEvent](statusevent.md).
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

