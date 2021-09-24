---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: O elemento DelegateUsers contém as identidades dos representantes para adicionar ou atualizar em uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7eae154297eb385903c57cbd8fe9b3feeb96c816
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540206"
---
# <a name="delegateusers"></a>DelegateUsers

O **elemento DelegateUsers** contém as identidades dos representantes para adicionar ou atualizar em uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

**ArrayOfDelegateUserType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifica um único representante para adicionar ou atualizar em uma caixa de correio.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Define uma solicitação para adicionar representantes a uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Define uma solicitação para atualizar representantes em uma caixa de correio. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação AddDelegate](adddelegate-operation.md) 
- [Operação UpdateDelegate](updatedelegate-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
- [Adicionando representantes](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

