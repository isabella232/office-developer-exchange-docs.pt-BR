---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: O elemento AttachmentId identifica um item ou anexo de arquivo. Esse elemento é usado em respostas CreateAttachment.
ms.openlocfilehash: a6363fad4e7ef9f0c21377f2c1ea8c19c494cdef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522016"
---
# <a name="attachmentid"></a>AttachmentId

O **elemento AttachmentId** identifica um item ou anexo de arquivo. Esse elemento é usado em respostas CreateAttachment. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica o identificador exclusivo do anexo.  <br/> |
|**RootItemId** <br/> |Identifica o identificador exclusivo do item do armazenamento raiz ao qual o anexo está anexado.  <br/> |
|**RootItemChangeKey** <br/> |Identifica a chave de alteração do item do armazenamento raiz ao qual o anexo está anexado.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Representa um Exchange que está anexado a outro Exchange item.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Representa um arquivo anexado a um item no Exchange store.  <br/> |
   
## <a name="remarks"></a>Comentários

É importante observar que, quando um anexo é criado, a chave de alteração do item raiz é alterada.
  
O [elemento AttachmentId (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) é usado em solicitações DeleteAttachment e GetAttachment. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

