---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: O elemento TextBody especifica o corpo do texto.
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459480"
---
# <a name="textbody"></a>TextBody

O elemento **TextBody** especifica o corpo do texto. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|BodyTypeType  <br/> |Indica o tipo de corpo. O valor de **texto** para o atributo **BodyTypeType** indica que o corpo está no formato de texto sem formatação. O valor de **HTML** para o atributo **BodyTypeType** indica que o corpo está no formato HTML. O atributo **BodyTypeType** é obrigatório.  <br/> |
|Istruncado  <br/> |Indica que o conteúdo do corpo foi truncado. Um valor de texto **false** para o atributo **IsTruncated** indica que o conteúdo do corpo não foi truncado. O corpo normalizado será truncado se o comprimento do corpo do texto for maior do que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md)  |  [Contato](contact.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **TextBody** é o corpo do texto do item. 
  
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
   

