---
title: Permissão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: O elemento Permission define o acesso que um usuário tem a uma pasta.
ms.openlocfilehash: bc3e140aaf7bd9ea7f1a4993c9bea1dcad8d39fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512664"
---
# <a name="permission"></a>Permissão

O **elemento Permission** define o acesso que um usuário tem a uma pasta. 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CanCreateItems](cancreateitems.md) <br/> |Indica se um usuário tem permissão para criar itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Indica se um usuário tem permissão para criar subpastas em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Indica se um usuário tem permissão para excluir itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[EditItems](edititems.md) <br/> |Indica se um usuário tem permissão para editar itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Indica se um usuário é um contato para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Indica se um usuário é o proprietário de uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Indica se um usuário pode exibir uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |Representa a combinação de permissões que um usuário tem em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |Indica se um usuário tem permissão para ler itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso à pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Permissões](permissions.md) <br/> |Contém todas as permissões configuradas para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
Esse elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).
  
### <a name="version-differences"></a>Diferenças de versão

Para aplicativos destinados Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o [elemento BaseShape](baseshape.md) tem um valor **allProperties** no [GetFolder](getfolder-operation.md) solicitação de operação. Para recuperar permissões de pasta, adicione o [elemento PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao [elemento AdditionalProperties](additionalproperties.md) na **solicitação GetFolder.** 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

