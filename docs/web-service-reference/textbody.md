---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: O elemento TextBody especifica o corpo do texto.
ms.openlocfilehash: 5dfc0aa76f0b0778d785e46fe12259c4a226b89f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515177"
---
# <a name="textbody"></a>TextBody

O **elemento TextBody** especifica o corpo do texto. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|BodyTypeType  <br/> |Indica o tipo de corpo. O valor de **Text** para o **atributo BodyTypeType** indica que o corpo está em forma de texto sem texto. O valor de **HTML** para o **atributo BodyTypeType** indica que o corpo está em formato HTML. O **atributo BodyTypeType** é obrigatório.  <br/> |
|IsTruncated  <br/> |Indica que o conteúdo do corpo foi truncado. Um valor de texto **false** para o **atributo IsTruncated** indica que o conteúdo do corpo não foi truncado. O corpo normalizado será truncado se o comprimento do corpo do texto for maior do que o valor definido no [elemento MaximumBodySize.](maximumbodysize.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md)  |  [Contato](contact.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento TextBody** é o corpo do texto do item. 
  
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
   

