---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: O elemento GetAttachment é o elemento raiz em uma solicitação para obter um anexo do repositório do Exchange.
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463976"
---
# <a name="getattachment"></a>GetAttachment

O elemento **GetAttachment** é o elemento raiz em uma solicitação para obter um anexo do repositório do Exchange. 
  
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
|[AttachmentShape](attachmentshape.md) <br/> |Identifica Propriedades de item estendido adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) . Este elemento é opcional.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contém uma matriz de identificadores de anexo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O elemento [AttachmentShape](attachmentshape.md) não é necessário para identificar as propriedades retornadas na resposta. A [operação GetAttachment](getattachment-operation.md) retorna o nome, ContentType, ContentId, ContentLocation e as propriedades de conteúdo para anexos de arquivo. Para anexos de item, as propriedades retornadas são o nome, ContentType, ContentId, ContentLocation e todas as propriedades do item anexado. Isso equivale a usar a forma base de propriedades em uma solicitação [GetItem](getitem.md) . 
  
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

