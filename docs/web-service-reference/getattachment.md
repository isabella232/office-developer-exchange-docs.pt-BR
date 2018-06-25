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
description: O elemento GetAttachment é o elemento raiz em uma solicitação para obter um anexo do armazenamento do Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752408"
---
# <a name="getattachment"></a>GetAttachment

O elemento **GetAttachment** é o elemento raiz em uma solicitação para obter um anexo do armazenamento do Exchange. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Identifica as propriedades de item estendido adicional para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) . Esse elemento é opcional.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contém uma matriz de identificadores de anexo.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O elemento [AttachmentShape](attachmentshape.md) não é necessário para identificar as propriedades retornadas na resposta. A [operação GetAttachment](getattachment-operation.md) retorna o nome, ContentType, ContentId, ContentLocation e as propriedades de conteúdo de anexos de arquivo. Anexos de item, as propriedades retornadas são o nome, ContentType, ContentId, ContentLocation e todas as anexado propriedades do item. Isso equivale a usar a forma de base AllProperties em uma solicitação de [GetItem](getitem.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

