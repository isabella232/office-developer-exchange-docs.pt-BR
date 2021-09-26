---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: O elemento TasksFolderPermissionLevel contém as permissões da pasta Tarefas padrão. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 991b13f9a9f95805b13312712b1f6c5941033c46
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543867"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

O **elemento TasksFolderPermissionLevel** contém as permissões da pasta Tarefas padrão. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
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
|[DelegatePermissions](delegatepermissions.md) <br/> |Contém as configurações de nível de permissão de representante para um usuário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores de texto que representam os níveis de permissão.
  
**Valores de texto de nível de permissão**

|**Nível de permissão**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |O usuário representante não tem permissões de acesso à pasta Tarefas.  <br/> |
|Revisor  <br/> |O usuário representante pode ler itens na pasta Tarefas.  <br/> |
|Autor  <br/> |O usuário representante pode ler e criar itens na pasta Tarefas.  <br/> |
|Editor  <br/> |O usuário representante pode ler, criar e modificar itens na pasta Tarefas.  <br/> |
|Personalizado  <br/> |O usuário representante tem permissões de acesso personalizadas para a pasta Tarefas.  <br/> |
   
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

- [Operação AddDelegate](adddelegate-operation.md)
- [Operação UpdateDelegate](updatedelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionando representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

