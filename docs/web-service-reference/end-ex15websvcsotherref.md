---
title: Final
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: O elemento final representa o final de uma duração.
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456140"
---
# <a name="end"></a>Final

O elemento **final** representa o final de uma duração. 
  
```xml
<End/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência modificada de um item de calendário recorrente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o final de uma duração.
  
## <a name="remarks"></a>Comentários

A operação UpdateItem pode definir a hora de [início](start.md) e de **término** de um item do repositório do Exchange. Em uma solicitação UpdateItem, você pode definir a hora de [início](start.md) sem definir a hora de **término** . Isso pode causar um erro se a hora de [início](start.md) for posterior à hora de **término** . Lembre-se de que os aplicativos cliente devem realizar ajustes na hora de **término** em que a hora de [início](start.md) é alterada para preservar a duração. 
  
 **Observação** As informações de deslocamento de fuso horário serão perdidas se as datas de [início](start.md) e **término** do item mestre recorrente não tiverem uma data igual à primeira ocorrência de um padrão de recorrência semanal. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[WeeklyRecurrence](weeklyrecurrence.md)
  
 **End**


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

