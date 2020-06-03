---
title: DeletedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: O elemento DeletedEvent representa um evento no qual um item ou pasta é excluído.
ms.openlocfilehash: 5eb0c947aacc592f81c595da2cc00bf4874f300b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526939"
---
# <a name="deletedevent"></a>DeletedEvent

O elemento **DeletedEvent** representa um evento no qual um item ou pasta é excluído. 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</DeletedEvent>
```

**BaseObjectChangedEventType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio.  <br/> |
|[Registra](timestamp.md) <br/> |Representa o carimbo de data/hora de um evento de caixa de correio de pasta ou item excluído.  <br/> |
|[FolderId](folderid.md) <br/> |Representa o identificador da pasta excluída.  <br/> |
|[ItemId](itemid.md) <br/> |Representa o identificador do item excluído.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai do item ou pasta excluído antes da exclusão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação Subscribe](subscribe-operation.md)  
- [Operação GetEvents](getevents-operation.md)  
- [Cancelar a operação](unsubscribe-operation.md)

