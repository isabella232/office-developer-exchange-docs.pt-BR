---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: O elemento FolderId contém o identificador e a chave de alteração de uma pasta.
ms.openlocfilehash: 7348fb7342bf33d487591a9daf93a9570f7552f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513679"
---
# <a name="folderid"></a>FolderId

O **elemento FolderId** contém o identificador e a chave de alteração de uma pasta. 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Contém uma cadeia de caracteres que identifica uma pasta no Exchange store. Esse atributo é necessário.  <br/> |
|ChangeKey  <br/> |Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo Id. Esse atributo é opcional. Use esse atributo para garantir que a versão correta de uma pasta seja usada.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta direcionada para ações que usam pastas.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual um item ou pasta é copiado.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para copiar e mover ações.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifica a pasta onde uma nova pasta ou item é criado.  <br/><br/>  Veja a seguir as expressões XPath para este elemento:<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Representa a coleção de pastas que serão mineradas para determinar o conteúdo de uma pasta de pesquisa.  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |Identifica uma única pasta a ser excluído no armazenamento do cliente local.  <br/> |
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Representa uma pasta de calendário em uma caixa de correio.  <br/> |
|[FolderChange](folderchange.md) <br/> |Representa uma coleção de alterações a serem executadas em uma única pasta.  <br/> Veja a seguir a expressão XPath para este elemento:  `/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Representa uma pasta de contato em uma caixa de correio.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas em uma caixa de correio.  <br/> |
|[ToFolderId](tofolderid.md) <br/> | Representa a pasta de destino de um item ou pasta copiado ou movido. <br/> <br/>  Veja a seguir as expressões XPath para este elemento: <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifica a pasta de destino para operações que atualizem, enviem e criem itens no Exchange store.  <br/><br/>  Veja a seguir as expressões XPath para este elemento: <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Representa a pasta que contém os itens a sincronizar.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Representa o nome de um objeto de configuração do usuário. O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifica a ID da pasta para a onde os itens de email serão copiados.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifica a ID da pasta para a onde os itens de email serão movidos.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

Todos **os elementos FolderId** são do **tipo FolderIdType.** O **elemento FolderId** é necessário em todos os casos, exceto em elementos cujo tipo estende **o BaseFolderType** ou onde o **elemento FolderId** faz parte de uma escolha. Revise o esquema para obter mais informações. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Criando Pastas (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

