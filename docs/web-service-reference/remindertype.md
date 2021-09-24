---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: O elemento ReminderType especifica o tipo de lembrete a ser retornado.
ms.openlocfilehash: ab10db372efb935b335868f5d212ded84b29e6eb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517998"
---
# <a name="remindertype"></a>ReminderType

O **elemento ReminderType** especifica o tipo de lembrete a ser retornado. 
  
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

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento ReminderType** é o tipo de lembretes a ser retornado, **All**, **Current** ou **Old**. **Tudo** é o valor recomendado para esse elemento. Para obter mais informações sobre a relação entre o **elemento ReminderType** e os elementos [BeginTime](begintime.md) e [EndTime,](endtime-remindermessagedatatype.md) consulte [GetReminders operation](getreminders-operation.md).
  
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

