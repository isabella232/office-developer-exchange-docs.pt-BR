---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: O elemento MimeContentUTF8 contém o fluxo MIME UTF-8 de um objeto representado no formato base64Binary e dá suporte à internacionalização de endereços de email e [RFC6530].
ms.openlocfilehash: f0ab38368d3a18be38f63c86183a238e2fd0a474
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540752"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

O **elemento MimeContentUTF8** contém o fluxo MIME UTF-8 de um objeto representado no formato base64Binary e dá suporte à internacionalização de endereços de email e [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Um valor de texto que representa um fluxo MIME base64binary é necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O conteúdo da mensagem passa pelos três níveis de codificação a seguir antes de ser armazenado no **valor MimeContentUTF8:** 
  
1. Texto da mensagem — Essa é a codificação do corpo, como iso-2022-jp para caracteres japoneses.
    
2. Fluxo MIME — Esta é a codificação UTF8 do texto da mensagem para o **elemento MimeContentUTF8** ou a codificação ASCII do texto da mensagem para o [elemento MimeContent.](mimecontent.md) 
    
3. Documento XML — Esse é sempre o fluxo ASCII codificado com base64 do fluxo MIME, onde caracteres como ' ', que são significativos para XML, são ocultos dos \< analisadores XML.
    
Cada nível é independente do nível que o precede.
  
O **elemento MimeContentUTF8** pode conter os mesmos dados que outras propriedades retornadas com um item. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
### <a name="version-differences"></a>Diferenças de versão

Esse elemento está disponível em versões do Exchange começando com a com build 15.00.0986.00.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

