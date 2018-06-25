---
title: Períodos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: O elemento de períodos representa uma matriz de períodos que definem o deslocamento de tempo em fases diferentes do fuso horário.
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824729"
---
# <a name="periods"></a>Períodos

O elemento de **períodos** representa uma matriz de períodos que definem o deslocamento de tempo em fases diferentes do fuso horário. 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 **NonEmptyArrayOfPeriodsType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Period](period.md) <br/> |Define o nome, a diferença de horário e o identificador exclusivo de um estágio específico do fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Define o fuso horário para a hora de início de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Define o fuso horário para a hora de término de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).  <br/> |
|[Timezonedefinition pela última vez](timezonedefinition.md) <br/> |Define um fuso horário.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

