---
title: Norte
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
description: O elemento Daylight representa a data e hora em que o horário se altera do horário padrão para o horário de verão.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457456"
---
# <a name="daylight"></a>Norte

O elemento **Daylight** representa a data e hora em que o horário se altera do horário padrão para o horário de verão. 
  
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

**Timechangtype**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**TimeZoneName** <br/> |Descreve o nome do fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Offset](offset.md) <br/> |Descreve o deslocamento do [BaseOffset](baseoffset.md). O deslocamento base além desse deslocamento identifica o tempo de acordo com o horário padrão ou de verão.  <br/> |
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |Descreve um padrão relativo de recorrência anual para um padrão de data de transição de fuso horário.  <br/> |
|[AbsoluteDate](absolutedate.md) <br/> |Representa a data em que o horário muda de horário padrão ou de horário de verão.  <br/> |
|[Tempo (timechangtype)](time-timechangetype.md) <br/> |Descreve o momento em que a hora é alterada entre o horário padrão e o horário de verão.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MeetingTimeZone](meetingtimezone.md) <br/> |Representa o fuso horário do local onde a reunião está hospedada.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

