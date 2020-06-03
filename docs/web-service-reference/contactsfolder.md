---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: O elemento ContactsFolder representa uma pasta de contatos que está contida em uma caixa de correio.
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529431"
---
# <a name="contactsfolder"></a>ContactsFolder

O elemento **ContactsFolder** representa uma pasta de contatos que está contida em uma caixa de correio. 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 **ContactsFolderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta de contatos.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Representa o identificador da pasta pai que contém a pasta contatos.  <br/> |
|[FolderClass](folderclass.md) <br/> |Representa a classe Folder de uma pasta contatos.  <br/> |
|[DisplayName (cadeia de caracteres)](displayname-string.md) <br/> |Contém o nome de exibição de uma pasta de contatos.  <br/> |
|[TotalCount](totalcount.md) <br/> |Representa a contagem total de itens em uma pasta contatos.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Representa o número de pastas filhas que estão contidas em uma pasta de contatos. Essa propriedade é somente leitura.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas nas pastas de contatos.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contém informações sobre uma pasta gerenciada.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.  <br/> |
|[SharingEffectiveRights (PermissionReadAccessType)](sharingeffectiverights-permissionreadaccesstype.md) <br/> |Indica as permissões que o usuário tem para os dados de contato que estão sendo compartilhados.  <br/> |
|[PermissionSet (PermissionSettype)](permissionset-permissionsettype.md) <br/> |Contém todas as permissões configuradas para uma pasta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Criar (FolderSync)](create-foldersync.md) <br/> |Identifica uma única pasta a ser criada no armazenamento do cliente local.  <br/> |
|[Setfolderfield](setfolderfield.md) <br/> |Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Atualização (FolderSync)](update-foldersync.md) <br/> |Identifica uma única pasta a ser atualizada no repositório do cliente local.  <br/> |
|[Pastas](folders-ex15websvcsotherref.md) <br/> |Contém uma matriz de pastas que são usadas em operações de pasta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

