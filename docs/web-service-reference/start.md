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
description: O elemento Start representa o início de uma duração.
ms.openlocfilehash: 0daf9c1422f7ba3894f9785aacac58263c5e721e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457211"
---
# <a name="start"></a>Início

O elemento **Start** representa o início de uma duração. 
  
```xml
<Start/>
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
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Representa uma ocorrência excluída de um item de calendário recorrente.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência modificada de um item de calendário recorrente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o início de uma duração.
  
## <a name="remarks"></a>Comentários

A operação UpdateItem pode definir a hora de [início](start.md) e de [término](end-ex15websvcsotherref.md) de um item do repositório do Exchange. Em uma solicitação UpdateItem, a hora de **início** pode ser definida sem definir também a hora de **término** . Isso pode causar um erro se a hora de **início** for posterior à hora de **término** . Lembre-se de que os aplicativos cliente devem realizar ajustes na hora de **término** quando essa hora de **início** é alterada para preservar a duração. 
  
> [!NOTE]
> As informações de deslocamento de fuso horário serão perdidas se as datas de [início](start.md) e [término](end-ex15websvcsotherref.md) do item mestre recorrente não tiverem uma data igual à primeira ocorrência de um padrão de recorrência semanal. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

