---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: O elemento InternetMessageHeader representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre os cabeçalhos de mensagem EWS e Internet, Consulteobter cabeçalhos de mensagem da Internet no EWS, MIME e os cabeçalhos de mensagem da Internet ausentes.
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459304"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

O elemento **InternetMessageHeader** representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, consulte "obtendo cabeçalhos de mensagens da Internet em [EWS, MIME e cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**HeaderName** <br/> |Identifica o nome do cabeçalho.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Propriedadeinternetmessageheaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o valor do cabeçalho.
  
## <a name="remarks"></a>Comentários

A seguir está a definição da propriedade estendida da API gerenciada do EWS para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME e os cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

