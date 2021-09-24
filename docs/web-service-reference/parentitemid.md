---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: O elemento ParentItemId identifica o item pai que se vincula a um anexo associado.
ms.openlocfilehash: d8072e86d8bd989d4baf6b0f29385dc955b83de8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515359"
---
# <a name="parentitemid"></a>ParentItemId

O **elemento ParentItemId** identifica o item pai que se vincula a um anexo associado. 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica um único item no Exchange para associar a um anexo. Esse valor é uma cadeia de caracteres. Esse atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão não especificada de um item identificado pelo **atributo Id** no Exchange store. Isso é usado para garantir que um item atual seja usado quando atualizado com um anexo. Esse valor é uma cadeia de caracteres. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Define uma solicitação para criar um anexo a um item em uma caixa de correio.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento é necessário na operação [CreateAttachment](createattachment-operation.md). Esse elemento é basicamente o mesmo que o [elemento ItemId.](itemid.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação CreateAttachment](createattachment-operation.md)

