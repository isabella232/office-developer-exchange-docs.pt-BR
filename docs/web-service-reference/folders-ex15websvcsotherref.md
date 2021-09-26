---
title: Folders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: O elemento Folders contém uma matriz de pastas que são usadas em operações de pasta.
ms.openlocfilehash: 77442965c9d372a2895404cf1c919be38e98abb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546431"
---
# <a name="folders"></a>Folders

O **elemento Folders** contém uma matriz de pastas que são usadas em operações de pasta. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Identifica uma pasta para criar, obter, encontrar, sincronizar ou atualizar.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta Contatos em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de Pesquisa contida em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta Tarefas em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CopyFolder.](copyfolder-operation.md)  <br/> |
|[CreateFolder](createfolder.md) <br/> |Define uma solicitação para criar uma pasta no Exchange store.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateFolder.](createfolder-operation.md)  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação CreateManagedFolder.](createmanagedfolder-operation.md)  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação GetFolder.](getfolder-operation.md)  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma [solicitação de operação MoveFolder.](movefolder-operation.md)  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifica a pasta onde uma nova pasta é criada.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Contém os resultados da pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação UpdateFolder.](updatefolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é um elemento filho necessário do [elemento ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md) 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2010 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

