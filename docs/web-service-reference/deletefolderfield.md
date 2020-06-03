---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: O elemento DeleteFolderField representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder.
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462154"
---
# <a name="deletefolderfield"></a>DeleteFolderField

O elemento **DeleteFolderField** representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder. 
  
- [UpdateFolder](updatefolder.md) 
- [FolderChanges](folderchanges.md)  
- [FolderChange](folderchange.md)  
- [Atualizações (pasta)](updates-folder.md) 
- [DeleteFolderField](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

**DeleteFolderFieldType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifica as propriedades com frequência referenciadas por URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifica membros individuais de uma propriedade de dicionário.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica as propriedades de MAPI estendidas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Atualizações (pasta)](updates-folder.md) <br/> |Contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades da pasta.  <br/> A seguir está a expressão XPath para este elemento:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação UpdateFolder](updatefolder-operation.md)

