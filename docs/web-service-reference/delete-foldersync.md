---
title: Excluir (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: O elemento de excluir identifica uma única pasta a ser excluído no repositório de cliente local.
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19751725"
---
# <a name="delete-foldersync"></a>Excluir (FolderSync)

O elemento de **Excluir** identifica uma única pasta a ser excluído no repositório de cliente local. 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)  
- [ResponseMessages](responsemessages.md)  
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [Alterações (hierarquia)](changes-hierarchy.md)  
- [Excluir (FolderSync)](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

**SyncFolderHierarchyDeleteType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Alterações (hierarquia)](changes-hierarchy.md) <br/> |Contém uma matriz sequenciada dos tipos de alteração que representam o tipo das diferenças entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do Exchange 2007 computador que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)
- [Referência do EWS para Exchange](ews-reference-for-exchange.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

