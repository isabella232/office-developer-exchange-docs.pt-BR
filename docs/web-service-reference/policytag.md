---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: O elemento PolicyTag especifica o identificador de retenção em um item ou pasta.
ms.openlocfilehash: 16759748dded6978e68450a6b8d504dd378c04be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519251"
---
# <a name="policytag"></a>PolicyTag

O **elemento PolicyTag** especifica o identificador de retenção em um item ou pasta. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|IsExplicit  <br/> |Indica se uma marca de política foi definida explicitamente em um item ou pasta.  <br/> Um valor de texto **true** para o **atributo IsExplicit** indica que a marca de política foi definida explicitamente no item ou pasta. Um valor de texto **false** indica que a marca de política foi definida implicitamente no item ou pasta com base na marca de política de pasta pai.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SearchPreviewItem](searchpreviewitem.md)  |  [Item](item.md)  |  [Contato](contact.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento PolicyTag** é o identificador de marca de política. O identificador de marca de política é um GUID. 
  
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
   

