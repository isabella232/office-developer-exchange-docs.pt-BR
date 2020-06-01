---
title: TasksFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: O elemento TasksFolder representa uma pasta de tarefas que está contida em uma caixa de correio.
ms.openlocfilehash: 522fe485482bd8159927f9925b7a5582ba2e1c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465335"
---
# <a name="tasksfolder"></a>TasksFolder

O elemento **TasksFolder** representa uma pasta de tarefas que está contida em uma caixa de correio. 
  
```xml
<TasksFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
      <EffectiveRights/>
</TasksFolder>
```

**TasksFolderType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta tarefas.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém a pasta tarefas.  <br/> |
|[FolderClass](folderclass.md) <br/> |Representa a classe Folder de uma pasta tarefas.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Contém o nome de exibição de uma pasta tarefas.  <br/> |
|[TotalCount](totalcount.md) <br/> |Representa a contagem total de itens em uma pasta tarefas.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Representa o número de pastas filhas que estão contidas em uma pasta tarefas. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em uma pasta tarefas.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Representa a contagem de itens não lidos em uma pasta tarefas.  <br/> |
|[PermissionSet (PermissionSettype)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta. Este elemento é somente leitura. Este elemento foi introduzido no Microsoft Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Criar (FolderSync)](create-foldersync.md) <br/> |Identifica uma única pasta a ser criada no armazenamento do cliente local.  <br/> |
|[Setfolderfield](setfolderfield.md) <br/> |Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Atualização (FolderSync)](update-foldersync.md) <br/> |Identifica uma única pasta a ser atualizada no repositório do cliente local.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas que são usadas em operações de pasta.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

