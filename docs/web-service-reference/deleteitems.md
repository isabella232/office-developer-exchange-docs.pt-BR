---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: O elemento DeleteItems indica quais itens em uma pasta um usuário tem permissão para excluir. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d41e44c3cc0996ab5933eafaf1087cf30d7944a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546669"
---
# <a name="deleteitems"></a>DeleteItems

O **elemento DeleteItems** indica quais itens em uma pasta um usuário tem permissão para excluir. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
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
|[Permissão](permission.md) <br/> |Define o acesso que um usuário tem a uma pasta. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Define o acesso que um usuário tem a uma pasta Calendário. Esse elemento foi introduzido no Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento DeleteItems.** 
  
**Valores de texto do elemento DeleteItems**

|**Valor**|**Descrição**|
|:-----|:-----|
|Nenhum  <br/> |Indica que o usuário não tem permissão para excluir itens na pasta.  <br/> |
|Owned  <br/> |Indica que o usuário tem permissão para excluir os itens que o usuário possui na pasta.  <br/> |
|Todos  <br/> |Indica que o usuário tem permissão para excluir todos os itens na pasta.  <br/> |
   
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
- [Definindo Folder-Level Permissões](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

