---
title: Delete (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: O elemento Delete identifica uma única pasta a ser excluído no armazenamento de cliente local.
ms.openlocfilehash: bd57c2f093fceda9948d8289fbd55b527bcf10cc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542495"
---
# <a name="delete-foldersync"></a>Delete (FolderSync)

O **elemento Delete** identifica uma única pasta a ser excluído no armazenamento de cliente local. 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)  
- [ResponseMessages](responsemessages.md)  
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [Changes (Hierarchy)](changes-hierarchy.md)  
- [Delete (FolderSync)](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

**SyncFolderHierarchyDeleteType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Changes (Hierarchy)](changes-hierarchy.md) <br/> |Contém uma matriz sequenciada de tipos de alteração que representam o tipo de diferenças entre as pastas no cliente e as pastas no computador que está executando Microsoft Exchange Server 2007.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador Exchange 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

