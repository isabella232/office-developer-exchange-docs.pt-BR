---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: O elemento CopiedEvent representa um evento no qual um item ou pasta é copiado.
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529242"
---
# <a name="copiedevent"></a>CopiedEvent

O elemento **CopiedEvent** representa um evento no qual um item ou pasta é copiado. 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
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
|[Registra](timestamp.md) <br/> |Representa o carimbo de data/hora de um evento Copiar item/pasta de caixa de correio.  <br/> |
|[FolderId](folderid.md) <br/> |Representa o identificador da pasta.  <br/> |
|[ItemId](itemid.md) <br/> |Representa o identificador do item.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta que contém a cópia.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Representa o identificador de pasta da pasta original antes de ela ser copiada.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contém o identificador exclusivo do item original antes de ser copiado.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contém o identificador da pasta pai original de um item ou pasta que foi copiado.  <br/> |
   
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
- [Usando assinaturas pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [Aplicativo de amostra de notificação por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

