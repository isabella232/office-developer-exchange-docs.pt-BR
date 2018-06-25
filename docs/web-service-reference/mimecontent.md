---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: O elemento MimeContent contém o fluxo de MIME ASCII de um objeto que é representado no formato base64Binary e suporta [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824465"
---
# <a name="mimecontent"></a>MimeContent

O elemento **MimeContent** contém o fluxo de MIME ASCII de um objeto que é representado no formato base64Binary e suporta [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**CharacterSet** <br/> |Se definido, o valor para este atributo é ignorado pelo servidor.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[CalendarItem](calendaritem.md) | [contato](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [mensagem](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tarefa](task.md)
  
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa um fluxo MIME base64Binary.
  
## <a name="remarks"></a>Comentários

O conteúdo da mensagem passa três níveis de codificação antes de ser armazenado no valor de **MimeContent** a seguir: 
  
1. Texto da mensagem — este é o corpo de codificação, como iso-2022-jp para caracteres japonês.
    
2. Fluxo de MIME — isto é a codificação ASCII do texto da mensagem para o elemento **MimeContent** ou a codificação UTF8 do texto da mensagem para o elemento [MimeContentUTF8](mimecontentutf8.md) . 
    
3. Documento XML — será sempre o fluxo de ASCII codificado na base64 do fluxo de MIME, onde caracteres como '\<', que sejam significativas XML, estão ocultos analisadores XML.
    
Cada nível é independente do nível que precede a ele.
  
O elemento **MimeContent** deve conter os mesmos dados que contêm outras propriedades que são retornadas com um item. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

