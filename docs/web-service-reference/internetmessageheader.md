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
description: O elemento InternetMessageHeader representa o cabeçalho da mensagem para um determinado cabeçalho dentro da coleção de cabeçalhos da Internet. Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre os cabeçalhos de mensagem do EWS e a Internet, seeGetting cabeçalhos de mensagens da Internet no EWS, MIME e os cabeçalhos das mensagens de Internet ausentes.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823952"
---
# <a name="internetmessageheader"></a>InternetMessageHeader

O elemento **InternetMessageHeader** representa o cabeçalho da mensagem para um determinado cabeçalho dentro da coleção de cabeçalhos da Internet. Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . Para obter mais informações sobre cabeçalhos de mensagem do EWS e a Internet, consulte "Getting Internet cabeçalhos das mensagens no [EWS, MIME e os cabeçalhos das mensagens de Internet ausentes](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 **InternetHeaderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**HeaderName** <br/> |Identifica o nome de cabeçalho.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Representa a coleção de todos os cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o valor para o cabeçalho.
  
## <a name="remarks"></a>Coment�rios

Apresentamos a seguir o EWS Managed API estendido a definição de propriedade para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** . 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

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


[EWS, MIME e os cabeçalhos das mensagens de Internet ausentes](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

