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
description: O elemento ContactsFolderPermissionLevel contém as permissões para a pasta de contatos padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 8d76e00ab63714e220bd3205b10c8b72d15a4788
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527121"
---
# <a name="contactsfolderpermissionlevel"></a>ContactsFolderPermissionLevel

O elemento **ContactsFolderPermissionLevel** contém as permissões para a pasta de contatos padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ContactsFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</ContactsFolderPermissionLevel>
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
|Nenhum  <br/> |O usuário delegado não tem permissões de acesso à pasta contatos.  <br/> |
|Revisor  <br/> |O usuário delegado pode ler itens na pasta contatos.  <br/> |
|Autor  <br/> |O usuário delegado pode ler e criar itens na pasta contatos.  <br/> |
|Editor  <br/> |O usuário delegado pode ler, criar e modificar itens na pasta contatos.  <br/> |
|Personalizado  <br/> |O usuário delegado tem permissões de acesso personalizadas à pasta contatos.  <br/> |
   
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

