---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: O elemento MimeContentUTF8 contém o fluxo de MIME UTF-8 de um objeto que é representado no formato base64Binary e oferece suporte à internacionalização de endereços de email e [RFC6530].
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530426"
---
# <a name="mimecontentutf8"></a>MimeContentUTF8

O elemento **MimeContentUTF8** contém o fluxo de MIME UTF-8 de um objeto que é representado no formato base64Binary e oferece suporte à internacionalização de endereços de email e [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).
  
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

Um valor de texto que representa um fluxo MIME base64Binary será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

O conteúdo da mensagem passa pelos três níveis de codificação a seguir antes de ser armazenado no valor **MimeContentUTF8** : 
  
1. Texto da mensagem – esta é a codificação do corpo, como ISO-2022-JP para caracteres japoneses.
    
2. Fluxo MIME — essa é a codificação UTF8 do texto da mensagem para o elemento **MimeContentUTF8** ou a codificação ASCII do texto da mensagem para o elemento [MimeContent](mimecontent.md) . 
    
3. Documento XML — este é sempre o fluxo ASCII codificado em base64 do fluxo MIME, onde caracteres como ' \< ', que são significativos para XML, estão ocultos de analisadores XML.
    
Cada nível é independente do nível que o precede.
  
O elemento **MimeContentUTF8** pode conter os mesmos dados que outras propriedades retornadas com um item contêm. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
### <a name="version-differences"></a>Diferenças de versão

Este elemento está disponível em versões do Exchange a partir do Build 15.00.0986.00.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

