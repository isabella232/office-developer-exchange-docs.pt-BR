---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: O elemento PermissionLevel representa o nível de permissão que um usuário tem em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458037"
---
# <a name="permissionlevel"></a>PermissionLevel

O elemento **PermissionLevel** representa o nível de permissão que um usuário tem em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Permissão](permission.md) <br/> |Define o acesso que um usuário tem a uma pasta. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **PermissionLevel** . 
  
**Valores de texto do elemento PermissionLevel**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o usuário não tem permissões na pasta.  <br/> |
|Proprietário  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas. O usuário é o proprietário da pasta e o contato da pasta.  <br/> |
|Publishingeditorcreateitems  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas.  <br/> |
|Editor  <br/> |Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta.  <br/> |
|Publishingauthorcreateitems  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta, editar e excluir somente os itens que o usuário cria e criar subpastas.  <br/> |
|Autor  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta e editar e excluir somente os itens que o usuário cria.  <br/> |
|Noneditingauthorcreateitems  <br/> |Indica que o usuário pode criar e ler todos os itens na pasta e excluir apenas os itens que o usuário cria.  <br/> |
|Revisor  <br/> |Indica que o usuário pode ler todos os itens na pasta.  <br/> |
|Colaborador  <br/> |Indica que o usuário pode criar itens na pasta. O conteúdo da pasta não é exibido.  <br/> |
|Personalizado  <br/> |Indica que o usuário tem permissões de acesso personalizadas na pasta.  <br/> |
   
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



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Definindo permissões no nível de pasta](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

