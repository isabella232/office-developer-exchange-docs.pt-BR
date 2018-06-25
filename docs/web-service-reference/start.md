---
title: Início
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: O elemento iniciar representa o início de uma duração.
ms.openlocfilehash: 8d013990e650b497abfa947938a69eed3fed7474
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825545"
---
# <a name="start"></a>Início

O elemento **Iniciar** representa o início de uma duração. 
  
```xml
<Start/>
```

**DateTime**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Representa uma ocorrência excluída de um item de calendário recorrente.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência de modificação de um item de calendário recorrente.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o início de uma duração.
  
## <a name="remarks"></a>Comentários

A operação UpdateItem pode definir a hora de [início](start.md) e [término](end-ex15websvcsotherref.md) de um item de armazenamento do Exchange. Em uma solicitação de UpdateItem, a hora de **início** pode ser definida sem também definir a hora de **término** . Isso pode causar um erro se a hora de **início** é posterior à hora de **término** . Lembre-se de que os aplicativos cliente devem executar ajustes à hora de **término** quando a hora de **início** for alterada para preservar a duração. 
  
> [!NOTE]
> As informações de deslocamento do fuso horário serão perdidas se as datas de [início](start.md) e [término](end-ex15websvcsotherref.md) do item mestre recorrente não tiver uma data que é igual a primeira ocorrência de um padrão de recorrência semanal. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

