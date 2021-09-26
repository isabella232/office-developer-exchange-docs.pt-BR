---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: O elemento AppointmentState especifica o status do compromisso.
ms.openlocfilehash: f984bbd5a1319a6051a3394ed04d56deabbb2c5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544278"
---
# <a name="appointmentstate"></a>AppointmentState

O **elemento AppointmentState** especifica o status do compromisso. 
  
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
|[CalendarItem](calendaritem.md) <br/> |Representa um Exchange de calendário.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma reunião no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Esse elemento contém um valor de texto que representa bits definidos. Isso está em formato inteiro. Esse elemento é somente leitura. Ele só será retornado em uma resposta.
  
## <a name="remarks"></a>Comentários

O valor inteiro retornado representa a máscara de bits de estado do compromisso. A tabela a seguir descreve cada bit.
  
|**Nome**|**Bit**|**Descrição**|
|:-----|:-----|:-----|
|Nenhum  <br/> |0x0000  <br/> |Nenhum sinalizador foi definido. Isso é usado apenas para um compromisso que não inclui participantes.  <br/> |
|Reunião  <br/> |0x0001  <br/> |Esse compromisso é uma reunião.  <br/> |
|Received  <br/> |0x0002  <br/> |Esse compromisso foi recebido.  <br/> |
|Cancelado  <br/> |0x0004  <br/> |Esse compromisso foi cancelado.  <br/> |
   
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

