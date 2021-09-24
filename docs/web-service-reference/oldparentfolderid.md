---
title: OldParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: O elemento OldParentFolderId contém o identificador da pasta pai de um item ou pasta que foi copiado ou movido.
ms.openlocfilehash: 9cf7eb834c0c7b70f234df26b466977e8e11957a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537454"
---
# <a name="oldparentfolderid"></a>OldParentFolderId

O **elemento OldParentFolderId** contém o identificador da pasta pai de um item ou pasta que foi copiado ou movido. 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Contém uma cadeia de caracteres que identifica uma pasta no Exchange store. Esse atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo Id. Esse atributo é opcional. Use esse atributo para garantir que a versão correta de uma pasta seja usada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual um item ou pasta é copiado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

