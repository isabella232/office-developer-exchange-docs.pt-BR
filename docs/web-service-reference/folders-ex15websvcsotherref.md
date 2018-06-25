---
title: Pastas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: O elemento de pastas contém uma matriz das pastas que são usadas nas operações da pasta.
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752338"
---
# <a name="folders"></a>Pastas

O elemento de **pastas** contém uma matriz das pastas que são usadas nas operações da pasta. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

 **ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Identifica uma pasta para criar, obter, encontre, sincronizar ou atualizar.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta que contém principalmente itens de calendário.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contatos em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa contida em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CopyFolder](copyfolder-operation.md) solicitação.  <br/> |
|[CreateFolder](createfolder.md) <br/> |Define uma solicitação para criar uma pasta no repositório do Exchange.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CreateFolder](createfolder-operation.md) solicitação.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação CreateManagedFolder](createmanagedfolder-operation.md) solicitação.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação GetFolder](getfolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de [operação MoveFolder](movefolder-operation.md) .  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifica a pasta onde uma nova pasta é criada.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Contém os resultados de verificação ortográfica de uma pasta raiz única durante uma [operação FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contém o status e o resultado de uma única [operação UpdateFolder](updatefolder-operation.md) solicitação.  <br/> |
   
## <a name="remarks"></a>Comentários

Este é um elemento necessário filho do elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

