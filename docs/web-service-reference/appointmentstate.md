---
title: Compromissostate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: O elemento Compromissostate especifica o status do compromisso.
ms.openlocfilehash: 8b0e827d02e9051f31d43199503dc286c50e2125
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463472"
---
# <a name="appointmentstate"></a>Compromissostate

O elemento **compromissostate** especifica o status do compromisso. 
  
```XML
<AppointmentState/>
```

 **int**
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
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Este elemento contém um valor de texto que representa os bits de conjunto. Isso está no formato de inteiro. Este elemento é somente leitura. Ele só será retornado em uma resposta.
  
## <a name="remarks"></a>Comentários

O valor inteiro retornado representa a bitmask do estado do compromisso. A tabela a seguir descreve cada bit.
  
|**Nome**|**Bits**|**Descrição**|
|:-----|:-----|:-----|
|Nenhum  <br/> |0x0000  <br/> |Nenhum sinalizador foi definido. Isso é usado apenas para um compromisso que não inclua participantes.  <br/> |
|Atenda  <br/> |0x0001  <br/> |Este compromisso é uma reunião.  <br/> |
|Received  <br/> |0x0002  <br/> |Este compromisso foi recebido.  <br/> |
|Foi  <br/> |0x0004  <br/> |Este compromisso foi cancelado.  <br/> |
   
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

