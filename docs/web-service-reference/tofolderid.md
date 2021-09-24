---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: O elemento ToFolderId representa a pasta de destino de um item ou pasta copiado ou movido.
ms.openlocfilehash: b58192aa4d1ffe609da78dfdf1b5c86522fc45c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515163"
---
# <a name="tofolderid"></a>ToFolderId

O **elemento ToFolderId** representa a pasta de destino de um item ou pasta copiado ou movido. 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador de uma pasta de destino para um item ou pasta copiado ou movido.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino nomeada para um item ou pasta copiado ou movido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação MoveFolder](movefolder-operation.md)  
- [Operação CopyFolder](copyfolder-operation.md) 
- [Operação MoveItem](moveitem-operation.md) 
- [Operação CopyItem](copyitem-operation.md)

