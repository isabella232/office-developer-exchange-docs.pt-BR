---
title: ContactsFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolderPermissionLevel
api_type:
- schema
ms.assetid: 805f05e7-b320-436a-9965-ba1ee235ac41
description: O elemento ContactsFolderPermissionLevel contém as permissões para a pasta padrão Contatos. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 4b6a109c3a38a20dc5d6f611607b16ada0e4e46b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751452"
---
# <a name="contactsfolderpermissionlevel"></a>ContactsFolderPermissionLevel

O elemento **ContactsFolderPermissionLevel** contém as permissões para a pasta padrão Contatos. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ContactsFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</ContactsFolderPermissionLevel>
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
|None  <br/> |O usuário delegado não tem nenhuma permissão de acesso à pasta Contatos.  <br/> |
|Reviewer  <br/> |O usuário delegado pode ler itens na pasta Contatos.  <br/> |
|Autor  <br/> |O usuário delegado pode ler e criar itens na pasta Contatos.  <br/> |
|Editor  <br/> |O usuário delegado pode ler, criar e modificar itens na pasta Contatos.  <br/> |
|Personalizado  <br/> |O usuário delegado tem permissões de acesso personalizada para a pasta Contatos.  <br/> |
   
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

