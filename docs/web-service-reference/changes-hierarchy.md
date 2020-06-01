---
title: Alterações (hierarquia)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: O elemento changes contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463269"
---
# <a name="changes-hierarchy"></a>Alterações (hierarquia)

O elemento **Changes** contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007. 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[Alterações (hierarquia)](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **SyncFolderHierarchyChangesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Criar (FolderSync)](create-foldersync.md) <br/> |Identifica uma única pasta a ser criada no armazenamento do cliente local.  <br/> |
|[Atualização (FolderSync)](update-foldersync.md) <br/> |Identifica uma única pasta a ser atualizada no repositório do cliente local.  <br/> |
|[Excluir (FolderSync)](delete-foldersync.md) <br/> |Identifica uma única pasta a ser excluída no repositório do cliente local.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação SyncFolderHierarchy.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um valor booliano é necessário.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SyncFolderHierarchy](syncfolderhierarchy-operation.md)


[Referência do EWS para Exchange](ews-reference-for-exchange.md)
  
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

