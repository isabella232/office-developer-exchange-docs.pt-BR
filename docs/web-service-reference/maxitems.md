---
title: MaxItems
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4ddba6b8-0f38-42cd-96a1-0d4283f6375b
description: O elemento MaxItems especifica o número máximo de itens a retornar na solicitação.
ms.openlocfilehash: 23a78db874ef3678be8c6703fb7004fc5f8a1425
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511111"
---
# <a name="maxitems"></a>MaxItems

O **elemento MaxItems** especifica o número máximo de itens a retornar na solicitação. 
  
```XML
<MaxItems/>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento MaxItems** é o número máximo de itens a retornar na solicitação. Esse número não pode ser menor que zero ou maior do que 200. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[GetReminders](getreminders.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

