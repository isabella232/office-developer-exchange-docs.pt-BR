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
description: O elemento ToFolderId representa a pasta de destino para um item movido ou copiada ou uma pasta.
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353655"
---
# <a name="tofolderid"></a>ToFolderId

O elemento **ToFolderId** representa a pasta de destino para um item movido ou copiada ou uma pasta. 
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador de uma pasta de destino para um item movido ou copiada ou uma pasta.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino nomeado para um item movido ou copiada ou uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Define uma solicitação para mover uma pasta no repositório do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Define uma solicitação para copiar uma pasta no repositório do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover um item no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar um item no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação MoveFolder](movefolder-operation.md)  
- [Operação CopyFolder](copyfolder-operation.md) 
- [Operação MoveItem](moveitem-operation.md) 
- [Operação CopyItem](copyitem-operation.md)

