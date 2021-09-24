---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: O elemento NewBodyContent representa o novo conteúdo de corpo de uma mensagem.
ms.openlocfilehash: 48f6a12e0492249d239196ca3be19857e34e0099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509508"
---
# <a name="newbodycontent"></a>NewBodyContent

O **elemento NewBodyContent** representa o novo conteúdo de corpo de uma mensagem. 
  
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
|**Texto** <br/> |Converte todos os corpos em texto sem texto.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ReplyToItem](replytoitem.md) <br/> |Contém uma resposta ao remetente de um item no Exchange store.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contém uma resposta ao remetente e a todos os destinatários identificados de um item no Exchange store.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contém um Exchange de armazenamento para encaminhar aos destinatários.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Representa o objeto de resposta usado para cancelar uma reunião.  <br/> |
|[PostReplyItem](postreplyitem.md) <br/> |Contém uma resposta a um item de postagem. Esse elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa o novo conteúdo de corpo de uma mensagem.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

