---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: O elemento CalendarPermission define o acesso que um usuário tem a uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7794cab261653f8cb6421d4e0633d496ba347a5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514799"
---
# <a name="calendarpermission"></a>CalendarPermission

O **elemento CalendarPermission** define o acesso que um usuário tem a uma pasta Calendário. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **CalendarPermissionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |Representa o nível de permissão que um usuário tem em uma pasta Calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |Indica se um usuário tem permissão para criar itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Indica se um usuário tem permissão para criar subpastas em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Indica se um usuário tem permissão para excluir itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[EditItems](edititems.md) <br/> |Indica se um usuário tem permissão para editar itens em uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Indica se um usuário é um contato para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Indica se um usuário é o proprietário de uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Indica se um usuário pode exibir uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |Indica se um usuário tem permissão para ler itens em uma pasta de calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário com permissões de acesso à pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Contém uma matriz de permissões de calendário para uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
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

