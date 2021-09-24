---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: O elemento NormalizedBody especifica uma representação HTML da propriedade Body de um item como um fragmento que pode ser inserido em outro corpo HTML.
ms.openlocfilehash: 9ce7a745cfbe2e08afbe4c83873cb670b6afa571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515429"
---
# <a name="normalizedbody"></a>NormalizedBody

O **elemento NormalizedBody** especifica uma representação HTML da propriedade **Body** de um item como um fragmento que pode ser inserido em outro corpo HTML. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|BodyType  <br/> |Indica o tipo de corpo. O valor de **Texto** para o **atributo BodyType** indica que o corpo está em forma de texto sem texto. O valor de **HTML** para o **atributo BodyType** indica que o corpo está em formato HTML. O **atributo BodyType** é obrigatório.  <br/> |
|IsTruncated  <br/> |Indica que o conteúdo do corpo foi truncado. Um valor de texto **false** para o **atributo IsTruncated** indica que o conteúdo do corpo não foi truncado. O corpo normalizado será truncado se o comprimento do corpo normalizado for maior do que o valor definido no [elemento MaximumBodySize.](maximumbodysize.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tarefa](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento NormalizedBody** é o corpo normalizado do item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

