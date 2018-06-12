---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: O elemento TextBody Especifica o corpo de texto.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837712"
---
# <a name="textbody"></a>TextBody

O elemento **TextBody** Especifica o corpo de texto. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|BodyTypeType  <br/> |Indica o tipo de corpo. O valor de **texto** para o atributo **BodyTypeType** indica que o corpo está no formato de texto sem formatação. O valor de **HTML** para o atributo **BodyTypeType** indica que o corpo está no formato HTML. O atributo **BodyTypeType** é necessário.  <br/> |
|IsTruncated  <br/> |Indica que o conteúdo do corpo ter sido truncado. Um valor de texto de **false** para o atributo **IsTruncated** indica que o corpo de conteúdo não foi truncado. O corpo normalizado será truncado se o comprimento do corpo de texto for maior que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Item](item.md) | [contato](contact.md) | [mensagem](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tarefa](task.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **TextBody** é o corpo de texto do item. 
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

