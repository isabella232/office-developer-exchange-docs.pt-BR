---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: O elemento MovedEvent representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.
ms.openlocfilehash: 1f8fb57dba7edb769fe0dd658d89c032dccf8c5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530405"
---
# <a name="movedevent"></a>MovedEvent

O elemento **MovedEvent** representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai. 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


**MovedCopiedEventType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Marca d'água](watermark.md) <br/> |Representa um indicador de eventos na tabela de eventos de caixa de correio.  <br/> |
|[Registra](timestamp.md) <br/> |Representa o carimbo de data/hora de um evento de caixa de correio mover item/pasta.  <br/> |
|[FolderId](folderid.md) <br/> |Representa o identificador da pasta movida.  <br/> |
|[ItemId](itemid.md) <br/> |Representa o identificador do item movido.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta que contém o item ou a pasta movido.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Contém o identificador de pasta da pasta original antes de ela ser movida ou copiada.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contém o identificador exclusivo do item original antes de ser movido.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contém o identificador da pasta pai original de um item ou pasta que foi movido.  <br/> |
   
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

