---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: O elemento GetAttachment é o elemento raiz em uma solicitação para obter um anexo do Exchange store.
ms.openlocfilehash: 057b42e78845f583cf1e52804e0108f335ef951c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546368"
---
# <a name="getattachment"></a>GetAttachment

O **elemento GetAttachment** é o elemento raiz em uma solicitação para obter um anexo do Exchange store. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Identifica propriedades de item estendidas adicionais para retornar em uma resposta a uma [solicitação GetAttachment.](getattachment.md) Esse elemento é opcional.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contém uma matriz de identificadores de anexo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O [elemento AttachmentShape](attachmentshape.md) não é necessário para identificar as propriedades retornadas na resposta. A [operação GetAttachment](getattachment-operation.md) retorna as propriedades Name, ContentType, ContentId, ContentLocation e Content para anexos de arquivo. Para anexos de item, as propriedades retornadas são Name, ContentType, ContentId, ContentLocation e todas as propriedades do item anexado. Isso equivale a usar a forma base AllProperties em uma [solicitação GetItem.](getitem.md) 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

