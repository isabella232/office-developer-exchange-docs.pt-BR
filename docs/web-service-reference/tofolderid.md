---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: O elemento ToFolderId representa a pasta de destino para uma pasta ou item copiado ou movido.
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468772"
---
# <a name="tofolderid"></a>ToFolderId

O elemento **ToFolderId** representa a pasta de destino para uma pasta ou item copiado ou movido. 
  
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
|[FolderId](folderid.md) <br/> |Contém o identificador de uma pasta de destino para uma pasta ou item copiado ou movido.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino nomeada para uma pasta ou item copiado ou movido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover um item no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar um item no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/CopyItem` <br/> |
   
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

