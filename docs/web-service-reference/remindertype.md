---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: O elemento ReminderType Especifica o tipo de lembretes para retornar.
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825077"
---
# <a name="remindertype"></a>ReminderType

O elemento **ReminderType** Especifica o tipo de lembretes para retornar. 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **ReminderType** é o tipo de lembretes a serem retornadas, **tudo**, **atual**ou **antigo**. **All** é o valor recomendado para esse elemento. Para obter mais informações sobre a relação entre o elemento **ReminderType** e os elementos [BeginTime](begintime.md) e [EndTime](endtime-remindermessagedatatype.md) , consulte [GetReminders operação](getreminders-operation.md).
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[GetReminders](getreminders.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

