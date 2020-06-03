---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: O elemento NormalizedBody especifica uma representação HTML da Propriedade Body de um item como um fragmento que pode ser inserido em outro corpo HTML.
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462665"
---
# <a name="normalizedbody"></a>NormalizedBody

O elemento **NormalizedBody** especifica uma representação HTML da propriedade **Body** de um item como um fragmento que pode ser inserido em outro corpo HTML. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|BodyType  <br/> |Indica o tipo de corpo. O valor de **texto** para o atributo **BodyType** indica que o corpo está no formato de texto sem formatação. O valor de **HTML** para o atributo **BodyType** indica que o corpo está no formato HTML. O atributo **BodyType** é necessário.  <br/> |
|Istruncado  <br/> |Indica que o conteúdo do corpo foi truncado. Um valor de texto **false** para o atributo **IsTruncated** indica que o conteúdo do corpo não foi truncado. O corpo normalizado será truncado se o tamanho do corpo normalizado for maior do que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tarefa](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **NormalizedBody** é o corpo normalizado do item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

