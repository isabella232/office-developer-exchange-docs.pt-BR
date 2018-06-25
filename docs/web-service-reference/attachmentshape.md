---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: O elemento AttachmentShape identifica propriedades adicionais para retornar em resposta a uma solicitação de GetAttachment.
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751223"
---
# <a name="attachmentshape"></a>AttachmentShape

O elemento **AttachmentShape** identifica propriedades adicionais para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) . 
  
- [GetAttachment](getattachment.md)
  
- [AttachmentShape](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 **AttachmentResponseShapeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo de email extensões MIME (Multipurpose Internet) de um item ou de um anexo é retornado na resposta. Esse elemento é opcional.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o corpo de texto é formatado na resposta. Esse elemento é opcional.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se o conteúdo potencialmente não seguro de HTML é filtrado de um anexo. Esse elemento é opcional.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica as propriedades adicionais para retornar em uma resposta. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |O elemento que define uma solicitação para fazer um anexo a partir de uma caixa de correio no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação GetAttachment](getattachment-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

