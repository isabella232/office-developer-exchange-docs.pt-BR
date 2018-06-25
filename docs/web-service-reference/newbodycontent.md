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
description: O elemento NewBodyContent representa o novo conteúdo de corpo de uma mensagem.
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824516"
---
# <a name="newbodycontent"></a>NewBodyContent

O elemento **NewBodyContent** representa o novo conteúdo de corpo de uma mensagem. 
  
```xml
<NewBodyContent BodyType=""/>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**BodyType** <br/> |Representa o conteúdo real do corpo de uma mensagem.  <br/> |
   
#### <a name="bodytype-attribute"></a>Atributo BodyType

|**Valor**|**Descrição**|
|:-----|:-----|
|**HTML** <br/> |Converte todos os corpos em HTML.  <br/> |
|**Text** <br/> |Converte todos os corpos de texto sem formatação.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta ao remetente de um item no armazenamento do Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta para o remetente e identificados todos os destinatários de um item no armazenamento do Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um item de armazenamento do Exchange para encaminhar para destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta é usado para cancelar uma reunião.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contém uma resposta para um item de postagem. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o novo conteúdo de corpo de uma mensagem.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do servidor do Exchange que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

