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
description: O elemento AttachmentShape identifica propriedades adicionais para retornar em uma resposta a uma solicitação GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529662"
---
# <a name="attachmentshape"></a>AttachmentShape

O elemento **AttachmentShape** identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) . 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta. Este elemento é opcional.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o corpo de texto é formatado na resposta. Este elemento é opcional.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se o conteúdo HTML potencialmente não seguro é filtrado de um anexo. Este elemento é opcional.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais a serem retornadas em uma resposta. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |O elemento que define uma solicitação para obter um anexo de uma caixa de correio no repositório do Exchange.  <br/> A seguir está a expressão XPath para este elemento:  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação GetAttachment](getattachment-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

