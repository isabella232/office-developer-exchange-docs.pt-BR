---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: O elemento ManagedFolderInformation contém informações sobre uma pasta personalizada gerenciada.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44450946"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

O elemento **ManagedFolderInformation** contém informações sobre uma pasta personalizada gerenciada. 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 **ManagedFolderInformationType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |Indica se uma pasta gerenciada pode ser excluída por um cliente.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Indica se uma determinada pasta gerenciada pode ser renomeada ou movida pelo cliente.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Indica se o comentário da pasta gerenciada deve ser exibido.  <br/> |
|[HasQuota](hasquota.md) <br/> |Indica se a pasta gerenciada tem uma cota.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Indica se a pasta gerenciada é a raiz de todas as pastas gerenciadas.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Contém a ID da pasta gerenciada.  <br/> |
|[Comment](comment.md) <br/> |Contém o comentário associado a uma pasta gerenciada.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Descreve a cota de armazenamento da pasta gerenciada.  <br/> |
|[FolderSize](foldersize.md) <br/> |Descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.  <br/> |
|[HomePage](homepage.md) <br/> |Especifica a URL que será a Home Page padrão para a pasta gerenciada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Representa uma pasta no repositório do Exchange. Pastas personalizadas gerenciadas só podem ser subpastas da pasta denominada **pastas gerenciadas**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Não aplicável.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Não aplicável.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Não aplicável.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Não aplicável.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionando pastas gerenciadas](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

