---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: O elemento NormalizedBody Especifica uma representação de HTML da propriedade corpo de um item como um fragmento que pode ser inserido em outro corpo em HTML.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824548"
---
# <a name="normalizedbody"></a>NormalizedBody

O elemento **NormalizedBody** Especifica uma representação de HTML da propriedade **corpo** de um item como um fragmento que pode ser inserido em outro corpo em HTML. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|BodyType  <br/> |Indica o tipo de corpo. O valor de **texto** para o atributo **BodyType** indica que o corpo está no formato de texto sem formatação. O valor de **HTML** para o atributo **BodyType** indica que o corpo está no formato HTML. O atributo **BodyType** é necessário.  <br/> |
|IsTruncated  <br/> |Indica que o conteúdo do corpo ter sido truncado. Um valor de texto de **false** para o atributo **IsTruncated** indica que o corpo de conteúdo não foi truncado. O corpo normalizado será truncado se o comprimento do corpo normalizado for maior que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md) | [mensagem](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [tarefa](task.md) | [PostItem ](postitem.md)  |  [CalendarItem](calendaritem.md) | [contato](contact.md) | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **NormalizedBody** é normalizado corpo do item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

