---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: O elemento NewBodyContent representa o novo conteúdo do corpo de uma mensagem.
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466854"
---
# <a name="newbodycontent"></a>NewBodyContent

O elemento **NewBodyContent** representa o novo conteúdo do corpo de uma mensagem. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**BodyType** <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
   
#### <a name="bodytype-attribute"></a>Atributo BodyType

|**Valor**|**Descrição**|
|:-----|:-----|
|**HTML** <br/> |Converte todos os corpos em HTML.  <br/> |
|**Text** <br/> |Converte todos os corpos em texto sem formatação.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta para o remetente de um item no repositório do Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta para o remetente e todos os destinatários identificados de um item no repositório do Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um item de repositório do Exchange para encaminhar aos destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto Response que é usado para cancelar uma reunião.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contém uma resposta a um item de postagem. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o novo conteúdo do corpo de uma mensagem.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

