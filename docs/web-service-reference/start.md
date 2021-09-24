---
title: Início
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Start
api_type:
- schema
ms.assetid: 7cfe9979-c893-4f9b-b3a1-8f9e17515a4b
description: O elemento Start representa o início de uma duração.
ms.openlocfilehash: 7342e285e57a165ec4a9ba0b8551bfbe045d3b9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521267"
---
# <a name="start"></a>Início

O **elemento Start** representa o início de uma duração. 
  
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
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[DeletedOccurrence](deletedoccurrence.md) <br/> |Representa uma ocorrência excluída de um item de calendário recorrente.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|[Occurrence](occurrence.md) <br/> |Representa uma única ocorrência modificada de um item de calendário recorrente.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa o início de uma duração.
  
## <a name="remarks"></a>Comentários

A operação UpdateItem pode definir a hora [de início](start.md) [e](end-ex15websvcsotherref.md) término de um Exchange de armazenamento. Em uma solicitação UpdateItem, a hora **de** início pode ser definida sem também definir a **hora de** término. Isso pode causar um erro se a hora **de** início for posterior à **hora de** Término. Esteja ciente de que os aplicativos cliente devem realizar ajustes na hora **de** término quando esse horário **de** início for alterado para preservar a duração. 
  
> [!NOTE]
> As informações de deslocamento do [](start.md) fuso [](end-ex15websvcsotherref.md) horário são perdidas se as datas inicial e final do item mestre recorrente não têm uma data igual à primeira ocorrência de um padrão de recorrência semanal. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [WeeklyRecurrence](weeklyrecurrence.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

