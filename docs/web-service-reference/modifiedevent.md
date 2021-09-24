---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: O elemento ModifiedEvent representa um evento no qual um item ou pasta é modificado.
ms.openlocfilehash: 92002c2824168687e6984913dbf46ee85da921e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539356"
---
# <a name="modifiedevent"></a>ModifiedEvent

O **elemento ModifiedEvent** representa um evento no qual um item ou pasta é modificado. 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

**ModifiedEventType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Representa o data/hora de um evento de caixa de correio de item ou pasta modificado.  <br/> |
|[FolderId](folderid.md) <br/> |Representa o identificador da pasta modificada.  <br/> |
|[ItemId](itemid.md) <br/> |Representa o identificador do item modificado.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai do item ou pasta modificado.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Representa a contagem de itens não lidos em uma determinada pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

Dois eventos modificados são gerados para cada modificação de um item em uma pasta. Um evento é relevante para o item que foi alterado. O outro evento é relevante para a pasta pai do item. Essa é a mesma pasta em que a assinatura foi criada. O evento associado à pasta é usado para comunicar uma possível alteração à [propriedade UnreadCount](unreadcount.md) na pasta. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação Subscribe](subscribe-operation.md)  
- [Operação GetEvents](getevents-operation.md)  
- [Cancelar a operação](unsubscribe-operation.md)

