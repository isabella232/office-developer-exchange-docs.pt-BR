---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: O elemento ReminderItemAction Especifica a ação para um item de lembrete.
ms.openlocfilehash: f44e8d354aedca2c1f950238d87ab5c2d6387954
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825069"
---
# <a name="reminderitemaction"></a>ReminderItemAction

O elemento **ReminderItemAction** Especifica a ação para um item de lembrete. 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 **ReminderItemActionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

[ActionType (ReminderActionType)](actiontype-reminderactiontype.md) | [ItemId](itemid.md) | [NewReminderTime](newremindertime.md)
  
### <a name="parent-elements"></a>Elementos pai

[ReminderItemActions](reminderitemactions.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[ReminderItemActions](reminderitemactions.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

