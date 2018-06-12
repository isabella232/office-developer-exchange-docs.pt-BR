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
description: O elemento MovedEvent representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.
ms.openlocfilehash: a375f421ca9159103e47b515729316b21149c68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824479"
---
# <a name="movedevent"></a>MovedEvent

O elemento **MovedEvent** representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai. 
  
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

 **MovedCopiedEventType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Marca d'água](watermark.md) <br/> |Representa um indicador de eventos na tabela de eventos de caixa de correio.  <br/> |
|[Carimbo de hora](timestamp.md) <br/> |Representa o carimbo de hora de um evento de caixa de correio de item/pasta de movimentação.  <br/> |
|[FolderId](folderid.md) <br/> |Representa o identificador da pasta movido.  <br/> |
|[ItemId](itemid.md) <br/> |Representa o identificador do item movido.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta que contém o item movido ou pasta.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Contém o identificador de pasta da pasta original antes que ele foi movido ou copiado.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contém o identificador exclusivo do item original antes de ser movida.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contém o identificador da pasta pai original de um item ou a pasta que foi movida.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

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

