---
title: Horário de verão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: O elemento de verão representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.
ms.openlocfilehash: cdb6ed305f1d77a73b952f8c659991f3b2a8df7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751699"
---
# <a name="daylight"></a>Horário de verão

O elemento de **verão** representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão. 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

**TimeChangeType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**TimeZoneName** <br/> |Descreve o nome do fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Offset](offset.md) <br/> |Descreve o deslocamento, desde o [BaseOffset](baseoffset.md). Base de deslocamento além este deslocamento identifica a hora de acordo com se ele está standard ou o horário de verão.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão de recorrência anual relativa para um padrão de data de transição do fuso horário.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Representa a data quando o tempo é alterado de standard ou o horário de verão.  <br/> |
|[Tempo (TimeChangeType)](time-timechangetype.md) <br/> |Descreve o tempo quando o tempo é alterado entre o período padrão e o horário de verão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Representa o fuso horário do local onde a reunião está hospedada.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

