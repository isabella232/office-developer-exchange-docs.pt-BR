---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: O elemento ParentFolderIds identifica pastas para as operações FindItem e FindFolder a ser pesquisadas.
ms.openlocfilehash: e9e0f14651b205ad64be04dbe1d0707a109f3edc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512900"
---
# <a name="parentfolderids"></a>ParentFolderIds

O **elemento ParentFolderIds** identifica pastas para as operações FindItem e FindFolder a ser pesquisadas. 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

**NonEmptyArrayOfBaseFolderIdsType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta. O **elemento ParentFolderIds** deve usar esse elemento ou [o elemento DistinguishedFolderId.](distinguishedfolderid.md)  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica Microsoft Exchange Server pastas 2007 que podem ser referenciadas pelo nome. O **elemento ParentFolderIds** deve usar esse elemento ou o [elemento FolderId.](folderid.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Define uma solicitação para identificar pastas em uma caixa de correio.  <br/> |
|[FindItem](finditem.md) <br/> |Define uma solicitação para encontrar itens em uma caixa de correio.  <br/> |
|[ResolveNames](resolvenames.md) <br/> |Define uma solicitação para resolver nomes ambíguos.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento ParentFolderIds** deve usar [o elemento FolderId](folderid.md) ou [DistinguishedFolderId.](distinguishedfolderid.md) Um número ilimitado de pastas pode ser definido para a pesquisa. 
  
## <a name="example"></a>Exemplo

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindFolder](findfolder-operation.md)  
- [Operação FindItem](finditem-operation.md) 
- [Operação ResolveNames](resolvenames-operation.md)

