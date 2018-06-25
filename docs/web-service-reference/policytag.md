---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: O elemento PolicyTag Especifica o identificador de retenção em um item ou pasta.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824835"
---
# <a name="policytag"></a>PolicyTag

O elemento **PolicyTag** Especifica o identificador de retenção em um item ou pasta. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|IsExplicit  <br/> |Indica se uma marca de política foi explicitamente definida em um item ou pasta.  <br/> Um valor de texto de **true** para o atributo **IsExplicit** indica que a marca da diretiva foi explicitamente definida no item ou na pasta. Um valor de texto de **false** indica que a marca da diretiva implicitamente foi definida no item ou na pasta com base na marca de política de pasta pai.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [contato](contact.md) | [mensagem](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tarefa](task.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **PolicyTag** é o identificador de marca de política. O identificador de marca de política é um GUID. 
  
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
   

