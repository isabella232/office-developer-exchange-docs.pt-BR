---
title: Padrão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: O elemento padrão representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.
ms.openlocfilehash: 1c9be4cf35773583078bc8e16ddf44433d3ad98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825536"
---
# <a name="standard"></a>Padrão

O elemento **padrão** representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão. 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
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
|[Offset](offset.md) <br/> |Descreve o deslocamento, desde o [BaseOffset](baseoffset.md). Em conjunto com o elemento **BaseOffset** , o elemento de **deslocamento** identifica se o tempo é a hora padrão ou o horário de verão.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão de recorrência anual relativa para uma data de transição do fuso horário.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Representa a data quando o tempo é alterado de hora padrão ou o horário de verão.  <br/> |
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

