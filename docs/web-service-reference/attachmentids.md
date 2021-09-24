---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: O elemento AttachmentIds contém uma matriz de identificadores de anexo.
ms.openlocfilehash: a631edbd1b82f3bbf7b99014d623fbb0072bb0c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525131"
---
# <a name="attachmentids"></a>AttachmentIds

O **elemento AttachmentIds** contém uma matriz de identificadores de anexo. 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 **NonEmptyArrayOfRequestAttachmentIdsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentId (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) <br/> |O elemento que identifica um único anexo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[DeleteAttachment](deleteattachment.md) <br/> |O elemento que define uma solicitação para excluir um anexo do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/DeleteAttachment` <br/> |
|[GetAttachment](getattachment.md) <br/> |O elemento que define uma solicitação para obter um anexo do Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação DeleteAttachment](deleteattachment-operation.md)
- [Operação GetAttachment](getattachment-operation.md)

