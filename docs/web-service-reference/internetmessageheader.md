---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: O elemento InternetMessageHeader representa o header de mensagem da Internet para um determinado header dentro da coleção de headers. Para obter toda a coleção de headers de mensagens da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre os headers de mensagens do EWS e da Internet, consulteGetting Internet message headers in EWS, MIME, and the missing Internet message headers.
ms.openlocfilehash: 4b3072611e8a3debf87ce2a023f4f68ee4487185
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541075"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

O **elemento InternetMessageHeader** representa o header de mensagem da Internet para um determinado header dentro da coleção de headers. Para obter toda a coleção de headers de mensagens da Internet, use **PR_TRANSPORT_MESSAGE_HEADERS** propriedade. Para obter mais informações sobre os headers de mensagens do EWS e da Internet, consulte "Obter os headers de mensagens da Internet no [EWS, no MIME](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)e nos headers de mensagem da Internet ausentes.
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**HeaderName** <br/> |Identifica o nome do header.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os headers de mensagens da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o valor do header.
  
## <a name="remarks"></a>Comentários

A seguir está a definição de propriedade estendida da API Gerenciada do EWS para a **propriedade PR_TRANSPORT_MESSAGE_HEADERS.** 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS, MIME e os headers de mensagens da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

