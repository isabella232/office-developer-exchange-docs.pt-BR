---
title: NotesFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotesFolderPermissionLevel
api_type:
- schema
ms.assetid: 76a2520c-f453-4fd7-b3eb-1c5f4666680a
description: O elemento NotesFolderPermissionLevel contém as permissões para a pasta de anotações padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: dd8644210692e0c342079d055ddf00b8d9283d7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824552"
---
# <a name="notesfolderpermissionlevel"></a>NotesFolderPermissionLevel

O elemento **NotesFolderPermissionLevel** contém as permissões para a pasta de anotações padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<NotesFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</NotesFolderPermissionLevel>
```

 **DelegateFolderPermissionLevelType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |Contém as configurações de nível de permissão do representante de um usuário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores de texto que representam os níveis de permissão.
  
**Valores de texto de nível de permissão**

|**Nível de permissão**|**Descrição**|
|:-----|:-----|
|None  <br/> |O usuário delegado não tem nenhuma permissão de acesso para a pasta anotações.  <br/> |
|Reviewer  <br/> |O usuário delegado pode ler itens na pasta anotações.  <br/> |
|Autor  <br/> |O usuário delegado pode ler e criar itens na pasta anotações.  <br/> |
|Editor  <br/> |O usuário delegado pode ler, criar e modificar itens na pasta anotações.  <br/> |
|Personalizado  <br/> |O usuário delegado tem permissões de acesso personalizada para a pasta anotações.  <br/> |
   
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



[Operação AddDelegate](adddelegate-operation.md)
  
[Operação UpdateDelegate](updatedelegate-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Adicionando representantes](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

