---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: O elemento de CalendarPermission define o que um usuário tem acesso a uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751359"
---
# <a name="calendarpermission"></a>CalendarPermission

O elemento de **CalendarPermission** define o que um usuário tem acesso a uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |Representa o nível de permissão que um usuário tem em uma pasta de calendário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |Indica se um usuário tem permissão para criar itens em uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Indica se um usuário tem permissão para criar subpastas em uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Indica se um usuário tem permissão para excluir itens em uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[EditItems](edititems.md) <br/> |Indica se um usuário tem permissão para editar itens em uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Indica se um usuário é um contato para uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Indica se um usuário é o proprietário de uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Indica se um usuário pode exibir uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |Indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[UserId](userid.md) <br/> |Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Contém uma matriz de permissões de calendário de uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões de nível de pasta](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

