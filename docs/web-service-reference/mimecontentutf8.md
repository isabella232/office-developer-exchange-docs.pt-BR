---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: O elemento MimeContentUTF8 contém o fluxo de MIME de codificação UTF-8 de um objeto que é representado no formato base64Binary e suporta internacionalização de endereço de email e [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824466"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

O elemento **MimeContentUTF8** contém o fluxo de MIME de codificação UTF-8 de um objeto que é representado no formato base64Binary e suporta internacionalização de endereço de email e [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
```XML
<MimeContentUTF8 CharacterSet="" />
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

Se este elemento for usado, será necessário um valor de texto que representa um fluxo MIME base64binary.
  
## <a name="remarks"></a>Coment�rios

O conteúdo da mensagem passa três níveis de codificação antes de ser armazenado no valor de **MimeContentUTF8** a seguir: 
  
1. Texto da mensagem — este é o corpo de codificação, como iso-2022-jp para caracteres japonês.
    
2. Fluxo de MIME — isto é a codificação UTF8 do texto da mensagem para o elemento **MimeContentUTF8** ou a codificação ASCII do texto da mensagem para o elemento [MimeContent](mimecontent.md) . 
    
3. Documento XML — será sempre o fluxo de ASCII codificado na base64 do fluxo de MIME, onde caracteres como '\<', que sejam significativas XML, estão ocultos analisadores XML.
    
Cada nível é independente do nível que precede a ele.
  
O elemento **MimeContentUTF8** deve conter os mesmos dados que contêm outras propriedades que são retornadas com um item. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
### <a name="version-differences"></a>Diferenças de versão

Este elemento está disponível nas versões do Exchange, começando com compilação 15.00.0986.00.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

