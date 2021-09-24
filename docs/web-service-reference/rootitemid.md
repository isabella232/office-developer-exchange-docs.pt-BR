---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: O elemento RootItemId identifica o item raiz de um anexo excluído.
ms.openlocfilehash: eab3cc30c2e3f2b6cdc443ba8eb7ae4bfa38d257
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509362"
---
# <a name="rootitemid"></a>RootItemId

O **elemento RootItemId** identifica o item raiz de um anexo excluído. 
  
[DeleteAttachmentResponse](deleteattachmentresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
  
[RootItemId](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **RootItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**RootItemId** <br/> |Identifica o item raiz de um anexo excluído.  <br/> |
|**RootItemChangeKey** <br/> |Identifica a nova chave de alteração do item raiz de um anexo excluído.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação DeleteAttachment.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento RootItemId** só é usado em respostas DeleteAttachment. Isso identifica o identificador de item raiz e, o mais importante, a nova chave de alteração para o item pai. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[DeleteAttachment](deleteattachment.md)
  
[Operação DeleteAttachment](deleteattachment-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

