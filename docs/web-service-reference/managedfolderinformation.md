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
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824341"
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |Indica se uma pasta gerenciada pode ser excluída por um cliente.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Indica se uma determinada pasta gerenciada pode ser renomeada ou movida pelo cliente.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Indica se o comentário de pasta gerenciada deve ser exibido.  <br/> |
|[HasQuota](hasquota.md) <br/> |Indica se a pasta gerenciada tem uma cota.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Indica se a pasta gerenciada é a raiz para todas as pastas gerenciadas.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Contém a ID de pasta da pasta gerenciada.  <br/> |
|[Comment](comment.md) <br/> |Contém o comentário associado uma pasta gerenciada.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Descreve a cota de armazenamento para a pasta gerenciada.  <br/> |
|[FolderSize](foldersize.md) <br/> |Descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.  <br/> |
|[Home page](homepage.md) <br/> |Especifica a URL que será a home page padrão para a pasta gerenciada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Representa uma pasta no repositório do Exchange. Pastas personalizadas gerenciadas só podem ser subpastas da pasta denominada **Pastas gerenciadas**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Não aplicável.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Não aplicável.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Não aplicável.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Não aplicável.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação CreateManagedFolder](createmanagedfolder-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionando pastas gerenciadas](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

