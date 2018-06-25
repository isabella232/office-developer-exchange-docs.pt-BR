---
title: Corpo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: O elemento Body Especifica o corpo de um item.
ms.openlocfilehash: a4803c0e5ac3b027396983a5524241590eac35f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751293"
---
# <a name="body"></a>Body

O elemento **Body** Especifica o corpo de um item. 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|BodyType  <br/> |Especifica o tipo do corpo.  <br/> |
|IsTruncated  <br/> |Valor Boolean que indica se o corpo será truncado.  <br/> |
   
#### <a name="bodytype"></a>BodyType

|**Valor**|**Descrição**|
|:-----|:-----|
|HTML  <br/> |Indica que o corpo é em HTML.  <br/> |
|Texto  <br/> |Indica que o corpo é no texto.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato no armazenamento do Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[1.1](item.md) <br/> |Representa um item genérico no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Representa um item de postagem no armazenamento do Exchange.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

O valor do elemento de **corpo** de texto é o conteúdo do corpo do item. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

