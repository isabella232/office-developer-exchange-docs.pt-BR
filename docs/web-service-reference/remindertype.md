---
title: Remindertype
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: O elemento remindertype especifica o tipo de lembretes a ser retornado.
ms.openlocfilehash: 4ac20143bbfb29fb8f962515f2faba224b2f973f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465524"
---
# <a name="remindertype"></a>Remindertype

O elemento **Remindertype** especifica o tipo de lembretes a ser retornado. 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Getlembretes](getreminders.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Remindertype** é o tipo de lembretes a ser retornado, **tudo**, **atual**ou **antigo**. **All** é o valor recomendado para este elemento. Para obter mais informações sobre a relação entre o elemento **Remindertype** e os elementos [BeginTime](begintime.md) e [EndTime](endtime-remindermessagedatatype.md) , consulte [getlembrations Operation](getreminders-operation.md).
  
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



[Getlembretes](getreminders.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

