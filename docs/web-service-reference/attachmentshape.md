---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: O elemento AttachmentShape identifica propriedades adicionais para retornar em uma resposta a uma solicitação GetAttachment.
ms.openlocfilehash: 2c7ceb25f481ec07577117e46e26537e657e18c7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520035"
---
# <a name="attachmentshape"></a>AttachmentShape

O **elemento AttachmentShape** identifica propriedades adicionais para retornar em uma resposta a uma [solicitação GetAttachment.](getattachment.md) 
  
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
|[IncludeMimeContent](includemimecontent.md) <br/> |Especifica se o conteúdo MIME (Extensões de Email da Internet Multipropósitos) de um item ou anexo será retornado na resposta. Esse elemento é opcional.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifica como o texto do corpo é formatado na resposta. Esse elemento é opcional.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Especifica se o conteúdo HTML potencialmente não seguro é filtrado de um anexo. Esse elemento é opcional.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais para retornar em uma resposta. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |O elemento que define uma solicitação para obter um anexo de uma caixa de correio no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/GetAttachment` <br/> |
   
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

