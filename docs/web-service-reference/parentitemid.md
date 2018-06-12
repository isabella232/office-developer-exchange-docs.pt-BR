---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: O elemento ParentItemId identifica o item pai que vincula a um anexo associado.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824703"
---
# <a name="parentitemid"></a>ParentItemId

O elemento **ParentItemId** identifica o item pai que vincula a um anexo associado. 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Identifica um único item no armazenamento do Exchange para associar um anexo. Esse valor é uma cadeia de caracteres. Este atributo é necessário.  <br/> |
|**ChangeKey** <br/> |Identifica uma versão não especificada de um item que é identificado pelo atributo **Id** no armazenamento do Exchange. Isso é usado para certificar-se de que um item atual é usado quando ela é atualizada com um anexo. Esse valor é uma cadeia de caracteres. Este atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Define uma solicitação para criar um anexo a um item em uma caixa de correio.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Coment�rios

Esse elemento é necessário na [operação CreateAttachment](createattachment-operation.md). Esse elemento é basicamente o mesmo que o elemento [ItemId](itemid.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação CreateAttachment](createattachment-operation.md)

