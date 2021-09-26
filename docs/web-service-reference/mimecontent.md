---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: O elemento MimeContent contém o fluxo MIME ASCII de um objeto representado no formato base64Binary e dá suporte a [RFC2045].
ms.openlocfilehash: 43040f241008010620ff4f1018cc5410a7a00e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542068"
---
# <a name="mimecontent"></a>MimeContent

O **elemento MimeContent** contém o fluxo MIME ASCII de um objeto representado no formato base64Binary e dá suporte [a [RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).
  
```xml
<MimeContent CharacterSet="" />
```

 **MimeContentType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**CharacterSet** <br/> |Se definido, o valor desse atributo será ignorado pelo servidor.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)  |  [Item](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tarefa](task.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um fluxo MIME base64Binary é necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O conteúdo da mensagem passa pelos três níveis de codificação a seguir antes de ser armazenado no **valor MimeContent:** 
  
1. Texto da mensagem — Essa é a codificação do corpo, como iso-2022-jp para caracteres japoneses.
    
2. Fluxo MIME — Esta é a codificação ASCII do texto da mensagem para o **elemento MimeContent** ou a codificação UTF8 do texto da mensagem para o [elemento MimeContentUTF8.](mimecontentutf8.md) 
    
3. Documento XML — Esse é sempre o fluxo ASCII codificado com base64 do fluxo MIME, onde caracteres como ' ', que são significativos para XML, são ocultos dos \< analisadores XML.
    
Cada nível é independente do nível que o precede.
  
O **elemento MimeContent** pode conter os mesmos dados que outras propriedades retornadas com um item. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

