---
title: CalendarFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolderPermissionLevel
api_type:
- schema
ms.assetid: 2a5c9381-dc2c-4fc6-b9b5-893477d0970e
description: O elemento CalendarFolderPermissionLevel contém as permissões para a pasta de calendário padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: dcbd57da42b5e701d898c3756ce9bcc100c20af7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461461"
---
# <a name="calendarfolderpermissionlevel"></a>CalendarFolderPermissionLevel

O elemento **CalendarFolderPermissionLevel** contém as permissões para a pasta de calendário padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<CalendarFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</CalendarFolderPermissionLevel>
```

 **DelegateFolderPermissionLevelType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |Contém as configurações de nível de permissão de representante para um usuário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores de texto que representam os níveis de permissão.
  
**Valores de texto do nível de permissão**

|**Nível de permissão**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |O usuário delegado não tem permissões de acesso à pasta calendário.  <br/> |
|Revisor  <br/> |O usuário delegado pode ler itens na pasta calendário.  <br/> |
|Autor  <br/> |O usuário delegado pode ler e criar itens na pasta calendário.  <br/> |
|Editor  <br/> |O usuário delegado pode ler, criar e modificar itens na pasta calendário.  <br/> |
|Personalizado  <br/> |O usuário delegado tem permissões de acesso personalizadas para a pasta calendário.  <br/> |
   
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



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionar representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

