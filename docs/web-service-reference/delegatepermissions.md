---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: O elemento DelegatePermissions contém as configurações de delegação de nível de permissão para um usuário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 2cf8c9a8d3c5db8e13d43c207df173c12fca5acb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457407"
---
# <a name="delegatepermissions"></a>DelegatePermissions

O elemento **DelegatePermissions** contém as configurações de delegação de nível de permissão para um usuário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

**DelegatePermissionsType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarFolderPermissionLevel](calendarfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta de calendário padrão. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[TasksFolderPermissionLevel](tasksfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta de tarefas padrão. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[InboxFolderPermissionLevel](inboxfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta de caixa de entrada padrão. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[ContactsFolderPermissionLevel](contactsfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta de contatos padrão. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[NotesFolderPermissionLevel](notesfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta padrão de anotações. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[JournalFolderPermissionLevel](journalfolderpermissionlevel.md) <br/> |Contém as permissões para a pasta de diário padrão. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifica um único representante para adicionar ou atualizar em uma caixa de correio. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação AddDelegate](adddelegate-operation.md) 
- [Operação UpdateDelegate](updatedelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionar representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

