---
title: EditItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EditItems
api_type:
- schema
ms.assetid: 1cb14493-c999-4d66-b82c-ecb410dc1c00
description: O elemento EditItems indica quais itens em uma pasta um usuário tem permissão para editar. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 0c3800b4d242dccb7455e0d0dea74e766db22854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459248"
---
# <a name="edititems"></a>EditItems

O elemento **EditItems** indica quais itens em uma pasta um usuário tem permissão para editar. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<EditItems>None or Owned or All</EditItems>
```

 **PermissionActionType**
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
|[CalendarPermission](calendarpermission.md) <br/> |Define o acesso que um usuário tem a uma pasta de calendário. Este elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **EditItems** . 
  
**Valores de texto do elemento EditItems**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o usuário não tem permissão para editar itens na pasta.  <br/> |
|Possuir  <br/> |Indica que o usuário tem permissão para editar os itens que o usuário possui na pasta.  <br/> |
|Todos  <br/> |Indica que o usuário tem permissão para editar todos os itens na pasta.  <br/> |
   
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
- [Definindo permissões no nível de pasta](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

